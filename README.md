# Tau Time Tracker

Captures the active window title and logs it to a sqlite database.
Example service files are provided for systemd.

## Requirements

* Python >= 3.6
* `xdotool` for Linux

The `xdotool` requirement could be lifted by supporting alternate backends.
Currently this just calls `xdotool getwindowfocus getwindowname` under the hood.
