# Tau Time Tracker

Captures the active window title and logs it to a sqlite database.
Example service files are provided for systemd.

## Setup


```bash
% cd path/to/cloned/tau
% pip3 install pipenv-shebang --user
% pipenv install
% ./tau --help
```

## Requirements

* Python >= 3.6
* `xdotool` for Linux

The `xdotool` requirement could be lifted by supporting alternate backends.
Currently this just calls `xdotool getwindowfocus getwindowname` under the hood.
