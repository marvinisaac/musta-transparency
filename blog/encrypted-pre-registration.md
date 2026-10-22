---
title: Encrypted Pre-registration
description: Privacy from the very start, not as an afterthought
date: 2026-10-20
---

Even during early development, my chosen path is already proving harder than I initially anticipated.

A traditional pre-registration system for future customers should be straightforward:
1. Create an email collection form in the website.
2. Create an API to handle incoming requests.
3. Save email addresses in a database.

But Musta has a privacy promise to uphold even this early in development. That makes something as simple as email collection significantly harder.

These are the problems I encountered during planning:
1. **Email addresses cannot be stored in plaintext.** The database should only contain encrypted values, never plain email addresses. Even if the database's remote backups are compromised, the stored email addresses should still be unreadable. Hashing is one way to achieve this goal but that solution is incompatible with the next problem.
2. **Invitations will be sent in the future.** Hashing any value is a one-way operation. Sending invitation emails in the future requires plain email addresses which means decrypting the previously encrypted values which, in turn, means storing the decryption key somewhere.
3. **Decryption keys must not be in the server**. Similar to the database, when the server gets compromised, the attacker should be able to extract no information. Storing the decryption key in the server, therefore, is not an option.

The goal is to design Musta so that even if the API and the database are both compromised, the attacker will be able to extract as little information as possible. This is an ambitious threat model but the project's privacy-first focus means these constraints are non-negotiables.

This means building three components:
1. **An admin dashboard.** This will work similar to the main website except there's only one person using it: me. For now, this dashboard will only be used to decrypt encrypted email addresses and trigger sending of actual invitation email in the future. After the email has been sent, the encrypted email addresses will be removed from the database. On login, the admin account's private key will also be deterministically reconstructed and stored in-memory only.
2. **A small slice of the "dumb server".** This will eventually grow to become the API for the main website as well. For now, the API will only handle a) saving encrypted email addresses, b) returning those encrypted values to the admin dashboard, and c) sending the invitation email in the future. Only during the last step will it see the actual email addresses.
3. **Updating the main website with my admin account's public key.** When someone requests to be invited, this would enable the main Musta website to encrypt the actual email address before sending the ciphertext to the API.

Even with all that, the current setup still has some vulnerabilities:
- Musta's website is served through Cloudflare Pages. Even if a bad actor gains control of the server, the frontend still sends encrypted data. However, if my GitHub account is compromised, they can theoretically change the site's code to skip encryption entirely and send the plaintext values to the server.
- If an attacker takes over the server but patiently waits for actual email sending operation, they can theoretically see the plain email address.
- My admin private key is never saved but if my own device is ever compromised, an attacker could potentially exfiltrate the private key from memory.

What I thought was a simple pre-registration form became a warm-up exercise in designing a system with privacy at its core. It has not been easy but now I understand more concretely why it is almost impossible to add this level of privacy as an afterthought.
