# Arios TV

**Your library. Your sources. Your TV.**

[![Android TV](https://img.shields.io/badge/Android_TV-Android_7%2B-3DDC84?logo=android)](https://github.com/warpirobo/openmediatv-releases/releases/latest)
[![Fire TV](https://img.shields.io/badge/Fire_TV-Compatible-FF9900)](https://github.com/warpirobo/openmediatv-releases/releases/latest)
[![Download](https://img.shields.io/github/v/release/warpirobo/openmediatv-releases?label=Download)](https://github.com/warpirobo/openmediatv-releases/releases/latest)
[![Buy me a coffee](https://img.shields.io/badge/%E2%98%95_Buy_me_a_coffee-PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.com/paypalme/ITARIOS)

Arios TV is a remote-first media library and player for **Android TV and Fire TV**.
Browse your rclone sources, identify movies and series, resume playback, and manage
favorites and watch history per profile. IPTV and TorBox are optional services.

## Features

- **Integrated rclone:** OneDrive / SharePoint, Google Drive, crypt, combine and other compatible remotes. Import `rclone.conf` or use guided setup, without mounting drives.
- **Visual library:** movies, series, episodes, optional collections and multiple versions of the same title. Metadata and artwork from TMDB, TheTVDB and compatible providers.
- **Playback:** Media3 / ExoPlayer, ASS rendering with libass, Custom OpenHub subtitle styling and track selection. FFmpeg provides alternative audio decoding when applicable; compatibility depends on the file, device and audio setup.
- **Profiles:** separate history, progress and favorites, child-profile options and optional PINs.
- **Optional IPTV:** remote TXT / M3U playlists, search, favorites and multiple sources per channel.
- **Optional TorBox:** movie, series and anime catalogs, My torrents, favorites, resume playback and language, resolution and edition filters. Season and episode artwork when available.
- **External providers:** Torrentio, Comet, Hydra, MediaFusion and configurable addons. DeepFlix and PlavioHD provide direct HTTPS links outside TorBox's cache. TorBox credentials are not shared with these addons.
- **Online subtitles:** OpenSubtitles and Subtitulamos.tv for series, through the TorBox player. Availability and timing depend on the provider and release.
- **Trackers:** optional SIMKL and WeTrakr integration.
- **Maintenance:** selectable backups, playback diagnostics and in-app updates.

## Download and install

1. Open [the latest release](https://github.com/warpirobo/openmediatv-releases/releases/latest).
2. Download the **public-armeabi-v7a-release.apk** TV installer.
3. Allow installation from your download tool and confirm in Android.
4. Choose your language and configure sources. Enable optional services under **Settings → IPTV · TorBox**.

Minimum requirement: **Android 7 / API 24**. This channel distributes the TV
variant, not the mobile version with Cast. Manufacturer restrictions may apply.

## Update without losing your settings

Open **Settings → App updates**, download the update and confirm installation
when Android prompts you. After a successful installation, the app cleans up the
installer it downloaded. It does not delete APKs you saved manually elsewhere.

**Update without uninstalling.** Existing settings, accounts and previously saved
provider registrations are retained. Data from the old separate TorBox app is not
automatically migrated into the normal app.

## Provider keys and privacy

The public APK **does not include private TMDB / TheTVDB keys**. On a clean
installation, enter your own keys under provider settings. Bridge versions save
existing registrations locally so they remain available after upgrading.
Credentials are encrypted on the device and are not published here.

The **Arios TV application source remains private**. This repository contains APK
distribution metadata, documentation and `update.json`, not application source,
personal configurations or signing keys. Optional services communicate with their
respective providers. Arios TV does not provide preloaded content or third-party accounts.

## Limits and availability

- Quality and language filters use source labels; a catalog poster does not guarantee an available 4K stream.
- My torrents progressively indexes up to 10,000 summaries per account and displays a limit warning. The initial pass may take time; subsequent visits use the local index.
- PlavioHD live-sports catalogs are not imported in this movie/series module.
- FMHY websites are not all compatible addons and are not automatically converted into providers.
- Playback capabilities and service availability depend on the device and provider. Release notes describe the scope of verification.

## Support and diagnostics

[Open an issue](https://github.com/warpirobo/openmediatv-releases/issues) with your
device model, app version and reproduction steps. Review diagnostics before
sharing them. **Do not post passwords, tokens, keys, rclone configurations or private links.**

## Third-party components and licenses

Arios TV uses AndroidX Media3, FFmpeg, libass, rclone and their dependencies.
See **About → Licenses** in the app. Release download assets contain only APKs.

This software uses FFmpeg libraries under LGPL 2.1 or later. Their unchanged
[corresponding source and build recipes](https://github.com/warpirobo/openmediatv-releases/raw/refs/heads/main/licenses/ffmpeg/OpenMediaTV-0.15.26.5-FFmpeg-source.zip)
remain separately available for the published 0.15.26.5, 0.15.26.6 and 0.15.27 APKs.
**This archive is third-party component source, not the Arios TV application source.**
See [FFmpeg's distribution guidance](https://ffmpeg.org/legal.html).

External providers are independent of Arios TV. Their availability, terms and
content rights are not controlled by this project.

## Support development

[☕ Buy me a coffee through PayPal](https://www.paypal.com/paypalme/ITARIOS)

The same support link used by [rclone-nexus-kodi](https://github.com/warpirobo/rclone-nexus-kodi).
