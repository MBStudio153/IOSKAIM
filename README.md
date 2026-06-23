# KAIM Calculator

Knowledge Asset Impairment Model calculator + full guide, built with Capacitor for Android and iOS.

## Project structure

```
www/                        ← Capacitor web root
  index.html                ← KAIM Calculator
  book.html                 ← In-app book reader
  book/
    sections/               ← Book content (xhtml)
    images/                 ← cover.png
    styles/                 ← stylesheet.css
resources/
  icon-512.png              ← App icon (512×512)
  feature-graphic-1024x500.png  ← Google Play feature graphic
capacitor.config.json
package.json
codemagic.yml               ← Android + iOS build pipelines
```

## Before submitting

1. Change `appId` in `capacitor.config.json` from `com.yourcompany.kaimcalculator` to your real bundle ID
2. Update the `bundle_identifier` in `codemagic.yml` iOS section to match
3. Fill in App Store Connect API key values in Codemagic dashboard (replace `Encrypted(...)` placeholders)
4. Host `privacy-policy.md` publicly (GitHub Pages works) and add the URL to both store listings

## Build

Codemagic handles all builds — just push to `main`.
