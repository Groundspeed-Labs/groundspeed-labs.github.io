## 1. Project Setup
- [ ] 1.1 Initialize Astro project (`npm create astro@latest`)
- [ ] 1.2 Configure `astro.config.mjs` — static output, `site` set to `https://groundspeed-labs.github.io`
- [ ] 1.3 Add GitHub Actions workflow for deploying to GitHub Pages

## 2. Layout and Styles
- [ ] 2.1 Create `src/layouts/BaseLayout.astro` — shared head, nav, footer
- [ ] 2.2 Create `src/styles/global.css` — base reset, typography (system font stack), responsive breakpoints
- [ ] 2.3 Create `src/layouts/MarkdownLayout.astro` — layout for Markdown content pages (privacy, terms)

## 3. Company Landing Page
- [ ] 3.1 Create `src/pages/index.astro` — Groundspeed Labs name, tagline, app listing with link to `/keepvalid/`

## 4. KeepValid App Page
- [ ] 4.1 Create `src/pages/keepvalid/index.astro` — app name, description, feature highlights
- [ ] 4.2 Add Google Play Store badge (local asset in `public/`, links to Play Store listing)
- [ ] 4.3 Add link to privacy policy

## 5. KeepValid Privacy Policy
- [ ] 5.1 Create `src/pages/keepvalid/privacy.md` — full privacy policy in Markdown with frontmatter
- [ ] 5.2 Cover all required sections: data collected, storage, third-party services (Supabase, FCM, ML Kit), retention, deletion, contact info
- [ ] 5.3 Add effective date and last-updated date

## 6. Validation
- [ ] 6.1 Build locally (`npm run build`) and verify output
- [ ] 6.2 Verify all pages render on mobile and desktop
- [ ] 6.3 Verify zero external requests in built output
- [ ] 6.4 Push to GitHub and verify GitHub Pages deployment works
