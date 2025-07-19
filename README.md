# Robohotkey

Simple Linux X11 temporary key remapper with tray icon and hotkey toggling.

## Usage

1. Write a hotkey file following the [robohotkey file syntax](#robohotkey-file-syntax).

    Check `sample.rbk` to see an example.

2. Run `robohotkey hotkey_file.rbk`

3. Optionally, add the robohotkey mime type.

    Copy `robohotkey.xml` into `~/.local/share/mime/packages/`

    Run `update-mime-database ~/.local/share/mime`

## Robohotkey file syntax

### Hotkeys

To define a hotkey use the following syntax:

```
input_keyname -> output_keyname
```

Check [Keys List](./key_list.md) or run `xmodmap -pke` for a list of all keycodes and keynames.

Example:

```
Scroll_Lock -> Alt_L
```

### Multiple Hotkeys

To define multiple hotkeys they must be newline separated.

```
input_keyname -> output_keyname
input_keyname2 -> output_keyname2
```

### Comments

Use `//` at the start of a line to comment that line out.

## Dependencies

Python 3: [Download link](https://www.python.org/downloads/)

Python `pystray` and `pillow` modules: To install then, enter the following command in cmd or a terminal:

```
pip install pystray pillow
```
