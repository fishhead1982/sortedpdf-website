## Status

Astro + Tailwind v4 marketing and legal site for SortedPDF deployed to Cloudflare Pages, dormant since the App Store compliance push in February 2026.

## Remaining

- None

## Done

- Initial SortedPDF marketing website (2026-02-17)
- `wrangler.jsonc` for Cloudflare Pages deployment
- Fix for CSS not loading in production build
- Fix for billing toggle thumb overflowing on annual
- Legal entity updated to "MacPherson Ventures trading as SortedPDF", then corrected to "MacPherson Ventures Pty Ltd"
- Data deletion page added for App Store compliance
- Data deletion FAQ entry added with link to the deletion page

## Notes

**Tech stack:** Astro (static site generator), Tailwind CSS v4, Lucide icons via `@lucide/astro`, Sora (headings) and DM Sans (body) from Google Fonts, Cloudflare Pages hosting. Pushes to `main` auto-deploy.

**Pages:** `index.astro` (homepage), `pricing.astro`, `privacy.astro`, `terms.astro`, plus the App Store compliance data deletion page.

**Local dev:** `npm install`, `npm run dev` (http://localhost:4321), `npm run build`, `npm run preview`. Build output is `dist/`, Node 18+.

**Related repos:** fishhead1982/Filla (Flutter mobile app, iOS & Android) and the backend proxy that lives inside that repo under `backend/` (Dart Shelf, deployed on Railway).
