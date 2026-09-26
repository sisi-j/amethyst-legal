---
layout: page
title: Privacy Policy
permalink: /privacy/
---

**Last updated: 26 September 2026**

This policy explains what the Amethyst network of Discord apps (**Donut
Verify**, **Global Schematics**, **Donut Server Trust** and **Amethyst Team
Bot**) and the verification website at `verify.aerialdesign.org` collect,
why, who can see it, how long it's kept, and how to have it deleted. It's
written from what the software actually does.

Amethyst is a community project run by the Amethyst team ("we", "us"). It is
not affiliated with DonutSMP, Mojang Studios, Microsoft or Discord.

## The short version

- We store the minimum needed for each feature: mostly Discord IDs, in-game
  names, and the things you choose to submit.
- **We never read your messages.** None of the apps has access to message
  content; they only see the commands and buttons you use.
- We don't sell data, show ads, or use anything for AI training.
- `/unlink` deletes your verification data immediately.
- Everything runs on our own server; off-site copies are encrypted backups.

## What we collect, by app

### Donut Verify

| What | Why |
|---|---|
| Your Discord user ID, and the Minecraft name and ID (UUID, when available) you verify as | To remember the link across every server in the network |
| Which method you used, and when you verified | To show on `/whois` and to decide whether a server's requirements are met |
| **Official-link method:** your nickname on the official DonutSMP Discord and the date you joined it | That nickname is what DonutSMP sets when you link there; it's how this method proves the account is yours |
| **Payment method:** the random amount you were asked to pay, and the in-game balances of your account and the receiving account at the start | Verification works by checking your balance went down and the receiver's went up by exactly that amount |
| The servers where you received the verified role | So `/unlink` can remove the role everywhere |
| Each server's verification settings (methods, role) | To run verification the way that server chose |

For the official-link method you sign in with Discord and grant one
permission, `guilds.members.read`. We use it once, to read your membership in
the official DonutSMP Discord (nickname and join date), and **don't keep the
Discord sign-in token**.

When you or anyone runs `/whois` on a linked account, the app fetches that
player's **public** DonutSMP stats (money, shards, playtime, kills and
deaths, blocks placed) live from DonutSMP to display. We don't store them.

### Global Schematics

| What | Why |
|---|---|
| Schematics and screenshots you upload, with the name, description, stats, instructions, tags and category you give them | To publish them in the library |
| Your Discord user ID as the poster, and the in-game name you enter (optional, not verified) | Shown on the listing so people know who built it |
| The server you submitted from | Record-keeping for reviews |
| Who has downloaded each listing | Only people who downloaded a build can rate it |
| Ratings you give (1–5 stars) | Shown only as an average and count |
| Categories you follow | To DM you when something new is approved there |
| Reports you file about listings, and the team's review decisions | Moderation |

### Donut Server Trust

| What | Why |
|---|---|
| Server IDs, names and member counts of servers that are checked, rated or reported | So they can be looked up by name |
| Ratings you give a server (trust, reliability, optional pricing) with your Discord ID and the date you joined that server | One rating per person per server, and only members of 7+ days may rate |
| Reports you file: your Discord ID, the reason and the evidence you provide | For the Amethyst team to review |

### Amethyst Team Bot and operations

The team bot is used only by the Amethyst team, in one private server. It
records who approved or rejected submissions, who resolved reports and any
team actions such as unlinking an account or banning someone from submitting
schematics (with the reason), for accountability.

The apps also keep short technical records: DonutSMP API request logs
(including the player names looked up) for **24 hours**, and service logs
that include Discord IDs and actions, which are **overwritten as they fill**,
typically within a few weeks.

## Who can see what

| Visible to | What |
|---|---|
| **Anyone** using the apps in any server on the network | Your verified Minecraft name, method and date, plus live public DonutSMP stats, via `/whois` or right-click → *Minecraft account* |
| **Anyone** who can see a listing | The listing, its files and screenshots, your Discord account as poster, the in-game name you entered, and its average rating |
| **Anyone** checking a server | Its average ratings and number of **confirmed** reports. Individual ratings and who gave them aren't shown |
| **The Amethyst team** | Everything above, plus report contents and evidence, pending submissions, and verification records, for moderation and support |

Server reports are never posted publicly. If a report is resolved, the
person who filed it is told the outcome by DM.

## Who else receives data

We don't sell or rent data. It leaves our server only where a feature needs
it:

- **Discord**, which runs the platform: everything you do through the apps
  passes through Discord. [Discord Privacy Policy](https://discord.com/privacy)
- **DonutSMP's public API**, which receives the in-game names we look up
  (to check an account exists, read balances for payment verification, and
  show `/whois` stats).
- **Cloudflare**, which carries the verification website's traffic and
  stores our encrypted off-site backups (Cloudflare R2).
  [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/)

Minecraft textures used to draw schematic renders are downloaded from Mojang;
no personal data is sent. We may disclose data if the law requires it.

## How long we keep it

| Data | Kept |
|---|---|
| Your verification link (for payment verification, including the amount paid and starting balances) | Until you `/unlink`, or the team removes it |
| Verification attempts (including payment balances) | Deleted after **30 days**, or immediately on `/unlink` |
| Schematics, listings, ratings, downloads, follows | While the listing or the library exists |
| Server ratings and reports | While the network runs, as the trust record depends on them |
| DonutSMP API request logs | 24 hours |
| Service logs | Overwritten as they fill (typically a few weeks) |
| Backups | 7 days on our server, 14 days off-site |

Deleted data can remain in backups until those backups expire.

## Deleting your data and your choices

- **Verification:** run `/unlink`. Your link, verification attempts and the
  record of servers where you got the role are deleted straight away, and the
  verified role is removed where possible.
- **Anything else** (listings, ratings, reports, follows): open an issue on
  [this site's GitHub repository](https://github.com/sisi-j/amethyst-legal/issues/new)
  asking for deletion. Issues are **public**, so include only your Discord
  username; we'll confirm it's you over Discord and then delete it.
- **Follows:** `/schematic watch` lets you untick categories, or stop all alerts, at any time.
- Server admins can remove any app from their server at any time.

Depending on where you live (for example under the GDPR in the EU/UK or
privacy laws in some US states), you may have rights to access, correct,
delete or object to the use of your data. Ask through the GitHub issue link
above and we'll respond within 30 days. We rely on providing the service you
asked for, and our legitimate interest in keeping it safe and free of abuse,
as the reasons for processing.

## Security

The apps run on a private server we control, with access restricted to the
Amethyst team. Stored files and the database aren't exposed to the internet;
only the verification website is, through Cloudflare. Off-site backups are
encrypted by Cloudflare. No system is perfectly secure, but we keep what we
store to a minimum.

## Children

The Service is meant for people old enough to use Discord where they live
(at least 13). We don't knowingly collect data from anyone younger; if you
believe we have, open an issue and we'll delete it.

## Changes

If we change this policy, the date at the top will change, and significant
changes will be announced where reasonably possible.

## Contact

[Open an issue on GitHub](https://github.com/sisi-j/amethyst-legal/issues/new).
Please don't post personal details publicly; we'll follow up on Discord.
