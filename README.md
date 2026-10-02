# bavarianTechWorks website

Public GitHub Pages home for three independently maintained app websites:

| App | Website | Support | App privacy |
| --- | --- | --- | --- |
| Pawference | https://makki93.github.io/pawference-site/ | https://makki93.github.io/pawference-site/support.html | Pending before external beta; its current privacy page covers the website only |
| GalleryTidy | https://makki93.github.io/GalleryTidy-Info/ | https://makki93.github.io/GalleryTidy-Info/ | https://makki93.github.io/GalleryTidy-Info/privacy.html |
| WaitASec | https://makki93.github.io/WaitASec-Info/ | https://makki93.github.io/WaitASec-Info/#support | https://makki93.github.io/WaitASec-Info/privacy/ |

Home: https://makki93.github.io/
Contact: bavariantechworks@mailbox.org

## Scope and publishing

This repository contains only static public website files. The three application
repositories remain private. GitHub Pages publishes `main` at the repository root;
`.nojekyll` disables Jekyll. There is no JavaScript, tracking, form backend, external
font or package dependency.

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
- `assets/waitasec.svg`: unchanged public WaitASec website icon.
- `assets/brand.svg`: simple vector monogram created for this website.

These app marks identify the owner's apps; they are not stock imagery or permission
to reuse the application assets in third-party products.

## Local preview

```sh
python3 -m http.server 18766 --bind 127.0.0.1 --directory .
```

Public inquiries through GitHub issues may disclose personal data. Prefer the
business email for private support; never commit credentials, device identifiers,
private photos, diagnostics or internal handoff documents here.
