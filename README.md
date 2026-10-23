# Lords Account for Mac

Native Lords Mobile account management and supported gameplay automation for
Apple silicon and Intel Macs running **macOS 14 or later**.

[Download the latest installer](https://cory-bennett.github.io/lords-account-releases/)
· [Release history](https://github.com/Cory-Bennett/lords-account-releases/releases)

## Install and update

1. Download the DMG and open it.
2. Drag **Lords Account** to **Applications**, then eject the image.
3. Open the installed app and add your game account using official IGG sign-in.

The universal app is Developer ID signed and Apple notarized. Installing and
updating require no Apple or GitHub login. Automatic update checks and downloads
are enabled by default; downloaded updates install when you quit. Use
**Lords Account → Check for Updates…** for a manual check, or General settings
to change update preferences. Keep the app in Applications for updates.

## What's new in 0.4.1 (build 401)

- Compact dark workspace with a named account sidebar, one row of account tabs,
  an Overview dashboard and direct settings and Activity navigation.
- Overview displays received account/resource/army observations and real routine
  diagnostics. Unknown or offline data is labeled; Recall All retains its review.
- Heroic Saga adds optional owned-Compass refreshes with a target grade, token
  reserve and configurable budget. Compass use defaults off; gem purchases stay disabled.
- Game/Guild mail deletion admits only read, unsaved, reward-free letters with
  verified native subtypes. Attachments and unknown subtypes remain protected.
- Guild-management policy and Realm admission checks are expanded. Live guild
  membership mutations and unverified Realm execution remain unavailable.

## Using the app

Manage accounts through Settings and Activity. The crossed-swords menu bar icon
shows online accounts in green, sleeping accounts in yellow with their next wake,
and offline accounts in red. Closing the dashboard leaves the menu bar app
available; choose Open Dashboard to return or Quit to exit.

Supported routines act only when their required current game data and saved
choices allow them. Activity reports accepted, rejected, waiting and unconfirmed
actions. Some event controls and imported Windows preferences still lack execution
support; a visible setting does not mean that every game mode is automated.
Live acceptance varies by feature, and Intel hardware testing remains separate
from universal binary verification. Updating preserves saved choices and does
not enable purchases or external delivery by itself.

## Privacy and downloads

Game sign-in uses IGG. Saved sign-in tickets use macOS Keychain; passwords are
not saved. Account workspaces and settings remain local to each Mac. This public
repository contains installers, checksums and the signed update feed; application
source, private account data, credentials and migration files are excluded.

Each release includes a DMG, an app ZIP and `SHA256SUMS`. Prefer the DMG for
installation. Check downloaded assets from their download directory with:

```sh
shasum -a 256 -c SHA256SUMS
```
