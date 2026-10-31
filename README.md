# deutsch-bilarabi-privacy

Public privacy policy for the Deutsch بالعربي Android app (`com.deutschbilarabi.app`).

## Google Play compliance

Google Play requires a **publicly accessible, non-geofenced HTML privacy policy URL** (not a PDF or editable doc) that is linked in:
- Play Console → App content → Privacy policy
- Inside the app (e.g. Settings / About screen)

The policy is in `privacy.html` (last updated 2026-10-31). It declares **no data collection/sharing** for the optional on-device `RECORD_AUDIO` pronunciation feature, matching the Data Safety form recommendation of "None". A dedicated **Your Rights and Data Deletion** section was added to clearly document the local-only deletion path (uninstall) required by Google Play Data safety.

An `index.html` redirect has been added so both the root URL and `/privacy.html` resolve cleanly once GitHub Pages is enabled.

## Enable the stable public URL (required)

1. In this repository: **Settings → Pages**
2. Source: Deploy from branch `main` / `/ (root)`
3. Save. GitHub will publish to:
   - `https://moaz76943-creator.github.io/deutsch-bilarabi-privacy/` (redirects to privacy.html)
   - `https://moaz76943-creator.github.io/deutsch-bilarabi-privacy/privacy.html`
4. Verify the URL loads in a browser (no login required).
5. Paste the preferred URL into Play Console and link it from the app.

Until Pages is enabled the URL returns 404. Once live, the policy is ready for production release.

## Contents
- `privacy.html` — full policy covering permissions, Data Safety, integrity, target SDK, children’s privacy, user rights/data deletion, and contact.
- `index.html` — root redirect for cleaner URL.

## Latest compliance improvement (this run)
Strengthened the privacy policy with an explicit data deletion and user rights section to better align with Google Play Data safety requirements. Target SDK 36, minimal permissions, Play App Signing, and Play Integrity declarations remain in place.
