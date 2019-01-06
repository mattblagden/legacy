# Mac Keys

Key placement varies between keyboards (e.g. modifier keys on the Apple MacBook keyboard vs the Apple USB Keyboard), and default key functions differ between OSes (e.g. Home on Windows means Beginning of Line, Home on macOS means Beginning of Document). This tool remaps keys to a layout that can be used consistently across various keyboards and OSes.

# Installation

```
svn checkout https://github.com/mattblagden/Projects/trunk/MattBlagden.MacKeys && cd MattBlagden.MacKeys
./build.sh
sudo ./install.sh
```

# Mapping

To remain consistent across keyboards and OSes, this mapping:
* Uses none of the keys that commonly move between keyboards (fn, control, alt, command/windows, F1-F12, numpad, ins, del, home, end, pgup, pgdn, etc.)
* Uses a single modifier key for primary actions, modifier+shift for derivatives (select text to start of line, previous window/tab, etc.)
* Only implements global concepts (application-specific combinations should be set in the individual application)

CapsLock is used as the modifier in this mapping, as it generally stays in the same place between keyboards, and can be easily pressed with the pinky.

While holding Caps Lock:

|Key|Action|+Shift Action|
|---|---|---|
|Q|Previous Tab| |
|W|Next Tab| |
|E|Close Tab| |
|T|Create Tab| |
|\`|Next Window in Application|Previous Window in Application|
|Tab|Next Application|Previous Application|

|Key|Action|+Shift Action|
|---|---|---|
|A|Select All| |
|X|Cut| |
|C|Copy| |
|V|Paste| |
|Z|Undo|Redo|
|Delete|Forward delete| |

|Key|Action|+Shift Action|
|---|---|---|
|N|New| |
|S|Save| |

|Key|Action|+Shift Action|
|---|---|---|
|,|Page Up|Select Previous Page|
|.|Page Down|Select Next Page|
|Up|Beginning of Line|Select to Beginning of Line|
|Down|End of Line|Select to End of Line|
|Left|Beginning of Word|Select to Beginning of Word|
|Right|End of Word|Select to End of Word|

|Key|Action|+Shift Action|
|---|---|---|
|I|Inspect (Terminal Inspect, Browser Developer Tools, File Properties, etc.)| |
|L|Location (Folder path, Browser URL, etc.)| |
|F|Find in Document|Find in Files|
|Esc|CTRL+C| |
