# Project Context

## Purpose

Public website for **Groundspeed Labs** — a small app studio. Hosts the company landing page and per-app sub-sites (landing pages, privacy policies, terms of service). The primary driver is the Google Play Store submission for **KeepValid**, which requires a publicly accessible privacy policy URL.

**Core Goals:**
- Present Groundspeed Labs as a company
- Host app-specific pages under `/<app-name>/` paths
- Provide privacy policy and legal pages required by app stores
- Keep it fast, simple, and dependency-free

## Tech Stack

- **Astro** — static site generator, outputs zero JS by default, component-based templating
- **HTML/CSS** — Astro components are HTML-like `.astro` files with scoped CSS
- **Markdown** — content pages (privacy policy, terms) written in Markdown
- **GitHub Pages** — static hosting, deployed from GitHub Actions
- **Domain**: `groundspeed-labs.github.io` (custom domain may be added later)

## Project Conventions

### Code Style

- Plain HTML5 and CSS3
- Semantic HTML elements (`<header>`, `<main>`, `<footer>`, `<section>`, `<nav>`)
- CSS in a shared stylesheet where possible; inline styles only when unavoidable
- Mobile-first responsive design
- No JavaScript unless strictly necessary for functionality (not aesthetics)

### Architecture Patterns

- **Astro layouts** — shared `BaseLayout.astro` for consistent page structure (head, nav, footer)
- **Astro pages** — file-based routing under `src/pages/`
  - `src/pages/index.astro` → `/`
  - `src/pages/keepvalid/index.astro` → `/keepvalid/`
  - `src/pages/keepvalid/privacy.md` → `/keepvalid/privacy/`
- **Per-app sub-sites** — each app gets its own directory under `src/pages/`
- **Markdown for content** — legal/content pages use Markdown with frontmatter and layout references
- **Shared assets** — common styles in `src/styles/`, images in `public/`

### Content Tone

Direct, no-nonsense. No marketing fluff. Clear, honest, professional. Matches the Groundspeed Labs brand.

### Testing Strategy

- Manual: verify pages render correctly on mobile and desktop
- Validate HTML with W3C validator
- Check all links work
- Lighthouse audit for performance and accessibility

### Git Workflow

- Work directly on `main` (simple static site, no need for feature branches unless changes are large)
- Conventional commits: `feat:`, `fix:`, `docs:`, `chore:`

## Domain Context

### Apps

**KeepValid** — document expiration reminder app (Flutter/Android). Tracks personal documents (IDs, passports, licenses) and sends notifications before they expire. Privacy-first: on-device OCR, minimal data storage.

### Company

**Groundspeed Labs** — small app studio. The name is an aviation term (groundspeed = actual speed over terrain). Brand values: practical, no-nonsense tools that do one thing well.

## Important Constraints

- **No cookies, no analytics, no tracking** — aligns with the privacy-first brand
- **No runtime JavaScript** — Astro outputs static HTML/CSS, no client-side JS unless explicitly opted in
- **No external dependencies at runtime** — no CDNs, no Google Fonts, no third-party scripts
- **Must be mobile-responsive** — most visitors arrive from Play Store links on their phones
- **Privacy policy must satisfy Google Play requirements** — covers data collection, storage, third-party services, retention, deletion, and contact information

## External Dependencies

- **GitHub Pages** — hosting (served from `main` branch)
- No other external services
