# Robohotkey

Simple Linux X11 temporary key remapper.

## Usage

1. Write a hotkey file.

    Check `sample.rbk` to see an example.

    Run `xmodmap -pke` for a list of all keycodes and keynames.

2. Run `robohotkey hotkey_file.rbk`

## Dependencies

Python 3: [Download link](https://www.python.org/downloads/)

Python `pystray` and `pillow` modules: To install then, enter the following command in cmd or a terminal:

```
pip install pystray pillow
```
