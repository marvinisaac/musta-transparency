---
title: Musta Privacy Policy
description: How the Musta website collects, uses, and processes information when you visit.
---

**Last updated: November 2, 2026**

## 1. Introduction

Musta is a project focused on helping people stay connected without sacrificing their privacy. This Privacy Policy explains how the Musta website collects, uses, and processes information when you visit.

The website uses the following:

- Cloudflare Pages for hosting.
- Sentry for error tracking.
- Umami for website analytics.

This policy describes the website's current data-handling practices. It will be updated as Musta develops and introduces additional features.

## 2. Information We Collect

### 2.1. Hosting and Technical Information

Musta's frontend is hosted on Cloudflare Pages. When visitors access the website, Cloudflare may process technical information necessary to deliver, secure, and operate the service, such as IP addresses, request metadata, and security-related information. This is separate from the analytics collected by Umami and the diagnostic information sent to Sentry.

For more information, see the [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/).

### 2.2. Error Tracking and Diagnostics

Musta uses Sentry's hosted service to identify, investigate, and resolve technical errors. When an error occurs, Sentry may receive diagnostic information such as error messages, stack traces, browser and operating system details, and the page or URL associated with the error. Diagnostic reports may inadvertently contain personal information; data scrubbing is enabled to reduce this, but its complete removal cannot be guaranteed. Sentry is used to maintain the reliability and security of the website, not to monitor visitors for advertising purposes.

For more information, see the [Sentry Privacy Policy](https://sentry.io/privacy/).

### 2.3. Website Analytics

Musta uses a self-hosted instance of Umami Analytics to understand how visitors use the website and to improve its content and usability. Depending on the request and configuration, analytics may include:

- Pages visited and page-view counts.
- Referring websites and traffic sources.
- Browser type, operating system, and device information.
- Approximate geographic information derived from visitor IP addresses.

Umami's standard analytics tracker is designed to operate without cookies, and Musta does not track visitors across unrelated websites. The Umami instance runs on hardware operated by the developer rather than through Umami's hosted analytics service, and the developer may access the analytics data for administration, maintenance, and website improvement.

Musta does not use these analytics for targeted advertising or sell visitors' personal information.

For more information, see the [Umami documentation](https://docs.umami.is/docs/faq).

### 2.4. Information You Provide

The current website does not require visitors to create an account or provide personal information to read the development blog. If you voluntarily contact the developer through an available communication channel, the information you provide may be processed to respond to your inquiry.

### 2.5. Waitlist

You may voluntarily join the Musta waitlist by submitting your email address through the "Join the waitlist" form on the home page. Providing it is optional. The rest of the website works without it.

Your email address is encrypted in your browser, before it leaves your device, so only that encrypted form is ever sent. The server receives, validates, and stores ciphertext. It never sees your email address, and no key capable of opening it exists on the server.

Those encrypted addresses can be decrypted only by the developer, only in the developer's own browser, and only to check the list before the actual invitations are sent. Once an invitation has been used to create an account, the waitlist entry it came from is deleted. An invitation the developer revokes without being used does not delete the entry so it can be invited again later.

### 2.6. Accounts

If you receive an invitation, you can create a Musta account with your email address and a passphrase of your choosing. Providing your email address is required to create the account; the passphrase stays on your device and never reaches the server.

Everything the server stores about your account — your email address, the entries in your account site's vault, and your profile details (first name, last name and nickname) — is encrypted before it leaves your browser, and the server holds nothing that can decrypt it. Your profile details are additionally stored so that the server cannot even link them to your account.

When you create the account, your browser also generates a **recovery code**: shown to you once, and never sent to the server or written to your device. If you forget your passphrase, recovering asks for **both** secrets, signs out every other device, and gives you a new passphrase and a new recovery code to write down, replacing both. Losing **both** your passphrase and your recovery code means your encrypted data cannot be recovered. Keep them somewhere separate.

Signing in sets session cookies that contain no personal information — no email address, no passphrase, no key. They exist only so that a session can be renewed and ended, they are removed when you sign out, and they expire at most fourteen days after the sign-in.

## 3. How We Use Information

Information processed through the website is used for the following purposes:

- **Communication:** Respond to inquiries that visitors voluntarily submit.
- **Waitlist and invitations:** Check voluntary waitlist sign-ups, send invitations, and create accounts for the people who use them.
- **Error diagnosis:** Identify, investigate, and resolve bugs and technical failures.
- **Reliability and security:** Maintain the website and investigate technical problems.
- **Website improvement:** Understand which pages and content are useful to visitors.

Invitation emails are delivered through a mail provider, which necessarily processes the invited person's email address and the invitation link in order to deliver the message. Invitations contain no other personal information.

Musta does not sell visitors' personal information or use the analytics and error-tracking tools described in this policy for targeted advertising.

## 4. Cookies and Similar Technologies

The account site uses session cookies when you are signed in. They hold no personal information, are removed when you sign out, and expire at most fourteen days after the sign-in; they exist only so that a session can be renewed and ended, and are not used for analytics, advertising or any form of tracking.

Umami's standard analytics tracker is designed to operate without cookies. Cloudflare Pages and other infrastructure may use cookies or other storage technologies as needed for service delivery and security, depending on the services enabled.

## 5. Data Retention

Analytics and diagnostic information is retained only as needed for the purposes described in this policy, subject to applicable service settings and legal requirements. For self-hosted Umami, retention depends on the developer's database, backup, and deletion practices; Sentry and Cloudflare data retention is subject to their applicable service settings, terms, and policies.

Encrypted waitlist sign-ups are retained only until the invitation they were collected for has been used to create an account, and are deleted at that point.

Account information — your email address, vault entries, and profile details — is retained for as long as the account exists, stored encrypted and unreadable to the server.

A signed-in session is kept for at most fourteen days from the sign-in, and for less when you sign out; the cookies that carry it are removed at sign out.

Musta aims to avoid retaining personal information longer than necessary for the purposes for which it is processed.

## 6. Data Security

Musta aims to minimize the information collected and apply reasonable safeguards to protect it against unauthorized access, disclosure, alteration, or destruction.

These safeguards may include:

- Restricting access to analytics and diagnostic systems.
- Limiting unnecessary information in error reports.
- Enabling data-scrubbing controls in Sentry.
- Securing the hardware and infrastructure used to operate self-hosted analytics.
- Reviewing data retention and deletion practices as the project develops.

However, no website, service, or method of electronic storage or transmission can be guaranteed to be completely secure.

## 7. Your Privacy Rights

Depending on your location and the applicable law, you may have rights concerning your personal information, including the right to:

- Be informed about how your personal information is processed.
- Request access to personal information held about you.
- Request correction of inaccurate information.
- Request deletion or restriction of processing where applicable.
- Object to certain processing activities.
- Lodge a complaint with the relevant data protection authority.

If you are in the Philippines, these rights may arise under the Data Privacy Act of 2012 and its implementing rules, subject to applicable conditions and exceptions.

Because the current website primarily processes analytics and technical diagnostic data, identifying and retrieving information associated with a particular visitor may be limited by the nature of the data collected.

To submit a privacy-related inquiry or request, contact the developer using the contact information provided in Section 9.

## 8. Changes to This Policy

This Privacy Policy may be updated as Musta develops, introduces new features, changes service providers, or modifies its data-handling practices.

The latest version will be published on the website with an updated revision date. Visitors should review this page periodically to understand the current practices.

## 9. Contact

For questions, concerns, or requests regarding this Privacy Policy or the processing of information through Musta, contact:

**Project:** Musta

**Developer:** Marvin Isaac

**Email:** marvin@musta.ph
