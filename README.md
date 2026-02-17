# SortedPDF Marketing Website

Marketing and legal pages for [SortedPDF](https://sortedpdf.com) — an AI-powered mobile app that auto-fills PDF forms and scans receipts.

## Tech Stack

- **Framework:** [Astro](https://astro.build) (static site generator)
- **Styling:** [Tailwind CSS v4](https://tailwindcss.com)
- **Icons:** [Lucide](https://lucide.dev) via @lucide/astro
- **Fonts:** Sora (headings) + DM Sans (body) from Google Fonts
- **Hosting:** [Cloudflare Pages](https://pages.cloudflare.com)

## Local Development

```bash
# Install dependencies
npm install

# Start dev server (http://localhost:4321)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deployment (Cloudflare Pages)

**Build settings:**
- Build command: `npm run build`
- Build output directory: `dist/`
- Node.js version: 18+

**Setup:**
1. Connect this repo to Cloudflare Pages
2. Set build command: `npm run build`
3. Set output directory: `dist`
4. Deploy

Pushes to `main` will auto-deploy.

## Project Structure

```
src/
├── layouts/BaseLayout.astro    — HTML shell, meta tags, fonts, theme
├── pages/
│   ├── index.astro             — Homepage (marketing landing)
│   ├── pricing.astro           — Detailed pricing page
│   ├── privacy.astro           — Privacy Policy
│   └── terms.astro             — Terms & Conditions
├── components/                 — Reusable UI components
└── styles/global.css           — Tailwind imports + brand tokens
public/
├── favicon.svg
├── _headers                    — Cloudflare security headers
└── robots.txt
```

## Related Repositories

- **Mobile App:** [fishhead1982/Filla](https://github.com/fishhead1982/Filla) (Flutter, iOS & Android)
- **Backend Proxy:** In the mobile app repo under `backend/` (Dart Shelf, deployed on Railway)
