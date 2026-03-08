## ADDED Requirements

### Requirement: Company Landing Page

The site SHALL serve a landing page at `/` that presents Groundspeed Labs as a company, lists published apps, and links to each app's sub-site.

#### Scenario: Visitor loads the homepage
- **WHEN** a visitor navigates to `groundspeed-labs.github.io`
- **THEN** they see the Groundspeed Labs name, a brief tagline, and a link to the KeepValid app page

### Requirement: App Landing Page

Each app SHALL have a landing page at `/<app-name>/` with the app name, a short description, key features, and a download link (Play Store badge).

#### Scenario: Visitor loads KeepValid page
- **WHEN** a visitor navigates to `/keepvalid/`
- **THEN** they see the KeepValid name, description, feature highlights, and a Google Play Store download badge

#### Scenario: Play Store link works
- **WHEN** a visitor clicks the Play Store badge
- **THEN** they are directed to the KeepValid listing on Google Play

### Requirement: App Privacy Policy

Each app SHALL have a privacy policy page at `/<app-name>/privacy/` that satisfies Google Play Store requirements.

#### Scenario: Privacy policy content
- **WHEN** a visitor navigates to `/keepvalid/privacy/`
- **THEN** they see a privacy policy covering: data collected, how it is stored, third-party services used, data retention and deletion, and contact information

#### Scenario: Google Play compliance
- **WHEN** the privacy policy URL is submitted to Google Play Console
- **THEN** it is accepted as a valid privacy policy URL

### Requirement: Mobile-Responsive Design

All pages SHALL be mobile-responsive and render correctly on screens from 320px to 1440px wide.

#### Scenario: Mobile visitor
- **WHEN** a visitor loads any page on a mobile device
- **THEN** the content is readable without horizontal scrolling and interactive elements are tap-friendly

### Requirement: No External Dependencies

The site SHALL load without any external requests (no CDNs, no external fonts, no analytics, no tracking scripts).

#### Scenario: Fully self-contained
- **WHEN** a page is loaded
- **THEN** all resources (CSS, images) are served from the same domain with zero third-party requests

### Requirement: Clean URLs

All pages SHALL be accessible via directory-based clean URLs without `.html` extensions.

#### Scenario: URL structure
- **WHEN** a visitor navigates to `/keepvalid/privacy/`
- **THEN** the page loads correctly via GitHub Pages serving `keepvalid/privacy/index.html`
