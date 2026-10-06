# Troubleshooting

## `No module named pip`
Repair/reinstall Python and enable pip, tcl/tk and IDLE, and Python Launcher.

## `ensurepip` is unavailable
You may be using an embedded/minimal Python distribution. Install the normal Windows Python distribution.

## Tkinter is missing
Repair Python and enable `tcl/tk and IDLE`.

## Browser cookies fail
Possible causes include a locked browser database, cookie encryption incompatibility, expired session, or site changes. Try closing the browser. Never export or post cookies publicly.

## Channel/library scan is slow
Very large channels may contain hundreds or thousands of items and can be rate-limited. Test with a small playlist first.

## A website suddenly stops working
Update `yt-dlp`:

```text
python -m pip install --upgrade yt-dlp
```
