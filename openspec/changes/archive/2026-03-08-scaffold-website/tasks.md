## 1. Project Setup
- [x] 1.1 Initialize Astro project (`npm create astro@latest`)
- [x] 1.2 Configure `astro.config.mjs` — static output, `site` set to `https://groundspeed-labs.github.io`
- [x] 1.3 Add GitHub Actions workflow for deploying to GitHub Pages

## 2. Layout and Styles
- [x] 2.1 Create `src/layouts/BaseLayout.astro` — shared head, nav, footer
- [x] 2.2 Create `src/styles/global.css` — base reset, typography (system font stack), responsive breakpoints
- [x] 2.3 Create `src/layouts/MarkdownLayout.astro` — layout for Markdown content pages (privacy, terms)

## 3. Company Landing Page
- [x] 3.1 Create `src/pages/index.astro` — Groundspeed Labs name, tagline, app listing with link to `/keepvalid/`

## 4. KeepValid App Page
- [x] 4.1 Create `src/pages/keepvalid/index.astro` — app name, description, feature highlights
- [x] 4.2 Add Google Play Store badge (placeholder "Coming soon" until Play Store URL is available)
- [x] 4.3 Add link to privacy policy

## 5. KeepValid Privacy Policy
- [x] 5.1 Create `src/pages/keepvalid/privacy.md` — full privacy policy in Markdown with frontmatter
- [x] 5.2 Cover all required sections: data collected, storage, third-party services (Supabase, FCM, ML Kit), retention, deletion, contact info
- [x] 5.3 Add effective date and last-updated date

## 6. Validation
- [x] 6.1 Build locally (`npm run build`) and verify output
- [ ] 6.2 Verify all pages render on mobile and desktop
- [x] 6.3 Verify zero external requests in built output
- [x] 6.4 Push to GitHub and verify GitHub Pages deployment works
