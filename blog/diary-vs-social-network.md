---
title: Diary vs Social Network
description: What is Musta's actual direction and identity?
date: 2026-10-15
---

In a [previous post](/blog/musta-world), I said that Musta is two things at the same time:
1. an online diary / journal, and
2. a way to share specific entries with specific people.

These two things pull directly against each other. The first thing is a private-first app, the second is a sharing-first app with strong privacy. Diary / journal entries are written for a single person: the writer's future self. A social network update is always intended for someone else.

Musta's v1 was trying to be both: a journal app with social sharing features, and a social network with strong privacy defaults. I only realized the contradiction while writing the project's manifesto because those two things constantly fought each other even on things they should have agreed on at first glance: privacy.

A good journaling app is all about keeping the author's data under lock and key. Any online backup stored on a server should be unreadable to anyone, not even the server code. A social network with strong privacy still needs to see some part of the author's data: their entries (or at least their entries' metadata), their connections, and which of those connections can see which entries. Even if the contents are encrypted, some metadata should still remain readable. "Privacy" means the same but, depending on the app's identity, the amount of privacy differs.

My goal with Musta aligns more with the latter, a social network with a strong focus on privacy. I want to know how my cousins are doing, I want to see my nieces and nephews growing up, all without handing their data to big tech.

**Musta, therefore, is a private-by-default social network.** It can be used as an online diary (like I'm usually using it) but that is only secondary, a "happy accident" caused by the project's promise of keeping everyone's data safe.
