# Robohotkey

Simple Linux X11 temporary key remapper with tray icon and hotkey toggling.

## Usage

1. Write a hotkey file.

    Check `sample.rbk` to see an example.

    Run `xmodmap -pke` for a list of all keycodes and keynames.

2. Run `robohotkey hotkey_file.rbk`

3. Optionally, add the robohotkey mime type.

    Copy `robohotkey.xml` into `~/.local/share/mime/application/`

    Run `update-mime-database ~/.local/share/mime`

## Dependencies

Python 3: [Download link](https://www.python.org/downloads/)

Python `pystray` and `pillow` modules: To install then, enter the following command in cmd or a terminal:

```
pip install pystray pillow
```
