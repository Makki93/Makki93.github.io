# bavarianTechWorks website

Public GitHub Pages home for four independently maintained app websites:

| App | Website | Support | App privacy |
| --- | --- | --- | --- |
| Pawference | https://makki93.github.io/Pawference-Info/ | https://makki93.github.io/Pawference-Info/support.html | https://makki93.github.io/Pawference-Info/app-privacy.html |
| GalleryTidy | https://makki93.github.io/GalleryTidy-Info/ | https://makki93.github.io/GalleryTidy-Info/ | https://makki93.github.io/GalleryTidy-Info/privacy.html |
| WaitASec | https://makki93.github.io/WaitASec-Info/ | https://makki93.github.io/WaitASec-Info/#support | https://makki93.github.io/WaitASec-Info/privacy/ |
| GaudiKistn | https://makki93.github.io/gaudikistn/de/index.html | https://makki93.github.io/gaudikistn/de/support.html | https://makki93.github.io/gaudikistn/de/privacy.html |

Home: https://makki93.github.io/
Contact: bavariantechworks@mailbox.org

## Scope and publishing

This repository contains only static public website files. The application
repositories remain private. GitHub Pages publishes `main` at the repository root;
`.nojekyll` disables Jekyll. There is no JavaScript, tracking, form backend, external
font or package dependency. GaudiKistn bundles its app fonts locally with their
OFL licenses; it has no external font requests.

Edit the site, inspect it at desktop and mobile widths, validate local links and
commit only named files before pushing `main`. Check the Pages deployment and the
public URLs after publishing. Bump the `styles.css` version in all HTML pages
when changing its rules to avoid serving a cached earlier layout.

The common `impressum.html` is linked from each app website. The postal address is
kept on that page only. Website privacy is separate from app privacy. App-specific
texts and release status must be checked with the owners of the app repositories.
Do not turn preparation status into an App Store release or add unapproved beta links.

## Assets

- `assets/pawference.png`: unchanged icon from the Pawference app/site; its
  provenance is documented in the app repository's `docs/APP_ICON.md`.
- `assets/gallerytidy.png`: unchanged shared GalleryTidy iOS/macOS app icon.
- `assets/waitasec.svg`: WaitASec pause-and-wave icon (variant A), selected by the owner on 2026-10-02. The square source is maintained in the private app repository at `docs/brand/appicon-pause-wave.svg`.
- `assets/brand.svg`: simple vector monogram created for this website.
- `gaudikistn/assets/`: unchanged GaudiKistn icon and wordmark, locally bundled
  DM Sans and Cormorant Garamond with licenses, and a clearly labelled generated
  example motif. The motif is not a customer photo or evidence of working app UI.

These app marks identify the owner's apps; they are not stock imagery or permission
to reuse the application assets in third-party products.

## GaudiKistn content

The `gaudikistn/` directory contains eleven static language versions (German,
British English, French, Spanish, Italian, Dutch, Polish, European Portuguese,
Romanian, Swedish and Czech), each with home, support, app privacy and subscription
pages. The default URL redirects to German without JavaScript.

The source content and dependency-free generator are in the private GaudiKistn
repository under `distribution/`; do not copy private review drafts here. Rebuild
and verify from that repository with:

```sh
python3 distribution/build.py --site-root /Users/markus/src/Makki93.github.io
python3 distribution/verify.py --site-root /Users/markus/src/Makki93.github.io
```

The public beta is in preparation. There is no public join link until Apple
approval and the exact build/group settings are verified. The planned subscription
is distinct from beta access. Translations are prepared drafts, not evidence of a
native-speaker or legal review. Inspect desktop and mobile output after regeneration.

## Local preview

```sh
python3 -m http.server 18766 --bind 127.0.0.1 --directory .
```

Public inquiries through GitHub issues may disclose personal data. Prefer the
business email for private support; never commit credentials, device identifiers,
private photos, diagnostics or internal handoff documents here.

## Pawference URL compatibility

The app website repository was renamed from `pawference-site` to `Pawference-Info`.
The `pawference-site/` directory in this overview repository redirects the old
home, support, website privacy, app privacy and legal-notice URLs to the new site.
Keep these files: installed app builds and existing App Store Connect metadata
may still use the old addresses. GitHub redirects repository URLs after a rename,
but does not redirect GitHub Pages project URLs automatically.
