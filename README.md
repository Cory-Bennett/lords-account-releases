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

## What's new in 0.4.2 (build 402)

- Recent Activities replaces the flickering routine rows, keeps background polling quiet,
  and shows confirmed chest and guild-gift rewards with item names, quantities and rarity.
  Routine configuration and prerequisites remain available in a separate status review.
- Numeric inputs accept exact K/M/B shorthand and optional currency prefixes, normalize
  on commit, and preserve saved values when an entry is invalid or outside its limits.
- Direct Bank, Guild and Quests navigation, distinct Buildings/Research/Army sections,
  a roomier current-task header and a scheduled-wake countdown in the account sidebar.
- Overview honors the saved resource visibility preference. Settings help distinguishes
  active native behavior from imported preferences retained for compatibility.
- Both Exchange editors share explicit enable/disable, default and zero-limit behavior.
  Claims still apply only to already-earned points; mission automation remains separate.
- Supply offers a read-only current guild refresh and recipient picker. Saved recipients
  are revalidated against current identity and guild membership before any shipment.

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
