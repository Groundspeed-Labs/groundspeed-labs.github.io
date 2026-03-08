# Change: Scaffold Groundspeed Labs website

## Why

Google Play Store requires a publicly accessible privacy policy URL before an app can be published. KeepValid is ready to submit but has no website. The company also needs a minimal public presence.

## What Changes

- Initialize Astro project with static output, GitHub Pages deployment
- Company landing page at `/` — Groundspeed Labs branding, link to KeepValid
- KeepValid app page at `/keepvalid/` — app description, features, Play Store badge
- KeepValid privacy policy at `/keepvalid/privacy/` — Markdown content, satisfies Google Play requirements
- Shared layout component (`BaseLayout.astro`) for consistent page structure
- GitHub Actions workflow for automated deployment to GitHub Pages

## Impact

- Affected specs: new `website` capability
- Affected code: all new files (empty repo)
- Unblocks: Google Play Store submission for KeepValid
