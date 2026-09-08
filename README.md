# Oscar for Windows — releases

Downloads for the Oscar desktop app. **There is no source code here**; Oscar
itself lives in a private repository. This exists only so the installer has a
public address.

## Get it

**[Download the latest installer](https://github.com/NeonG4/Oscar-Windows-App-Release/releases/latest/download/OscarSetup.exe)**

Or, from the website, <https://oscarassistant.com/download> — which redirects
here, so the link on the site never has to change when a release does.

64-bit Windows 10 or 11. It installs for you alone, under
`%LOCALAPPDATA%\Programs\Oscar`, so it never asks for administrator.

The app is not code-signed yet, so Windows will warn you the first time you run
it: choose **More info**, then **Run anyway**.

## Why this repository is empty

The installer is attached to each [Release][releases] as an **asset**, not
committed as a file. Those are different things, and the difference matters:

- A release asset is stored outside git. Downloading it costs nothing and
  cloning this repository does not drag 67 MB along with it.
- A committed binary is in the history **forever**, on every clone, and a second
  version does not replace the first — it doubles it. This repository briefly
  had two of them and was 134 MB before it held anything worth reading.

So: assets, always. The one rule that keeps it working is that every release
names its asset exactly `OscarSetup.exe`, because that fixed name is what makes
`releases/latest/download/OscarSetup.exe` resolve. The version lives in the tag.

[releases]: https://github.com/NeonG4/Oscar-Windows-App-Release/releases
