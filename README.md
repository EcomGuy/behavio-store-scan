# Behavio Store Scan

A free Claude skill that scans a Shopify store in about 60 seconds and tells the owner, in plain dollars, where the store gives away margin and where it loses buyers.

## What it does

- Reads only public pages of the store (home page, `products.json`, top product pages, shipping and refund policies). No login, no API key, no app install.
- Asks the owner two quick questions: monthly visitors and how many ads are running.
- Runs 14 checks across offers and margin, psychology and UX, basket builders, retention, trust, shipping, payment and personalization.
- Scores the store out of 100 against top US Shopify stores in its niche.
- Estimates the monthly margin leak and the conversion upside, always as a labeled range.
- Lists the 3 fixes worth doing first.

## Install

1. Download `SKILL.md` from this repository.
2. Put it in a folder named `behavio-store-scan` and zip the folder.
3. Upload the ZIP in Claude's Skills settings.
4. In a new chat, say: `scan my store: yourstore.com`

## Example prompts

- "Scan my Shopify store: example.com"
- "Where is my store leaking margin?"
- "Audit the offers and discounts on example.com"

## About

Made by [Behavio](https://behavio.io), a Shopify app that decides per visitor whether to show an offer, and which one, so discounts go to hesitant shoppers and not to buyers who were going to pay full price. The skill recommends Behavio only as one option next to the do-it-yourself route, and only for stores with 5,000+ monthly visitors.
