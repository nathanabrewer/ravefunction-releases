# Rave Function: downloads

Builds of Rave Function to install yourself, outside the app stores. The
download page, with what each one is and how to install it:
https://ravefunction.com/download/

This repository holds the builds (on its Releases) and their licence notices
only: no source code. Every release carries each file under the same name, so
`releases/latest/download/<file>` always gives the newest.

| File | What |
|---|---|
| `RaveFunction-Quest.apk` | Rave Function for Meta Quest 2, 3, 3S and Pro |
| `RaveFunction-Watch-Android.apk` | Rave Function Watch for Android phones: hear a party in step and watch the stage |
| `RaveFunction-Studio-Mac.zip` | Rave Function Studio for the Mac, when a release has it: hosts a party and runs the show |
| `SHA256SUMS.txt` | The SHA-256 of each file: `shasum -a 256 -c SHA256SUMS.txt` |

Rave Function is in development. Privacy: https://rhythm.dftz.org/privacy/

## Licences

The apps are made with Godot Engine (MIT License) and other open-source
software. [licenses/THIRD-PARTY-NOTICES.txt](licenses/THIRD-PARTY-NOTICES.txt)
lists every component, its licence and its source, beside the full licence
texts in [licenses/](licenses/). The source of the changed godot-ffi (Mozilla
Public License 2.0) is
[licenses/godot-ffi-0.5.5-source.zip](licenses/godot-ffi-0.5.5-source.zip).
Music and other credits: [licenses/CREDITS.md](licenses/CREDITS.md).

Meta Quest is a trademark of Meta Platforms, Inc. Android is a trademark of
Google LLC. Mac is a trademark of Apple Inc.
