# Opportunity Hub — first prototype

This is a beginner-friendly, mobile-first web app prototype.

## What works now
- Browse sample opportunity categories (jobs, freelance, surveys, learning, affiliate).
- Search and filter listings.
- Save listings on the current device.
- Submit an opportunity for local review.
- Demo admin page to inspect and add submitted listings to the local directory.
- Basic installable PWA setup.

## Important limitations
This is a front-end prototype, not a production marketplace.
- Listings, saved items and submissions are stored only in the current browser using localStorage.
- They do not sync between devices or users.
- There is no real login, cloud database, secure admin account, payment processing, automated verification, or push notifications.
- Demo listings are examples, not live vacancies. Replace them with verified opportunities and official links before publishing.
- The demo admin page is not protected. Do not enter private or payment information.

## Preview on your phone
1. Extract the ZIP.
2. Open `index.html` in a browser to test the basic interface.
3. For the installable PWA/service worker to work, deploy it to an HTTPS host (for example, a free static hosting tier).

## Free deployment outline (GitHub + Cloudflare Pages)
1. Create a GitHub account at https://github.com/ if you do not already have one.
2. Create a new repository named `opportunity-hub`.
3. Upload `index.html`, `manifest.webmanifest`, and `service-worker.js` to the repository root.
4. In Cloudflare, open Workers & Pages, create a Pages project, and connect the GitHub repository.
5. Use the static site / no build command setup. Set the output directory to `/` or the repository root as prompted by the current Cloudflare setup.
6. Deploy, then open the HTTPS URL on your phone.
7. In your mobile browser menu, choose “Add to Home screen” or “Install app” if available.

## Next development stage
Before accepting real public submissions, connect a hosted database and authentication (for example, Supabase). Add role-based admin access and server-side validation. Add payment processing only after the business model, legal terms, refunds, privacy policy and provider approval are in place.
