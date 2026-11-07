# deutsch-bilarabi-privacy

Public privacy policy for the Deutsch بالعربي Android app (`com.deutschbilarabi.app`).

## Google Play compliance

Google Play requires a **publicly accessible, non-geofenced HTML privacy policy URL** (not a PDF or editable doc) that is linked in:
- Play Console → App content → Privacy policy
- Inside the app (e.g. Settings / About screen)

The policy is in `privacy.html` (last updated 2026-11-01). It declares **no data collection/sharing** for the optional on-device `RECORD_AUDIO` pronunciation feature, matching the Data Safety form recommendation of "None". A dedicated **Your Rights and Data Deletion** section documents the local-only deletion path (uninstall) required by Google Play Data safety.

An `index.html` redirect has been added so both the root URL and `/privacy.html` resolve cleanly once GitHub Pages is enabled.

## Enable the stable public URL (REQUIRED — current risk of rejection)

**CRITICAL: Action required before Play Console submission.** As of November 7, 2026, the URL still returns 404 because GitHub Pages is not enabled for this repository. This remains the primary remaining rejection risk.

1. In this repository: **Settings → Pages**
2. Source: Deploy from branch `main` / `/ (root)`
3. Save. GitHub will publish to:
   - `https://moaz76943-creator.github.io/deutsch-bilarabi-privacy/` (redirects to privacy.html)
   - `https://moaz76943-creator.github.io/deutsch-bilarabi-privacy/privacy.html`
4. Verify the URL loads in a browser (no login required, works without JavaScript, not a PDF).
5. Paste the preferred URL into Play Console → App content → Privacy policy and confirm it is linked from the in-app Settings/About screen (constant `kPrivacyPolicyUrl` in the app).

Until Pages is enabled the URL returns 404 and the app risks rejection during review or Data safety validation. Once live, the policy is ready for production release.

## Current compliance status (November 7, 2026)

- **Target SDK**: 36 (Android 16) — meets August 31, 2026 requirement for new apps/updates. Extension window closed Nov 1.
- **Permissions**: Minimal; only optional RECORD_AUDIO (on-device only). Storage/media permissions explicitly removed. No restricted permissions without justification.
- **Privacy policy**: Content complete and accurate; **URL not yet live** (Pages disabled — verified 404).
- **Data Safety**: Matches policy (no collection/sharing). Local deletion via uninstall documented.
- **Signing**: Release signing enforced; Play App Signing expected.
- **Integrity**: Play Integrity API integrated (client + dependency).
- **Other**: allowBackup=false, cleartext disabled, minify/shrink enabled, prominent disclosure for mic, FLAG_SECURE in release.

## Contents
- `privacy.html` — full policy covering permissions, Data Safety, integrity, target SDK, children’s privacy, user rights/data deletion, and contact.
- `index.html` — root redirect for cleaner URL.

## Latest compliance improvement (this run — 2026-11-07)
Updated README date and confirmed the privacy policy public URL continues to return 404 (GitHub Pages still disabled). This is the sole major remaining rejection risk for production release. All other areas (target SDK 36, permissions, signing, integrity protection, Data Safety alignment, security configs) remain compliant. Enable GitHub Pages immediately to clear the final blocker.
