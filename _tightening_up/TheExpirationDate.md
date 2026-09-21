---
title: "The Expiration Date: Why \"It Still Works\" Doesn't Mean \"It's Still Safe\""
description: "What end-of-life technology actually means, why it's one of the most common ways small businesses get breached, and how to find and fix what's already expired in your office."
date: 2026-09-16
order: 5
---

Milk doesn't ask permission before it goes bad. It just sits in the fridge looking exactly the same, right up until the day it very much isn't.

Old software and old hardware work the same way. Nothing changes on the outside. The screen still turns on. The program still opens. That's exactly the problem — there's no smell test for a server that quietly stopped being safe two years ago.

## What "end of life" actually means

Every piece of software, and most hardware, comes from a manufacturer who eventually decides they're done maintaining it. When that happens, a few different things stop, and it's worth knowing the difference:

- **Feature updates stop first.** No new capabilities, no redesigns. Not a security problem on its own.
- **General support stops next.** Your vendor won't troubleshoot it anymore, and documentation or help desk access usually dries up too.
- **Security patches may stop too, and this is the part that matters most for security.** Once your product is outside its security-update coverage, you can no longer count on the vendor to fix newly discovered vulnerabilities. Some products offer extended coverage, so check the exact version and support arrangement before assuming updates have ended.

Some vendors give you a bridge between these stages. Windows 10 is a good example: standard support for Windows 10 version 22H2 ended on October 14, 2025. For eligible business PCs enrolled in Microsoft's commercial Extended Security Updates (ESU) program, critical and important security updates can continue for up to three years after that date, with coverage purchased annually. This is not automatic, and it does not restore new features or general technical support. Businesses need to confirm that each PC is eligible, enrolled, and covered for the applicable year. Think of ESU as extra time to finish the move, not permission to put the moving boxes in the attic and forget about them. [Microsoft explains the commercial ESU program here](https://learn.microsoft.com/en-us/windows/whats-new/extended-security-updates).

Not every vendor offers a bridge like that. Plenty of software and hardware has exactly one hard stop date, and once you're past it, you're past it.

## Why this is quietly one of the most common ways in

This is the easiest risk in the whole series to ignore, because nothing about it looks urgent. A phishing email at least looks like something is happening. An unpatched server just keeps running, right up until it doesn't.

The 2017 Equifax breach, 147 million people's personal data exposed, traced back to one thing: a known vulnerability in a piece of software the company hadn't patched. Not a sophisticated attack. Not a criminal mastermind. Just an update nobody applied.

That's not a one-off story. Verizon's latest breach report found that exploiting a vulnerability that already had a fix available was the way in for roughly 3 out of every 10 breaches last year, the single most common cause, ahead of stolen passwords for the first time ever. Other research puts it even higher, with some studies finding that up to 60% of breach victims can trace it back to a patch that existed and simply wasn't installed.

It's not only aging computers, either. Firewalls and VPN devices, the boxes that sit quietly in a closet for years without anyone thinking about them, have become one of the fastest-growing targets. Verizon's research found exploitation of these devices jumped from about 3% of attacks to 22% in a single year. Attackers have figured out that the device guarding your network is often the one piece of equipment nobody's logged into since the day it was installed.

Same theme as the rest of this series: it's the boring stuff that gets you.

## Where to actually look

Old operating systems get the headlines, but they're rarely the only thing quietly aging out in a small business. Worth walking through:

- **Workstations and laptops.** Check the operating system version in Settings, and compare it against the manufacturer's support page.
- **Servers**, especially the one in the closet or supply room nobody's touched since it was installed. If nobody remembers the last time it was rebooted, that's worth a second look on its own.
- **Line-of-business software**: accounting, estimating, scheduling, or anything industry-specific still running a version the vendor stopped supporting years ago. Check the "About" or "Help" menu for a version number.
- **Network equipment**: firewalls, routers, switches. If you've never logged into the admin panel yourself, or didn't know that login existed, that's a sign nobody's been maintaining it.
- **Point-of-sale and payment systems**, especially if you're handling card data directly. An outdated POS system is a security problem and a compliance problem at the same time.

## When you'll actually find out

Here's the good news: manufacturers announce these dates years in advance. Microsoft published Windows 10's October 2025 end-of-support date back in 2021, four years ahead of time. This was never a surprise inspection. It's been public information the entire time, which means the businesses that get caught off guard usually aren't unlucky. They just never looked.

The mistake I see most often isn't ignorance, it's timing. A lot of businesses only start paying attention once the deadline is a few weeks out, which turns a plannable, unhurried upgrade into a rushed, expensive one. Checking now, whenever "now" happens to be for you, is always cheaper than checking during the scramble.

## How to actually fix this

Three steps. None of them require a computer science degree.

**1. Build a quick inventory.** Walk through the list above and write down what you're running and its version. This doesn't need to be fancy. A spreadsheet with device name, what it does, and version number is enough to start.

**2. Check support status for each one.** Search "[product name] end of life" or "[product name] end of support," and the vendor's own lifecycle page usually comes up first. If you genuinely can't find an answer, that's worth asking your IT provider directly instead of guessing.

**3. Decide a path for anything already past its date.** Usually that's upgrading or replacing it. But if something can't be replaced right away, maybe it's specialized equipment that only runs on one old controller, the real answer is isolation: get it off your main network, onto its own segment with no direct internet access, so a vulnerability in that one device can't become a doorway into everything else. That's not a permanent fix, but it buys you time without leaving the front door open.

If you find something already past its expiration date, that's not a reason to panic. It just means you know something now that you didn't an hour ago, which is exactly how every fix in this series starts.

One more reason this matters beyond security: unsupported technology is also one of the fastest ways to get a cyber insurance claim denied after the fact. Worth keeping in mind once you actually look at what your policy assumes you're running.

