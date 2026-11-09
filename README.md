# ChoreDeal information

Static HTML pages for ChoreDeal. **Updated policy/support copy prepared November 9, 2026; local source has an effective date and no draft/indexing notices. These changes have not been published. Live GitHub Pages still serves the prior draft, verified by direct HTTP on November 9.**

- [Privacy policy](docs/privacy.html)
- [Support](docs/support.html)

Publisher: **Daniel Mancilla**, an individual. Contact: **support@fussionlabs.com**. Launch model: one upfront App Store purchase, all features included, no subscriptions, ads or feature purchases. Apple Family Sharing configuration and purchase testing remain release tasks.

## Remaining launch checks

- [x] Confirm publisher and contact with the owner.
- [x] Confirm deletion of resolved support emails/screenshots within 90 days and use of Apple-provided crash reports and aggregated analytics.
- [x] Draft policy/support copy against the app's privacy and deletion documentation.
- [ ] Review draft wording with the owner, including family/minor use and the intended countries of availability. Do not infer legal compliance or a minimum-age policy from the App Store rating.
- [ ] Verify removal instructions using disposable households on physical devices with distinct Apple Accounts. Simulator tests do not prove actual CloudKit deletion or revocation.
- [ ] Establish the mailbox cleanup routine needed to meet the 90-day commitment, including attachments and downloaded copies. The owner confirmed on November 9 that Apple reports/analytics are viewed only in Apple tools; no downloaded copies are retained.
- [x] Select GitHub Pages and prepare static HTML in `/docs`.
- [x] Publish on GitHub Pages and verify home/privacy/support URLs return HTTP 200 (November 9, 2026).
- [ ] Repository visibility and exact Pages source settings have not been independently inspected.
- [x] Prepare revised local copy with an effective date and remove draft/noindex notices (November 9).
- [ ] Complete publication review and publish the updated pages; verify live content matches source. The effective date in prepared source must be adjusted if publication occurs on a later date.
- [x] Add policy links in the app (About and onboarding), plus Support in About; app validation is tracked in the app repository.
- [ ] Confirm final URLs and disclosures saved in App Store Connect.
- [ ] Finalize App Store privacy answers and reassess manifests against actual practices. Do not treat the source audit's empty collected-data declarations as final answers. Optional support disclosures require all applicable Apple criteria.

The release record remains in the ChoreDeal app repository at `docs/trackers/Initial_Release.md` (R03). Drafts were based on that repository's `docs/architecture/Privacy.md` and `docs/architecture/Deletion.md`. No app runtime changes, portal submission or device validation were performed while preparing these documents.

## Reference material

- [Apple App Privacy Details](https://developer.apple.com/app-store/app-privacy-details/)
- [Apple privacy review guidelines](https://developer.apple.com/app-store/review/guidelines/#privacy)
- [Apple app analytics](https://developer.apple.com/app-store/measuring-app-performance/)
- [GitHub Pages and visitor logging](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)

When changing these documents, keep the app release tracker current and distinguish drafted, published and verified work. Never put private household data or support correspondence in this repository.

## Site structure and editing

- `docs/index.html`: introduction and links.
- `docs/privacy.html`: canonical privacy policy.
- `docs/support.html`: canonical support page.
- `docs/styles.css`: shared responsive styles; system fonts, no external assets or scripts.
- `docs/.nojekyll`: serve the static files without Jekyll processing.

Edit HTML directly. The original Markdown drafts were converted without changing policy/support wording and removed to avoid divergent copies. Keep the prepared changes local until the outstanding publication review/verification checks above are complete. Do not describe local changes as live. Relative links work both locally and under the GitHub project URL.

## GitHub Pages setup

After the approved pages are committed and pushed to `main`, open the repository's **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, branch **main**, folder **/docs**, then **Save**. Confirm the deployment succeeds and check all pages before using the URLs in the app or App Store Connect.

Published addresses (HTTP 200 verified November 9, 2026):

- Home: `https://dm0275.github.io/choredeal-info/`
- Privacy: `https://dm0275.github.io/choredeal-info/privacy.html`
- Support: `https://dm0275.github.io/choredeal-info/support.html`

The `/docs` source folder does not appear in the website URL. No domain, backend, package installation or build step is required for this layout.

For a local preview, run `python3 -m http.server 8765 --bind 127.0.0.1 --directory docs` from the repository and visit `http://127.0.0.1:8765/`. Stop the preview with Control-C.

## November 9 policy refresh

Prepared updated effective policy/support copy, recorded Apple-tools-only diagnostics, matched the current Invite & manage sharing label, and removed obsolete draft banners from local source. No change to confirmed publisher, support contact, 90-day resolved-support retention, household sharing/storage, or removal limitations. App links use the canonical GitHub Pages URLs above. Publication and live verification of this revision remain pending; physical-device removal and portal-disclosure gates are not closed by copy edits.
