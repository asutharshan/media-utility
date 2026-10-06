# Troubleshooting

## No module named pip

Repair or reinstall a full Python distribution and enable pip.

## `ensurepip` unavailable

You are probably using a minimal or embedded Python distribution.

## Tkinter missing

Enable `tcl/tk and IDLE` in the Python installer.

## Browser cookies fail

Possible reasons:

- browser database is locked;
- session expired;
- cookie encryption is unsupported;
- source site changed authentication behaviour.

Never export or publish cookies.

## Channel/library scan is slow

Large channels can contain hundreds or thousands of items and may be rate-limited.

## Duplicate warning

Persistent history is stored under:

```text
%APPDATA%\MediaUtility\download_history.json
```

Use:

```text
History → Reset Duplicate History
```

to clear it.

## Source website stops working

Update `yt-dlp`:

```text
python -m pip install --upgrade yt-dlp
```
