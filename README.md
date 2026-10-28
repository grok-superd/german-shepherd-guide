# Shepherd Guide: German Shepherd Dog information site

Static, dependency-free site (plain HTML + one CSS file) published with GitHub Pages from the `main` branch root.

Live: https://grok-superd.github.io/german-shepherd-guide/

## Structure
- `*.html`: pages (Home, Breed Overview, History, Care, Training, Health, Puppies, FAQ, About, Contact, Privacy, Terms, 404)
- `assets/style.css`: all styles (system fonts, no JS)
- `sitemap.xml`, `robots.txt`, `ads.txt` (placeholder), `favicon.svg`, `assets/og-image.png`

## AdSense placeholders
- Each page `<head>` has a commented-out AdSense auto-ads script with `ca-pub-XXXXXXXXXXXXXXXX`.
- Manual ad slots are `<aside class="ad-slot">` blocks, each preceded by an `AD SLOT` HTML comment showing where to paste the ad unit code. Their min-heights reserve space to avoid layout shift.
- `ads.txt` must live at the domain root, so it only becomes effective with a custom domain.

## Before applying for AdSense
1. Point a custom domain at this repo (GitHub Pages > Custom domain) and update `BASE` URLs (canonical, OG, sitemap, robots).
2. Replace the contact email placeholder in `contact.html`.
3. Verify the domain in Google Search Console and submit `sitemap.xml`.
