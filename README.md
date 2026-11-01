# Rao's Vandana — Google review page

A single-page site that helps customers of **Rao's Vandana Enterprises**, Vijayawada,
leave a Google review in a few taps. Built in the shop's own branding taken from
[raosvandana.in](https://raosvandana.in/).

> Demo page. Not an official website of the business.

## What the page does

1. **About** — the shop's own wording, product categories and address.
2. **Review builder** — the customer taps what matched their visit (quality, papads,
   ravva, millets, price, packing, service), gets an editable draft, and
   "Copy & open Google reviews" copies it and opens the shop's real review box.
   Each option has two phrasings picked at random so no two reviews read alike.
3. **Follow us** — Instagram, Facebook, Pinterest.
4. **Get in touch** — Call, WhatsApp, Email, Website, Google listing, plus an
   "Order on WhatsApp" button.
5. **Visit the store** — opens Google Maps directions.

## Shop details

| | |
|---|---|
| Google place ID | `ChIJ52M_DF3vNToRrOzyq71-YOg` |
| Review link | https://search.google.com/local/writereview?placeid=ChIJ52M_DF3vNToRrOzyq71-YOg |
| Address | 4/7A, D.No 39-2-19/12B, Pragati Nagar Road, opp. Gollapudi, Bhavanipuram, Vijayawada 520012 |
| Phone | 9533777779 (website) · +91 98666 99099 (Google listing) |
| Email | raosvandana@hotmail.com |

## Editing

Everything configurable sits at the top of the `<script>` block in `index.html`:

```js
const SOCIAL = { instagram: "...", facebook: "...", pinterest: "..." };
const PLACE_ID = "ChIJ52M_DF3vNToRrOzyq71-YOg";
```

The logo is embedded in the file as a data URI, so the page is self-contained and
works offline — no external image to break.

## Publishing

Settings → Pages → Branch `main`, folder `/ (root)`. It then goes live at:

```
https://chakravarthiperumalla.github.io/raosvandana/
```

The page is marked `noindex` so it stays out of search results while it's a demo.
