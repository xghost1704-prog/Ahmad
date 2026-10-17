# The Matrix Lounge Gaming Zone Website

A responsive multi-page static website demo with interactive navigation, game search/filter, gallery lightbox, FAQ accordion, enquiry form preparation, editable business configuration, and local SEO foundations.

## Pages
- `index.html` — Home
- `gaming.html` — Gaming & Consoles
- `games.html` — Searchable Games Library
- `rates.html` — Rates & Packages
- `gallery.html` — Gallery with lightbox
- `about.html` — About
- `contact.html` — Contact & Location and enquiry form
- `faq.html` — FAQs
- `privacy.html` — Privacy policy starter template

## Run locally
This is a static site and does not require a build step. For the most reliable local testing, run a local web server from this directory:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

You can also deploy the folder to any static hosting provider that serves HTML, CSS and JavaScript. No deployment has been performed by this package.

## Edit business details
Edit `js/config.js`. This is the central source of truth for:
- Name, phone, address, Maps URLs, opening hours and review link.
- Game categories and game descriptions.
- Pricing data.
- FAQs and gallery imagery.
- Email and WhatsApp integration configuration.

**Before production:** verify the phone number, complete street address, operating hours, consoles, current games, prices, review link, and the business owner's approved logo/photos. The phone/address shown in the demo are sourced from public listing information and require confirmation. Do not present the stock gallery images as actual venue photos.

## Contact form limitation
The form validates the consent checkbox and prepares a readable enquiry. If `email` is configured in `js/config.js`, it opens the visitor's email application with a prefilled message; it cannot confirm delivery. If no email is configured, the form displays a copyable message. This static demo does not send data to a server and does not store submissions.

For a production form, connect a secure backend or trusted form service. Add server-side validation, spam protection, rate limiting, data-retention controls and an updated privacy notice. Only configure WhatsApp after confirming the business number is WhatsApp-enabled; the current demo intentionally does not assume that.

## Images and fonts
The demo uses remote Unsplash image URLs and Google Fonts. A network connection is required. Replace illustrative stock imagery with licensed or owner-approved assets before production. Verify asset licensing and image loading in the deployed environment.

## Quality and security notes
- No fake reviews, fabricated ratings, invented prices or claimed statistics are included.
- Opening hours and business details are marked as unverified.
- The Maps link uses the supplied public listing as a fallback.
- The website uses semantic HTML, keyboard-friendly controls and reduced-motion support.
- Privacy policy is a starter template and needs owner/legal review.
- Add a verified production domain before finalizing canonical URLs, sitemap and production structured data.
- Add a backend only when real data submission or owner-managed content is required.

## Production checklist
1. Confirm exact business name, address, phone and opening hours.
2. Confirm current console and game availability.
3. Add verified rates or retain the enquiry-only pricing message.
4. Replace stock images and add approved logo assets.
5. Configure a real form destination and test success/failure states.
6. Verify Maps and review links.
7. Review privacy and consent wording.
8. Test all pages on mobile and desktop.
9. Add production domain, sitemap, robots.txt and valid LocalBusiness structured data using verified details only.
10. Deploy and test HTTPS, links, accessibility and performance.
