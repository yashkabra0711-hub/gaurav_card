# gaurav_card
Digital business card landing page.
Gaurav Agrawaal — Digital Business Card
A single-page, mobile-first digital business card for the QR code on Gaurav's visiting card.
Structure
```
gaurav-agrawaal-card/
├── index.html          # everything: markup, Tailwind config, styles, JS
├── assets/
│   ├── favicon.svg      # navy "GA" monogram favicon
│   └── headshot.jpg     # profile photo, optimized to 480×480
└── README.md
```
Tech
HTML5 + Tailwind CSS (via CDN, configured with the navy/ivory palette in the `<script>` tag in `<head>`)
Vanilla JS (scroll-reveal via `IntersectionObserver`, clipboard copy with a `document.execCommand` fallback)
No build step, no dependencies to install — open `index.html` directly or deploy as static files
Before you publish
URLs — the `canonical`, `og:url`, `og:image`, `twitter:image`, and the JSON-LD `image` field all assume the final page lives at `https://www.altevius.com/gaurav` with the image at `.../gaurav/assets/headshot.jpg`. Update those if the real hosting path differs, so link previews load the photo correctly.
Host it — any static host works (Vercel, Netlify, GitHub Pages, or a folder on altevius.com). Point the QR code at the final URL.
Notes on the brief
The "Experience" section listed "Associate" in the brief, but the person details name Gaurav as Founder & CEO — the page uses Founder & CEO, Altevius Partners there, since that matches who the card is for. Flag if that was intentional and it should say something else.
Dark mode follows the visitor's system setting automatically (`prefers-color-scheme`) rather than a manual toggle, to keep the interface uncluttered.
WhatsApp and Call both use `+91 99290 23389`, formatted as `tel:+919929023389` and `https://wa.me/919929023389`.
