# mytelly releases

Published builds of [mytelly](https://mytelly.app). This repository holds only releases; the source lives elsewhere.

- **Apps** (`apps-vX.Y.Z`): the macOS app (DMG and pkg) and the Windows app (MSI), with `SHA256SUMS`, the Sparkle `appcast.xml`, `latest.json`, and the signed Windows `update.json`. The latest release is always the apps'. Installed apps read their update feeds from `https://app.mytelly.app/updates/`, which is copied from here.
- **Home server** (`home-vX.Y.Z`): `mytelly-home` for macOS, Linux, and Windows (bare executables, archives, deb, rpm, pkg, MSI), `SHA256SUMS`, the signed update manifest `update.json` and `update.json.minisig`, and the FFmpeg and x264 source archive. The container image is `ghcr.io/adossey/mytelly-home`, and the Homebrew cask is in [adossey/homebrew-mytelly](https://github.com/adossey/homebrew-mytelly).

Every release lists SHA-256 checksums in `SHA256SUMS`.

## Source code offer

mytelly ships FFmpeg, x264, and other components under the GPL and LGPL. Each release attaches their complete source (the home server's `mytelly-home-X.Y.Z-ffmpeg-source.tar`, the macOS app's `mytelly-X.Y.Z-lgpl-sources.tar`), and the `SOURCE-OFFER.txt` in each package describes it.

For at least three years after we last distribute a version, we will also give anyone who asks a complete machine-readable copy of that source, on a medium customarily used for software interchange, for no more than our cost of physically performing the distribution. To ask, [open an issue](https://github.com/adossey/mytelly-releases/issues/new) naming the product and the version you have (`mytelly-home version`, or About mytelly in the app).

## Reporting problems

Open an issue here for a problem with a download, a checksum, or the source offer.
