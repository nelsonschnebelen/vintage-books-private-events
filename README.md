# Vintage Books — Private Dining & Events

Standalone private-events site for Vintage Books Hawaii (Kaimuki, Honolulu).
Static HTML: no build step. Every push to `main` redeploys wherever it's hosted.

## Files
- `index.html` — the whole site (styles and scripts inline)
- `pe-*.jpg` — venue photography
- `vb-logo*.png`, `parchment.jpg` — brand assets

## Updating prices
All estimator numbers live in the `PRICING` object near the bottom of `index.html`
(space minimums, per-guest menu prices, drinks, service charge, GET, deposit).
Displayed prices elsewhere on the page are plain text in the matching sections.

## Inquiries
The proposal form posts to FormSubmit, which emails each request to
sherene@vintagebookshawaii.com. The first submission triggers a one-time
activation email to that address that must be confirmed.

## Tracking
Meta Pixel `825719913590196`: `PageView`, `ViewContent`, `InitiateCheckout`
("Hold this date"), and `Lead` (form submitted).
