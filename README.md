# Windows IDE Session Extensions

No guarantees whatsoever. Some of this _will_ crash your interpreter. Requires Dyalog v20.0+ Unicode for Windows.

## Installation

Put StartupSession/seext into `[=Documents]\Dyalog APL-64 21.0 Unicode Files\StartupSession\`

## Contents

Utility functions are with uppercase and feature enabling functions are with lowercase.

To disable a feature, remove the corresponding feature source file, or change its internal name to begin with a capital letter.

| Function       | Description |
|----------------|---|
| `APLcart`      | Opens/closes APLcart palette  |
| `FSNotify`     | Displays fading notification about how to exit full screen mode |
| `Fullscreen`   | Toggles full screen mode |
| `Get`          | Calls `]Get` |
| `OnTop`        | Toggles making the IDE be on top of all other windows |
| `Resize`       | Changes the session font size |
| `Run`          | Calls all niladic functions that begin with a lowercase letter (listed below) |
| `autoLink`     | Automatically links `#` with a timestamp-named directory |
| `extStatusBar` | Extends the status bar to allow dropping files and folders |
| `extToolsMenu` | Extends the Tools menu with an APLcart entry |
| `extViewMenu`  | Extends the View menu with Always on Top, Full Screen, and Zoom In/Out |
| `setCaption`   | Sets the session caption to include `#`'s link and brief version info |
| `setFKeys`     | Sets up a lot of F-keys |
| `setFont`      | Sets the font name and size to *APL387 Unicode*, 17 |
| `setLog`       | Sets the log file to be in the temp dir and be named per the Dyalog version |
| `setOutput`    | Sets up `]Box` and `]Rows` |
