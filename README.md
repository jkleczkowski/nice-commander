# NiceCommander

A fast, keyboard-driven, two-panel file manager in the spirit of Total Commander, built with .NET and Avalonia.
Familiar Total Commander shortcuts, native behaviour on each operating system.

> **Status: pre-release.** Builds are unsigned and still change between versions. macOS (Apple Silicon) is the
> primary platform; the Windows x64 build is experimental.

This repository publishes release builds and the update feed. Development happens in a separate repository.

## Features

- **Two panels** with a fully keyboard-driven workflow, sorting, marking, filtering and a virtualized list that stays
  smooth with 100,000+ entries.
- **File operations** run as background jobs: copy (F5), move (F6), new folder (F7), delete to Trash (F8) or permanently
  (Shift+F8), rename (F2). Same-volume copies use native clones.
- **Lister (F3):** text with encoding detection, hex and image views; large files are read in windows and never loaded
  into memory whole. **F4** opens the file in your own editor.
- **SFTP:** browse and work on remote servers through the system `ssh` (your `~/.ssh/config`, keys, agent and
  `ProxyJump` just work). Includes remote editing with conflict detection, resumable transfers and sudo.
  Passwords are stored in the macOS Keychain.
- **Archives:** open ZIP, TAR (gz, bz2, xz, zst), 7z and RAR like folders (Enter or Ctrl+PageDown), including
  password-protected ones. Extract with F5/F6, pack with Alt+F5 to ZIP (optionally AES-256 encrypted), tar.gz,
  tar.xz or tar.zst.
- **Command line** under the panels: commands run in Terminal.app in the current panel's directory; `cd` changes
  the panel in place.
- **Quick filter:** Ctrl+S (Cmd+F on macOS).
- **Automatic updates:** Help → Check for updates.

## Installation

1. Download the installer for your system from the [Releases](https://github.com/jkleczkowski/nice-commander/releases)
   page.
2. Because the builds are not signed yet:
   - **macOS:** if the system refuses to open the app, go to *System Settings → Privacy & Security* and choose
     *Open Anyway*.
   - **Windows:** on the SmartScreen prompt choose *More info → Run anyway*.

Once installed, NiceCommander updates itself from this repository's releases.

## Keyboard basics

| Key | Action |
| --- | --- |
| Tab | Switch panel |
| Enter / Backspace | Open / go to parent folder |
| Space, Insert | Mark entry |
| F2 | Rename |
| F3 / F4 | View / edit |
| F5 / F6 | Copy / move |
| F7 | New folder |
| F8 / Shift+F8 | Delete to Trash / delete permanently |
| Alt+F5 | Pack into an archive |
| Ctrl+S (Cmd+F) | Filter the panel |

On macOS the function keys also have Cmd+digit equivalents (e.g. Cmd+5 for copy).

## Release notes

Each release lists its changes on the [Releases](https://github.com/jkleczkowski/nice-commander/releases) page.
