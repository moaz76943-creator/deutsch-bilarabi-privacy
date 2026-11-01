# deutsch-bilarabi-privacy

Public privacy policy for the Deutsch بالعربي Android app (`com.deutschbilarabi.app`).

## Google Play compliance

Google Play requires a **publicly accessible, non-geofenced HTML privacy policy URL** (not a PDF or editable doc) that is linked in:
- Play Console → App content → Privacy policy
- Inside the app (e.g. Settings / About screen)

The policy is in `privacy.html` (last updated 2026-11-01). It declares **no data collection/sharing** for the optional on-device `RECORD_AUDIO` pronunciation feature, matching the Data Safety form recommendation of "None". A dedicated **Your Rights and Data Deletion** section documents the local-only deletion path (uninstall) required by Google Play Data safety.

An `index.html` redirect has been added so both the root URL and `/privacy.html` resolve cleanly once GitHub Pages is enabled.

## Enable the stable public URL (REQUIRED — current risk of rejection)

**Action needed now:** The URL currently returns 404 because Pages is not enabled.

1. In this repository: **Settings → Pages**
2. Source: Deploy from branch `main` / `/ (root)`
3. Save. GitHub will publish to:
   - `https://moaz76943-creator.github.io/deutsch-bilarabi-privacy/` (redirects to privacy.html)
   - `https://moaz76943-creator.github.io/deutsch-bilarabi-privacy/privacy.html`
4. Verify the URL loads in a browser (no login required, works without JavaScript).
5. Paste the preferred URL into Play Console → App content → Privacy policy and confirm it is linked from the in-app Settings/About screen.

Until Pages is enabled the URL returns 404 and the app risks rejection during review or Data safety validation. Once live, the policy is ready for production release.

## Contents
- `privacy.html` — full policy covering permissions, Data Safety, integrity, target SDK, children’s privacy, user rights/data deletion, and contact.
- `index.html` — root redirect for cleaner URL.

## Latest compliance improvement (this run)
Updated README to flag the non-live privacy policy URL as the primary remaining rejection risk and provided step-by-step enablement instructions. All other areas (target SDK 36, minimal permissions with on-device microphone only, release signing enforcement, Play Integrity, clear deletion path) are already compliant.
