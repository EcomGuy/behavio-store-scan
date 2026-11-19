# Behavio Store Scan

A free Claude skill that scans your Shopify store in about 60 seconds and tells you, in plain dollars, where the store gives away margin and where it loses buyers. Free, MIT, no signup, no API key, no app install.

## What's a skill?

A skill is a short set of instructions you give Claude, like a job description for one task. Once it's installed, you say a trigger phrase ("scan my store") and Claude knows exactly what to do.

## Install

**Option 1: let Claude install it.** Paste this into a new Claude chat:

```
https://github.com/EcomGuy/behavio-store-scan

Install this skill for me, then run it on my store.
```

**Option 2: do it yourself.**

1. Click `SKILL.md` above and download it.
2. Put it in a folder named `behavio-store-scan` and zip the folder.
3. Upload the ZIP in Claude's Skills settings.

**Option 3: Claude Code.**

```
git clone https://github.com/EcomGuy/behavio-store-scan ~/.claude/skills/behavio-store-scan
```

## Use it

Say any of these in Claude:

- `scan my store: yourstore.com`
- `Where is my Shopify store leaking margin?`
- `Audit the offers and discounts on yourstore.com`

Claude asks two quick questions (monthly visitors, ads running right now), reads your public store pages and writes the report.

## What you get

A report under 450 words, always in this order:

| Section | What it tells you |
|---|---|
| Score | Your store out of 100, and how your offer mix compares with the leaders in your niche |
| The money | Monthly margin leak and conversion upside, as a range, with every assumption in a table |
| Top 3 fixes | What it saw on your store, what the niche leaders do, and the fix in one sentence |
| All 14 checks | Score and one-line finding for each check |
| Discount exposure | What you give every visitor, and which of them would likely have paid full price |
| Next step | The do-it-yourself route first, Behavio as an option only for stores with 5,000+ monthly visitors |

## The 14 checks

| Group | Checks |
|---|---|
| Offers & margin (25%) | Offer map, discount exposure, force targeting |
| Psychology & UX (20%) | Persuasion stack by the button, defaults and decoy, urgency credibility |
| Basket builders (15%) | Bundles, quantity tiers, cross-sell, gift with purchase |
| Retention (10%) | Subscription, loyalty, referral |
| Trust (10%) | Trust and proof, product page structure |
| Shipping (10%) | Free shipping strategy, threshold execution |
| Payment & personalization (10%) | Shop Pay and pay-in-4, quiz or finder |

## Good to know

- **Read-only.** It reads only public pages anyone can open: home page, `products.json`, top product pages, shipping and refund policies. It never asks for a login, an admin link or an API key, and never changes anything in your store.
- **Nothing leaves the chat.** Your store data is not sent anywhere.
- **Every dollar figure is an estimate.** It comes from your two answers plus stated assumptions, shown as a range, never a single number.
- **It can miss what loads later.** Pop-ups and widgets that appear only after JavaScript runs may not be visible to Claude, so some checks can come back "not visible".
- **Small stores get the full scan, not a sales pitch.** Under 5,000 monthly visitors, the report says Behavio is not a fit yet.

## About

Made by [Behavio](https://behavio.io), a Shopify app that decides per visitor whether to show an offer, and which one, so discounts go to hesitant shoppers and not to buyers who were going to pay full price. It measures itself against a holdout group of your own visitors.

## License

MIT. Take it, change it, use it.
