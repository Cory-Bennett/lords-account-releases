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

## What's new in 0.4.0 (build 400)

- A top-level **Events** category with Guild Fest, 24-Hour Event, Hell Events,
  Solo Events, KVK, Chaos Arena and Exchange sub-tabs.
- Expanded supported automation for gathering, building and research, troop
  queues, equipment, familiars, rewards, combat and Guild Bank operations.
- Multiple Colosseum challenges and defense updates, Trial by Fire formation
  support, and improved compatibility with imported settings.
- Fixes for heartbeat timing, reconnects, shelter renewal readiness, Guild Fest
  help state and Colosseum completion.

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
