# Tablesand site

Static marketing site for Tablesand LLC, deployed to `tablesand.com` via a Cloudflare Worker (`wrangler.jsonc`). Plain HTML/CSS, no build step.

- `index.html` - studio homepage (inline styles, self-contained).
- `auditly/` - the Auditly product site: `index.html` (inline styles) plus legal/support pages (`privacy.html`, `terms.html`, `support.html`, `health-disclaimer.html`, `consumer-health-data.html`) that share `/styles.css`.
- Root assets: `auditly-icon.png`, `appstore-badge.svg`, `favicon-96.png`, `apple-touch-icon.png`.
- `auditly/img/` - app screenshots (`iphone-*.png`, `ipad-*.png`). Use root-relative paths (`/auditly/img/...`), not absolute `https://tablesand.com/...` URLs.

## Writing style

Never use en dashes (–) or em dashes (—) in copy or prose. Use a single hyphen (-) instead. Long dashes read as AI-generated. The only exception is numeric or date ranges, where an en dash is acceptable (e.g. `2024-2025`, `9-5`). When in doubt, rewrite the sentence rather than reaching for a dash.
