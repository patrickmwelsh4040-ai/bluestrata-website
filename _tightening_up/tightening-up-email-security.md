---
title: "The Mail Slot: The Email That Looks Completely Normal"
description: "How phishing, impersonation, and business email compromise get past otherwise careful small businesses."
date: 2026-09-08
order: 3
---

Your business has a front door: the login, protected by a passphrase and hopefully MFA. This article isn't about that door. It's about the mail slot.

Sometimes an attacker doesn't have to break into anything. Sometimes they just send an email.

And the ones that actually cause damage don't look dangerous. They look like an invoice from a vendor you already work with. A note from your boss asking you to handle something before lunch. A Microsoft alert telling you your password is about to expire.

Nothing about it looks wrong, but that's exactly the point.

## The obvious phishing email isn't the one I worry about

Everybody knows what the classic phishing email looks like. Bad spelling. Strange formatting. A stranger informing you that you've inherited $14 million from an uncle you've never heard of.

Those still show up. They're not the ones I worry about.

The ones that actually work have a little homework behind them. Your website tells an attacker who your employees are. LinkedIn tells them who runs Accounting. Social media might tell them the owner is currently sitting on a beach somewhere. None of that is secret information on its own, but put enough of it together and you can write an email that sounds exactly like your business.

Something like:

> *Hey Sarah, I'm tied up with a client right now. Can you get this invoice taken care of before end of day? They updated their banking info, so use the account on the attached.*
>
> *Thanks.*

That email doesn't need malware. It doesn't need a clever exploit. It just needs Sarah to believe it's actually her boss.

The FBI has a name for this: Business Email Compromise, or BEC. And it works so well because the attacker isn't attacking your computer. They're attacking the conversation.

## There's more than one way to fake an email

When somebody says an email was "spoofed," that can mean a few different things.

The simplest version just changes the display name. Your inbox might show:

Michelle Garcia

...while the actual address underneath is something like michelle.garcia.company@gmail.com. If you're reading on your phone at 7am, you'll probably never notice.

A step up from that is a lookalike domain. Your vendor's real domain might be coloradosteel.com. The attacker registers colorad0steel.com with a zero standing in for the letter O. That one character is doing all the work.

The version that actually worries me is when the attacker gets into somebody's real mailbox. Now there's nothing fake about the sender. It really is coming from your vendor's account, possibly from inside a thread you're already in. They read the thread, see an invoice is about to go out, and send new payment instructions right on schedule.

## Money changes get a phone call, not a reply

If there's one rule to take out of this article, it's this: never change payment information based on an email alone.

New bank account? Call the vendor.

Updated ACH instructions? Call the vendor.

Somebody suddenly wants a wire instead of a check? Call the vendor.

And don't call the number sitting in the email. Use the number you already had on file before this message showed up. If I can fake the email, I can put whatever phone number I want at the bottom of it.

The FBI's own guidance comes down to the same thing: verify anything involving money through a separate, already-trusted channel.

It sounds too simple to matter. It's not. A two-minute phone call stops something your firewall was never going to catch.

## Three acronyms worth knowing

I'm not going to bury you in jargon here, but email security has three acronyms you should at least recognize, even if you never touch the settings yourself: SPF, DKIM, and DMARC.

You don't need to configure these, you just need to know whether somebody already has.

**SPF** tells the rest of the internet which systems are allowed to send email as your domain. If you're on Microsoft 365 (and most of the businesses I work with are) your DNS records can say "Microsoft is allowed to send mail as us." Someone sending from somewhere else now has a much harder time pretending to be you@yourcompany.com.

**DKIM** adds a digital signature to your outgoing mail. The receiving system checks that signature to confirm the message actually came from your domain and wasn't altered along the way. You never see any of this happening. That's by design.

**DMARC** ties the two together. It tells other mail servers what to do when a message claiming to be from your domain fails those checks â€” monitor it, quarantine it, or reject it outright. It can also send you reports showing where mail claiming to be "you" is actually coming from.

SPF says who's allowed to send. DKIM proves the message wasn't tampered with. DMARC decides what happens when something doesn't add up.

That's the plain-English version. Hope it helps.

## These settings don't stop phishing on their own

This part matters: you can configure SPF, DKIM, and DMARC perfectly and still get phished.

They make it harder to directly impersonate your exact domain. They don't stop a lookalike domain. They don't stop an attacker who's already sitting inside a vendor's real mailbox. And they definitely don't stop an employee from typing their password into a convincing fake Microsoft login page.

There's no single switch that turns phishing off. Email security is layers, stacked on top of each other. Your mail provider filters what it can catch. Domain authentication makes spoofing harder. MFA makes a stolen password less useful. Your employees learn what deserves a second look. And your internal process makes sure one believable email can't move $40,000 out the door without somebody picking up the phone first.

None of those layers is perfect by itself. Stacked together, they make the attacker's job considerably harder. That's the goal. Not perfection, just enough friction that the easy version of the attack stops working.

## Give employees something specific to watch for

Telling people to "be careful with email" doesn't accomplish much. Careful about what? Everything? Your team gets hundreds of legitimate emails a month and you can't expect them to treat every single one like a digital crime scene.

Give them specific triggers instead. Slow down when an email:

- changes where money is supposed to go
- asks for a password or an MFA code
- creates unusual urgency
- includes an attachment you weren't expecting
- sends you to a login page through a link
- changes a normal process
- comes from someone senior asking you to keep it quiet

None of those automatically means the email is bad. It means it's earned a second look before anyone acts on it.

And make it easy to report something that feels off. If an employee's first thought after clicking a bad link is "I'm going to get in trouble," they'll sit on it and hope nothing happens, which is the worst possible outcome. I'd rather hear about a bad click five minutes after it happens than find out about it three weeks later because someone was embarrassed to say anything.

## Your homework

This one has two parts.

First, ask whoever manages your email three questions: Do we have SPF configured? Is DKIM enabled? Do we have a DMARC record, and what is it actually set to do? If the answer to any of those is "I don't know," write that down. That's useful information on its own.

Second, look at how your business actually handles money changes. If a vendor emailed Accounting tomorrow saying they'd switched banks, could one person update the payment info and send money without confirming it any other way? If the answer is yes, fix the process. Not the computer. The process. A known phone number, a second set of eyes, an approval step or whatever fits the needs of your business. The point is that an email by itself should never carry enough authority to redirect your money.

Email is the door attackers use most often, but it's not the only one. If a phishing attempt gets through anyway, or a laptop dies, or ransomware hits, the next question is whether you can actually get your data back. A lot of businesses find out the hard way that having backups and being able to restore from them are two very different things.

