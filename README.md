# Media Utility

A Windows desktop utility for scanning supported media links, loading channel or playlist libraries, selecting individual items, and downloading authorised media in MP3 and/or MP4 formats.

**Version:** 2.0.1  
**Author:** Arun Sutharshan  
**Date:** 06 October 2026  
**Licence:** Media Utility Personal & Non-Commercial License

> **Authorised Use Notice:** Use Media Utility only with content you own, created, are licensed to use, or are otherwise authorised to access and download. The software does not grant rights to third-party content and does not bypass DRM or technical access controls.

## Intended use

Media Utility is primarily intended for:

- personal use;
- educational use;
- non-commercial research and experimentation;
- internal evaluation;
- archiving or managing your own content;
- business use where the organisation owns or is properly licensed to use the content.

Commercial redistribution, paid-service use, OEM bundling, or commercial exploitation of the software itself requires written permission from the copyright holder.

## Features

- Colourful Windows desktop interface
- Multiple URL input
- Automatic source detection
- YouTube single-video support
- YouTube playlist support
- YouTube channel/library scanning
- Library preview before download
- Select all / select none / invert selection
- Individual item selection
- MP3 and MP4 multi-select
- Selectable MP3 quality
- Selectable MP4 maximum resolution
- Optional thumbnail embedding
- Optional metadata embedding
- Browser-cookie support for legitimate authenticated access
- Persistent duplicate detection
- Download history
- Queue pause/resume/stop controls
- Per-file detail logging
- Live percentage progress
- Transfer speed and ETA where available
- Windows EXE build support

## Channel / library workflow

1. Paste a supported channel, playlist, or media URL.
2. Choose **Scan / Load Library**.
3. Media Utility retrieves the item list without downloading the media itself.
4. Review the library.
5. Select all, none, invert, or choose individual items.
6. Choose MP3, MP4, or both.
7. Choose output quality/resolution.
8. Download only the selected items.

Very large libraries may take time to enumerate and may be subject to source-site rate limits or authentication requirements.

## Duplicate detection

Completed items are stored locally under:

```text
%APPDATA%\MediaUtility\download_history.json
```

Duplicate detection is based primarily on the source/extractor, media ID, and requested format.

MP3 and MP4 are tracked separately.

Duplicate history remains across application restarts until the user explicitly chooses:

```text
History → Reset Duplicate History
```

Resetting the history does not delete downloaded media files.

## Browser cookies

Browser-cookie integration is intended only for content that the logged-in user is already authorised to access.

Supported browser selections may include Chrome, Edge, Firefox, Brave, Opera and Vivaldi.

Media Utility is not intended to:

- bypass authentication;
- defeat paid access;
- steal sessions;
- obtain another person's private content;
- bypass DRM or technical protection measures.

Never publish cookies, tokens or private authentication information in GitHub issues.

## Installation

Recommended environment:

- Windows 10 or Windows 11
- Python 3.10+
- pip
- Tkinter / tcl-tk

Run:

```text
INSTALL_AND_RUN.bat
```

## Build a standalone Windows EXE

Run:

```text
BUILD_EXE.bat
```

The build output is typically:

```text
dist\MediaUtility.exe
```

Build and test Windows executables on Windows.

## Privacy

Media Utility does not intentionally upload download history, local settings, cookies or local file paths to a project-controlled server.

When browser-cookie support is enabled, cookies are passed locally to the extraction engine for legitimate authentication against the relevant source.

Do not post logs containing private URLs, account identifiers, cookies, tokens, customer information or local secrets.

## Commercial use

The software is **not generally licensed for commercial redistribution or paid-service use**.

However, an organisation may use it internally to manage content that it owns or is properly licensed to use, subject to the licence terms and relevant platform rules.

For broader commercial use, obtain written permission from the copyright holder.

See [LICENSE](LICENSE).

## Third-party platforms

Media Utility is an independent project and is not affiliated with, endorsed by, sponsored by, or officially connected to YouTube, Google, Meta, Facebook, TikTok, ByteDance or any other supported platform.

## Third-party dependencies

Media Utility relies on third-party libraries and tooling, including `yt-dlp` and FFmpeg-related components.

Those dependencies retain their own licences and terms.

## Security

See [SECURITY.md](SECURITY.md).

## Disclaimer

See [DISCLAIMER.md](DISCLAIMER.md).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## Changelog

See [CHANGELOG.md](CHANGELOG.md).
