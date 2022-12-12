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

I got 50 aliases, including addresses for my domains. Setting them up was as easy as adding a bunch of DNS values (TXT and MX) after authenticating the domains themselves with Mailbox. I can also improve the reputation by [adding SPF, DKIM and DMARC](https://kb.mailbox.org/en/private/custom-domains/spf-dkim-and-dmarc-how-to-improve-the-spam-reputation-of-your-domain).

They gave me automatic configuration profiles for email, calendar and contacts. While preferring a manual setup for IMAP and SMTP on Mail.app, I've chosen the easy and fast procedure for calDAV and cardDAV.

Next, I've exported a full backup of contacts and calendars from Proton. Importing them back on Mailbox was straightforward: all I've used was the default import functionality from the default integrated Apple applications. To move the entirety of my 25-thousand emails I relied on a manual migration: selecting large chunks of messages at a time, using macOS' integrated Mail.app.

All in all, despite dreading the idea of wasting time and energy, it was a surprisingly quick job. From start (zero experience with Mailbox.org) to finish I think it took a couple hours max.

## Side effects

Migrating a whole email system isn't limited to the above. There's also the most frustrating consequence of bad choices: having a load of accounts registered under an address tied to a walled garden. Could be Proton like in my case, could be Gmail or whatever. Anything that ties me to a system that's closed in itself and completely outside my control is awfully shortsighted.

So, I had to alter all my accounts, swapping addresses connected to Proton (that I'm going to lose soon) to my domains'. My domain is what's under my full control. I can move it from hosting to hosting, change DNS, nameservers, whatever: *it stays with me*, while everything else can disappear. Google, Apple and others could close my account on a whim, good luck trying to get them back.

In the end, changing email address for a multitude of online accounts took longer than the entire migration.

## Mobile

This was the surprise I liked the most. Being on Android, I feared the idea of having to search for good apps that can support cardDAV and calDAV natively. While reading their FAQs, I stumbled on an article by Mailbox where they were suggesting an open source app available on F-Droid called [DAVx<sup>5</sup>](https://f-droid.org/en/packages/at.bitfire.davdroid/).

It was just a matter of adding the one Mailbox account in that app and activate calDAV and cardDAV. Afterwards, the integrated Contacts and Calendar apps by Google (or any other default) would simply sync to it. I feel obliged to repeat that I *don't have a Google account* set up with my Android phone, and yet they work seamlessly with Mailbox.

## Conclusions

Only time will tell, but I'm very impressed by Mailbox so far. Can't wait for the first month to end so that I can commit for a full year.