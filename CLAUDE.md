# Tablesand site

Static marketing site for Tablesand LLC, deployed to `tablesand.com` via a Cloudflare Worker (`wrangler.jsonc`). Plain HTML/CSS, no build step.

Every page is self-contained: one inline `<style>` block per file, no shared stylesheet.

- `index.html` - studio homepage.
- `auditly.html` - the Auditly product page, served at `/auditly`.
- `auditly/` - legal and support pages (`privacy.html`, `terms.html`, `support.html`, `health-disclaimer.html`, `consumer-health-data.html`).
- Root assets: `auditly-icon.png`, `appstore-badge.svg`, `favicon-96.png`, `apple-touch-icon.png`.
- `auditly/img/` - app screenshots (`iphone-*.png`, `ipad-*.png`). Use root-relative paths (`/auditly/img/...`), not absolute `https://tablesand.com/...` URLs.

## Screenshots

Site shots are downscaled copies of the App Store captures in the Auditly repo
(`Auditly/marketing/app-store/screenshots/`). Take the **unframed** directories -
the device bezel is drawn in CSS here - and resize with `sips --resampleWidth`:
`iphone-6.9_1320x2868/*` to 700px wide, `ipad-13_2064x2752/*` to 1300px. Filenames
differ between the two repos (e.g. `05-my-stack.png` becomes `iphone-stack.png`),
so confirm each shot by eye rather than by name.

## Writing style

Never use en dashes (–) or em dashes (—) in copy or prose. Use a single hyphen (-) instead. Long dashes read as AI-generated. The only exception is numeric or date ranges, where an en dash is acceptable (e.g. `2024-2025`, `9-5`). When in doubt, rewrite the sentence rather than reaching for a dash.
