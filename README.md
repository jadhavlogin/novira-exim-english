# Novira Exim — English Book Landing Page

Static landing page for the book **Import-Export Business Complete Guide — All the Way to Your First Export Shipment** (English, printed hard copy).

## Files
- `index.html` — design 1: dark navy + gold (matches the ad creatives)
- `v2.html` — design 2: light editorial, table-of-contents + shipping-label order card

Each page is self-contained (HTML + CSS + a little JS, no build step). Pick one and rename it to `index.html` when deploying.
- `assets/` — banner creatives and the cropped book cover

## Before going live
Open the page you use, scroll to the `CONFIG` block near the bottom and fill in:

| Key        | Example                           | Effect |
|------------|-----------------------------------|--------|
| `price`    | `"₹499"`                          | Shows price tag on cover, order card and mobile bar |
| `mrp`      | `"₹999"`                          | Struck-through original price |
| `saveText` | `"50% OFF"`                       | Green discount badge |
| `buyUrl`   | Razorpay / Instamojo payment link | All "Buy / Order" buttons go here |
| `whatsapp` | `"919876543210"`                  | WhatsApp order button (used for Buy buttons if `buyUrl` is empty) |
| `email`, `phone` | —                           | Shown in footer |
| `testimonials` (index.html) | `{ quote, name, place, rating }` | Real reader reviews in the "Readers" section |

Empty values are hidden automatically.

## Deploy
Any static host works: Netlify / Vercel / GitHub Pages / Hostinger — upload `index.html` and the `assets/` folder.
