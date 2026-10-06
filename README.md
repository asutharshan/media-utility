# Media Utility

A Windows desktop utility for scanning supported media links, loading channel/playlist libraries, selecting individual items, and downloading authorised media in MP3 and/or MP4 formats.

**Version:** 2.0  
**Author:** Arun Sutharshan  
**Date:** 06 October 2026  
**Status:** Personal experiment / educational utility

> **Important:** Use Media Utility only for media that you own, created, or are authorised to download. This project does not grant rights to content, bypass DRM, or override website terms, copyright, authentication requirements, or access controls.

## Features

- Colourful Windows desktop interface
- Multiple URL input
- Automatic source detection for supported URLs
- YouTube individual video, playlist and channel/library support
- Library preview before download
- Select all / select none / invert selection / individual selection
- MP3 and MP4 multi-select output
- MP3 quality selector: 128–320 kbps
- MP4 maximum resolution selector: Best, 2160p, 1440p, 1080p, 720p, 480p, 360p
- Optional thumbnail and metadata embedding
- Browser-cookie support for legitimate authenticated access
- Persistent duplicate detection and download history
- Queue pause/resume/stop controls
- Per-file percentage, transfer speed and ETA where available
- Windows `.exe` build script

## Supported sources

Media Utility uses `yt-dlp` as its media extraction engine. Common examples include YouTube, Facebook and TikTok. Other sites may work when supported by the installed `yt-dlp` version.

Website compatibility can change without notice because sites frequently change interfaces, authentication mechanisms, delivery formats and anti-automation measures.

## Channel / playlist workflow

1. Paste a supported channel, playlist or media URL.
2. Select **Scan / Load Library**.
3. Media Utility retrieves the available item list without downloading the media files.
4. Select all, none, invert, or individual items.
5. Choose MP3, MP4, or both.
6. Choose quality/resolution.
7. Select **Download Selected**.

Very large libraries can take time to enumerate and may be subject to website rate limits.

## Duplicate detection

Media Utility keeps a persistent local download history at:

```text
%APPDATA%\MediaUtility\download_history.json
```

Duplicate detection is primarily based on source/extractor + media ID + requested format. MP3 and MP4 are tracked separately. Closing and reopening the app does not reset this history. Use **History → Reset Duplicate History** to clear it. Resetting history does not delete downloaded media files.

## Browser cookies

Browser-cookie functionality is intended only for content that the logged-in user is already legitimately authorised to access. It is not intended to steal sessions, bypass authentication, defeat DRM, or circumvent paid access.

Do not post cookies, tokens, credentials or private URLs in public GitHub issues.

## Installation

Recommended: Windows 10/11, Python 3.10+, pip and Tkinter.

Run:

```text
INSTALL_AND_RUN.bat
```

## Build the standalone Windows EXE

Run:

```text
BUILD_EXE.bat
```

The output should appear under:

```text
dist\MediaUtility.exe
```

## Repository structure

```text
MediaUtility/
├─ media_utility.py
├─ INSTALL_AND_RUN.bat
├─ BUILD_EXE.bat
├─ requirements.txt
├─ README.md
├─ LICENSE
├─ DISCLAIMER.md
├─ NOTICE.md
├─ SECURITY.md
├─ CONTRIBUTING.md
├─ CHANGELOG.md
├─ CODE_OF_CONDUCT.md
├─ RELEASE_CHECKLIST.md
├─ .gitignore
├─ docs/
│  ├─ INSTALLATION.md
│  └─ TROUBLESHOOTING.md
├─ screenshots/
│  └─ README.md
└─ .github/
   ├─ ISSUE_TEMPLATE/
   │  ├─ bug_report.md
   │  └─ feature_request.md
   └─ pull_request_template.md
```

## Privacy

Media Utility does not intentionally upload download history, local file paths, cookies, URLs or settings to a project-controlled server. URLs are, of course, sent to the relevant source website during scanning/downloading.

## Legal / acceptable use

Use this software only where you have permission. You are responsible for complying with copyright law, local law, contractual restrictions, website terms, account conditions and licensing requirements. See [DISCLAIMER.md](DISCLAIMER.md) and [NOTICE.md](NOTICE.md).

## License

Released under the MIT License. See [LICENSE](LICENSE).

## Disclaimer

This software is provided **"as is"**, without warranty of any kind. Created by **Arun Sutharshan** for personal experiment and educational purposes. See [DISCLAIMER.md](DISCLAIMER.md).
