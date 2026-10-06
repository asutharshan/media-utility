# Contributing to Media Utility

Contributions are welcome for UI improvements, accessibility, error handling, progress reporting, queue management, duplicate detection, tests, documentation, logging, performance, packaging and lawful media-library workflows.

## Not accepted

Please do not submit functionality intended to bypass DRM, steal sessions, evade paid access, defeat account controls, obtain another person's private content, circumvent technical protection measures, or automate abusive scraping.

## Development setup

```text
python -m pip install -r requirements.txt
python media_utility.py
```

## Pull requests

Keep changes focused, explain the purpose, describe testing, do not commit cookies/media/personal data, update documentation where behaviour changes, and update `CHANGELOG.md` for user-visible changes.

## Testing

Before submitting, test UI launch, single-media scan/download, playlist/library scan, MP3, MP4, duplicate detection, history reset and queue controls where relevant. Confirm logs do not expose credentials or private data.
