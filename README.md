# IDE Session Extensions

No guarantees whatsoever. Requires Dyalog v21.0+ Unicode.

## Installation

Run in the APL session of the version for which you want to install:
```
      ]get github.com/dyalog-labs/winide-session-extensions/tree/main/StartupSession/seext
      ⎕SE.Link.Export seext(⎕SE.Dyalog.StartupSession.VerSpec,'/seext')
```

## Contents

Utility functions are with uppercase and feature enabling functions are with lowercase.

| Function       | Description (<sup>⊞</sup> indicates requiring Microsoft Windows) |
|----------------|---|
| `Get`          | Calls `]Get` |
| `Resize`       | Changes the session font size<sup>⊞</sup> |
| `Run`          | Calls all niladic functions that begin with a lowercase letter (listed below) |
| `autoLink`     | Automatically links `#` with a timestamp-named directory |
| `extStatusBar` | Extends the status bar to allow dropping files and folders<sup>⊞</sup> |
| `extViewMenu`  | Extends the View menu with Zoom In/Out<sup>⊞</sup> |
| `setCaption`   | Sets the session caption to include `#`'s link and brief version info* |
| `setFKeys`     | Sets up a lot of F-keys |
| `setFont`      | Sets the font name and size to *APL387 Unicode*, 17<sup>⊞</sup> |
| `setLog`       | Sets the log file to be in the temp dir and be named per the Dyalog version |
| `setOutput`    | Sets up `]Box` and `]Rows` |

## Disabling features

To disable a feature, add its function name as a line in a `exclude.config` file. For example, to disable the Windows-only functions, create the file with the following content:
```
extStatusBar
extViewMenu
setFont
```
