# AK SELLER PWA — starter demo

This is a mobile-friendly Progressive Web App (PWA) starter. It uses original branding and demo product data. It is not affiliated with or endorsed by Flipkart.

## Files
- `index.html`: storefront, search, categories, product cards and demo Buy Now behavior.
- `manifest.json`: PWA metadata.
- `sw.js`: basic offline caching service worker.
- `icons/`: install icons.

## Important before publishing
1. Replace demo product names, photos, and prices with accurate data you have permission to use.
2. Add only valid, authorized affiliate URLs to each product's `url` property in `index.html`.
3. Confirm current affiliate-program eligibility, branding, link-tracking, disclosures, and API/data-use rules with the affiliate provider.
4. Do not scrape retailer pages or copy retailer branding.
5. Buy Now opens a link only if the product has a valid HTTPS URL; otherwise it shows a demo notice.
6. Host on HTTPS for PWA installation/service-worker support.

## Edit affiliate links
Find the `const products = [...]` array in `index.html`. For a product, change `url:""` to the full authorized HTTPS affiliate link, e.g. `url:"https://example.com/your-authorized-tracking-link"`. This is only a placeholder format; do not use a made-up link.

## Test on your phone
PWA install and service worker require an HTTPS host (or localhost). Opening `index.html` directly from a file manager will show the page but will not enable all PWA features.

## Free publishing outline
- Create a GitHub account if eligible, create a new repository, upload the contents of this folder, then enable GitHub Pages in repository Settings → Pages.
- Or use another HTTPS static host such as Netlify or Vercel.
- Open the published HTTPS URL in Chrome on Android → menu (⋮) → Add to Home screen / Install app.
- Keep in mind provider account eligibility and publishing service terms.
