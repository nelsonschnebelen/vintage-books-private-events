# Vintage Books — Private Dining & Events

Standalone private-events site for Vintage Books Hawaii (Kaimuki, Honolulu).
Static HTML: no build step. Every push to `main` redeploys wherever it's hosted.

## Files
- `index.html` — the whole site (styles and scripts inline)
- `pe-*.jpg` — venue photography
- `vb-logo*.png`, `parchment.jpg` — brand assets

## Updating prices and menus
Everything editable is near the bottom of `index.html`:
- `MINIMUMS`: food & beverage minimum per space (`buyout`, `lounge`), time of day
  (`day`, `evening`) and day of week. The calendar, quote and space cards all read it.
- `MENUS`: the six family-style and plated menus. The Menus section and the quote's
  menu options are both built from this list.
- `PRICING`: capacities, brunch price, drinks, service charge, GET, deposit.

## Blocking booked dates
Add the date to the `BOOKED_DATES` list in `index.html` (format `"2026-12-12"`).
It shows crossed out on the calendar and can't be selected. Push to `main` and
it goes live.

## Inquiries
The proposal form posts to FormSubmit, which emails each request to
sherene@vintagebookshawaii.com. The first submission triggers a one-time
activation email to that address that must be confirmed.

## Tracking
Meta Pixel `825719913590196`: `PageView`, `ViewContent`, `InitiateCheckout`
("Hold this date"), and `Lead` (form submitted).
