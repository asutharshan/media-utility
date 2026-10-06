# Security Policy

## Supported version

| Version | Supported |
|---|---|
| 2.x | Yes |
| 1.x | Best effort only |

## Reporting a vulnerability

Do **not** publish secrets or sensitive information in a public GitHub issue. This includes browser cookies, authentication tokens, API keys, passwords, private media URLs, private account identifiers, personal information, or sensitive local paths.

For reproducible non-sensitive reports, include the Media Utility version, Windows version, Python version, steps to reproduce, expected behaviour, observed behaviour and redacted logs.

For sensitive reports, use a private security reporting mechanism if one is enabled for the repository.

## Browser cookies

Browser-cookie access should remain opt-in. The project should never intentionally upload cookies to a project-controlled server or write raw cookies/tokens to logs.

## Dependency security

Keep dependencies current:

```text
python -m pip install --upgrade yt-dlp imageio-ffmpeg
```

Downloaded media should be treated as untrusted content and should never be executed automatically.
