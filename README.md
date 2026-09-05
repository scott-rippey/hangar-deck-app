# Hangar Deck

The launcher for the Power Your Process Mac apps. One window and a menu bar
item show every app, whether it is installed, and whether a newer version is
out. Install and update them from here, and get told when something new
lands. On an airfield the hangar deck is where the aircraft live between
flights and get serviced. Same idea.

**[Download the latest release](https://github.com/scott-rippey/hangar-deck-app/releases/latest)**. The `.dmg` file is the installer; the other files on the release are the app's auto-update machinery. See what changed in each version: [CHANGELOG](CHANGELOG.md) or the [release notes](https://github.com/scott-rippey/hangar-deck-app/releases).

## Apps you can install from Hangar Deck

- **[CC Blackbox](https://github.com/scott-rippey/cc-blackbox-app)**: a local
  macOS IDE and flight recorder for Claude Code. Every session is recorded:
  what Claude did, what it touched, what it cost. Watch it live, replay it
  later, run scheduled headless agents on your repos.
- **[Model Radar](https://github.com/scott-rippey/model-radar-app)**: a
  read-only inventory of the AI models used across your development folder,
  with freshness tracking and retirement checks. Bring your own API key.

New apps appear in Hangar Deck automatically; there is nothing to reinstall.
Hangar Deck keeps itself current the same way.

## Install

1. Download the `.dmg` from the latest release above.
2. Open it and drag **Hangar Deck** to Applications.
3. First launch: macOS shows the standard "downloaded from the internet"
   confirmation. Click Open.
4. In the app: press Install on any app you want. Updates show up as a
   button on the app's card and as a count on the menu bar icon.

Install once. The app keeps itself current from this repository's releases
automatically; a fresh download is only needed for a new machine.

New to the app? The **[User Guide](user-guide.md)** walks through it, and the
**[feature list](features.md)** is the at-a-glance overview.

## Your Mac stays yours

Every download is verified against its published checksum and against Apple's
Developer ID signature for Power Your Process before it is installed; anything
that fails is discarded and the app tells you why. Nothing is uploaded. No
accounts, no telemetry. The only network calls are the product catalog in
this repository, each app's release feed, and the downloads you start.

## Requirements

- Apple Silicon Mac on a recent macOS

## About

The application is signed and notarized. The source code is not published;
this repository hosts installers, release notes, and the product catalog
(`catalog.json`).
Built by Scott Rippey, [Power Your Process](https://poweryourprocess.ai).
© Scott Rippey. All rights reserved.
