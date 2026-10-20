# CozyPlace – Cozy Date landing page

A single static page: `index.html` (HTML, CSS and JS in one file) plus `assets/`.
Open `index.html` in a browser to preview. There's no build step.

## Interactions
- **Locations**: clicking a location card opens that outlet's pop-up. The tabs inside switch outlets without closing it. Close with the Close button or Esc.
  Deep links work, e.g. `index.html#location-paya-lebar`.
- **FAQ**: an accordion. Only one answer is open at a time.
- **Booking bar**: a sticky "Find Your CozyPlace" bar appears after you scroll past the hero.
- Every "Book" button goes to `https://cozyplace.sg/booking-detail`.

## Editing content
All editable data is at the top of the `<script>` block in `index.html`:
- `BOOKING_URL`: where the Book buttons go
- `LOCATIONS`: name, address, MRT line, card image and room `photos` for each outlet
- `FAQS`: questions and answers (a blank line starts a new paragraph)

Room photos: every outlet currently uses the Jalan Besar set (`assets/pop1–6.webp`).
To give an outlet its own photos, add the images to `assets/` and change that outlet's `photos` list.

## Font
Headings use **Sunliner Revival**, served from `assets/fonts/`:
- `SunlinerRevival-Regular.woff2` (51 KB, loaded first by modern browsers)
- `SunlinerRevival-Regular.otf` (backup)

Make sure you're licensed to use Sunliner Revival on the web before publishing.
Body text uses Poppins and labels use Headland One, both from Google Fonts.
