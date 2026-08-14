# chapter-dash-landing

Legal pages for the Chapter Dash app, hosted via GitHub Pages for use in the
Google Play Console and App Store submission forms.

## Pages

- `privacy.html` — Privacy Policy (GDPR + CCPA sections, data collected, account deletion instructions)
- `terms.html` — Terms of Use (freemium subscription, user-generated content/reviews, uptime/liability limits)
- `style.css` — shared stylesheet for both pages

## Hosting via GitHub Pages

1. Push this repo to GitHub (already at `origin` → `phoenixVS/chapter-dash-landing`).
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`.
4. Choose branch `main`, folder `/ (root)`, then **Save**.
5. After a minute or two, the pages will be live at:
   - `https://phoenixvs.github.io/chapter-dash-landing/privacy.html`
   - `https://phoenixvs.github.io/chapter-dash-landing/terms.html`

Paste those URLs into Google Play Console's Privacy Policy field and App Store
Connect's App Privacy / support links.

## Before submitting

- [ ] Fill in the governing-law jurisdiction placeholder in `terms.html` (§14).
- [ ] Update the third-party services note in `privacy.html` (§4) if you add
      analytics, crash reporting, or billing SDKs (e.g., Firebase, RevenueCat).
- [ ] Add in-app "Privacy Policy" / "Terms of Service" links in the iOS and
      Android apps pointing at the URLs above (SFSafariViewController / Custom
      Tabs), per Apple and Google's in-app disclosure requirements.
