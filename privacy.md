# OutBeat privacy notice

**Last updated:** 5 October 2026

## Who we are

OutBeat is a Windows app. It is developed by Joshua Roldan Burgos ("Owa") and sold by Sam
Beljon Catapusan through Gumroad. Sam is the seller, is in the Philippines, and is responsible
for the data described in this notice.

Contact for anything in this notice: **joshuart.1499@gmail.com**.

## The short version

- Your designs, settings, pictures, sounds, fonts and sign-ins stay on your PC and are not sent
  to us.
- Gumroad handles your payment and holds your name and email. We don't copy them into the
  activation service or the usage data. If you email us or use the feedback form, we keep what
  you send (see below).
- To run Pro on up to two PCs, a small activation service keeps scrambled IDs for your PCs, the
  names you give them and some dates. No name, no email.
- Usage data is off unless you say yes when OutBeat first asks. It is anonymous and you can turn
  it off any time.
- We never sell your data. No third-party ads; OutBeat's own Pro and Shop may appear in the
  editor, never on your stream.

## What stays on your PC

OutBeat keeps these in its folder on your PC and does not send them to us: your designs and
presets, settings, uploaded pictures, sounds and fonts, your Twitch sign-in, your Euler Stream
key, your lyrics cache, and a private key that lets your second PC show your stream output on
your own network.

The music OutBeat shows is read from Windows on your PC. It is not sent to us. Two lookups do
leave your PC, described under "Services OutBeat talks to".

## Buying Pro (Gumroad)

You buy Pro on Gumroad. Gumroad collects what it needs for the payment, including your email,
and sends you your licence key. Gumroad's own privacy policy covers that. In Gumroad's seller
dashboard, Sam and Owa see, for each order: your email address, your name if you gave
one, your country (from your internet address at purchase), what you bought, the price and
date, your licence key, how you found the product (for example Gumroad Discover or a referral
link), any discount code, your rating if you left one, and whether it was refunded.

If you joined the referral program, Gumroad handles your affiliate account and payouts.

## Activating Pro (our activation service)

**Why:** to let Pro run on up to two PCs, let you free a slot with "Deactivate this PC", let us
reset a slot when you email us, and stop Pro after a refund.

**What is stored:**

| Item | What it is |
|---|---|
| A scrambled form of your licence key | A one-way hash, so the key itself is not kept |
| A scrambled PC ID | Made from a random ID that OutBeat creates when it is installed, hashed with your key |
| A scrambled Windows hint | A hash of your Windows installation's ID, hashed again on our side, so a reinstall on the same PC gets its slot back. The Windows ID itself never leaves your PC. |
| PC names you choose | For example "Streaming PC". If you leave it blank we use "PC 1" or "PC 2". OutBeat never sends your Windows computer name. |
| Dates | When each PC was activated, last checked in, and freed, and whether it was freed by you, by support or for being away 60 days |
| Purchase status | Gumroad's answer about your key (good, refunded, disputed, chargeback, turned off) and when we last asked |

**What is not stored:** your name, email, licence key in readable form, or your Windows ID.

**How it works:** when you activate, and about once a week after that, the app checks in with
the service. The service asks Gumroad whether your key is still valid.

**Where:** on Cloudflare Workers. The data is stored by Cloudflare, placed in the Asia-Pacific
region.
Like any web service, Cloudflare sees your internet address when the app connects. Our service
does not save it in its records. Cloudflare keeps short technical logs of each connection, which
can include your internet address, for 3 days, so we can fix problems.

**How long:** a PC that has not checked in for 60 days loses its slot automatically.
Records of freed slots and refunded keys (the scrambled IDs, PC names and
dates above; no name or email) are kept for 12 months after the slot is freed or the key is
refunded, so we can help when you write in. Then they are deleted. Records for a key that has
not been refunded (including one Gumroad has turned off) are kept for as long as the key exists,
so Pro keeps working and we can help you.

## Anonymous usage data (PostHog), only if you say yes

The first time you start OutBeat it asks: "Help improve OutBeat with anonymous usage data?" If
you say no, nothing is sent.

If you say yes, OutBeat sends a small amount of information to PostHog, the analytics service
we use: which editors you open, which built-in styles and parts you pick, when you try a Pro
item or open the Upgrade screen, whether activation worked (never your licence key), your
OutBeat version, Free or Pro, your Windows version, whether you use Twitch or TikTok (never
your channel or username), and how many errors happened.

- It is linked to a random ID made on your PC for this purpose only, not to your name, email,
  licence or PC, and not to the activation IDs above.
- We never send your name, email, licence or Euler Stream keys, what you listen to, chat
  messages, Twitch or TikTok usernames, or anything from your TikTok LIVE events.
- Your stream output never sends usage data.
- Your internet address is used only to estimate your country and is then discarded.

- Usage data is stored by PostHog in the European Union.

- How long PostHog keeps it: 1 year, then it is deleted (PostHog's free plan).

**Turning it off:** in the app, Theme → Usage data. Sending
stops straight away and the random ID is deleted from your PC. Because the data is not linked to
you, we cannot find "your" data to delete it on request; turning it off is how you stop it.

## Feedback form in the app

The chat bubble on the app's front page sends us a message. It asks for your email and up to 500
words; your Discord name is optional. You can attach one screenshot, which the app shrinks
first. The app also adds which version of OutBeat you are using.

We use it to read and answer your feedback. It is stored in a Google Sheet, with screenshots in
a Google Drive folder, in OutBeat's own Google account, through a Google Apps Script. (OutBeat versions before 2.13.0
send feedback to an older mailbox in the developer's own Google account.)

We keep feedback messages and screenshots for 12 months after your last message, then delete
them.

## Support emails

If you email **joshuart.1499@gmail.com**, we keep the email thread to help you. Sam and Owa
both answer. We use Gmail, and AI assistants (currently Anthropic's Claude) that may read an
email to help us sort it or draft a reply. A person checks every reply before it is sent.

We keep support emails for 12 months after your last message, then delete them.

## Services OutBeat talks to

| Service | When | What it receives |
|---|---|---|
| **Gumroad** | When you buy, and when our service checks your key | Your purchase; your licence key from our service |
| **Cloudflare** | When you activate, check in or deactivate | The activation data above; your licence key, passed to Gumroad to check it and not stored; your internet address as part of the connection |
| **PostHog** | Only if you said yes to usage data | The usage data above |
| **Euler Stream** | When you connect TikTok LIVE | A request to connect to the LIVE room, with its room number (not your TikTok username), and your Euler Stream key if you added one. TikTok data comes straight to your PC and never passes through our servers. |
| **TikTok** and **Twitch** | When you connect them | The requests needed to read your alerts, goals and chat. Your Twitch sign-in stays on your PC. |
| **LRCLIB** (lrclib.net) | Only when the lyrics page is on | The song title, artist, album and length |
| **Apple's iTunes Search** | When the album art Windows gives is too small and OutBeat looks for a sharper copy | The artist and song title |
| **GitHub** (and jsDelivr, a mirror of GitHub files) | When the app checks for updates, downloads one, or you open the Shop | A normal download request |
| **Google** | When you send feedback | Your feedback message, as above |

This sharper-art lookup is on by default. You can turn it off with "Sharper album art" in the
OutBeat tray menu.

Each of these services handles data under its own privacy policy.

## Your choices and rights

- **Usage data:** say no at first start, or turn it off any time.
- **Free a PC:** "Deactivate this PC" in the app, any time.
- **Ask, correct or delete:** email **joshuart.1499@gmail.com**. We can delete your activation
  records (this frees your PC slots; you can activate again with your key), your feedback
  messages and your support emails. Your purchase record stays with Gumroad; ask Gumroad about it.
  To confirm it is you, write from the email you bought with on Gumroad and include your licence
  key (it is how we find your activation records, since we never store your email there). For
  feedback or support emails without a purchase, writing from the same email address is enough.

- We reply within 2 business days and finish your request within 30 days.

**The law that applies:** the seller is in the Philippines, and Philippine law applies,
including the Data Privacy Act of 2012. If you have a complaint about how we handle your data,
you can take it to the National Privacy Commission.

## Children

OutBeat is for people aged 18 and over. We don't knowingly collect data from anyone under 18.
If you think someone under 18 has sent us data, email us and we will delete it.

## Changes

If we change this notice, we update the "last updated" date at the top and say what changed in
the app's "what's new" notes and on the product page. For big changes, we also email buyers
through Gumroad.
