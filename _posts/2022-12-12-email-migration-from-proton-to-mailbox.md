---
title: 'Email migration from Proton to Mailbox'
date: '2022-12-12 23:31:58'
last_modified_at: '2022-12-12 23:32:01'
categories:
  - 'Internet'
tags:
  - email
  - proton
  - mailbox
description: 'Migrating a whole email, calendar and contacts ecosystem from Proton to Mailbox. On both desktop and mobile.'
excerpt: 'The main reason for embarking on such a task has a very short answer: I can’t support the fact of being trapped in a <a href="/ethics/">walled garden</a>. When I chose Proton years ago I wasn’t bothered by the concept.'
---
It also costs more than [Mailbox.org](https://mailbox.org), the competitor that mostly appealed to me, while offering less features. I'm going to save around €20 per year: money that can be redirected to other digital venues.

With Proton I’m not allowed to use any system app such as Calendar and Contacts, which makes a proper sync quite cumbersome. External email clients are barely supported — on desktop only — and require a special application called Bridge running in the background at all times. It supports a very limited number of mail applications, such as Apple Mail, Thunderbird and Outlook.

Mailbox.org is hosted in the EU (Germany) on green servers.

## The process

The following has been done on macOS (Catalina).

After getting the gist of how the various services and settings work in my new Mailbox account, I've added €3 to become a paying customer. I like this formula, as it leaves me free to fully experiment for a while without committing to an annual payment yet.

I got 50 aliases, including for my custom domains. Setting them up was as easy as adding a bunch of DNS values (TXT and MX) after authenticating the domains with Mailbox. I can also improve the spam reputation by [adding SPF, DKIM and DMARC](https://kb.mailbox.org/en/private/custom-domains/spf-dkim-and-dmarc-how-to-improve-the-spam-reputation-of-your-domain).

Mailbox gave me automatic configuration profiles for email, calendar and contacts. While preferring a manual setup for IMAP and SMTP on Mail.app, I've chosen the easy and fast procedure for calDAV and cardDAV.

Next, I've exported a full backup of contacts and calendars from Proton. Importing them back on Mailbox was straightforward: all I've used was the import functionality from the default integrated Apple applications. To move the entirety of my 25-thousand emails I relied on a manual migration: selecting large chunks of messages at a time (around 1k), using Mail.app: no issue whatsoever.

All in all, despite dreading the idea of wasting time and energy, it was a surprisingly quick job. From start (zero experience with Mailbox.org) to finish it took no more than a couple hours.

## Side effects

Migrating a whole email system isn't limited to the above. There's also the most frustrating consequence of a bad choice: having a gigantic number of accounts registered with an email address tied to Proton. Could be Gmail or a free Outlook or iCloud or whatever: anything that ties me to a system that's closed in itself and completely outside my control is awfully shortsighted.

I had to alter all my accounts, swapping an address that I'm going to lose soon with one from a personal domain. My domain is under my full control: I can move it from hosting to hosting, change DNS, nameservers, whatever — *it stays with me*, while everything else can disappear. Google, Microsoft, Apple could close my account on a whim, good luck trying to get them back.

In the end, changing email address for a multitude of online accounts took longer than the entire migration. Especially government services.

## Mobile

This was the surprise I enjoyed the most. Being on Android, I feared the idea of having to look for good apps that can support cardDAV and calDAV natively. While reading Mailbox FAQs, I stumbled on an article where they suggested an <abbr title="Free and Open Source Software">FOSS</abbr> app available on F-Droid called [DAVx<sup>5</sup>](https://f-droid.org/en/packages/at.bitfire.davdroid/).

It was just a matter of adding the single Mailbox account in the app and activate calDAV and cardDAV. Afterwards, the integrated Contacts and Calendar apps by Google would simply sync to it. I feel obliged to repeat that I *don't have a Google account* set up with my Android phone, and yet they work seamlessly with Mailbox through DAVx<sup>5</sup> sync.

Email on Android was as easy as setting up a single account on [K-9](https://k9mail.app/) and adding all the identities connected to my domains.

## Conclusions

Only time will tell, but I'm very impressed by Mailbox so far. Can't wait for the first month to end so that I can commit for a full year.