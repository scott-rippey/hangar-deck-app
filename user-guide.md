# Hangar Deck User Guide

## Install

Download the DMG from the hangar-deck-app releases page, open it, and drag
Hangar Deck to Applications. Open it once. From then on it lives in the menu
bar; the window opens from the menu bar icon, the Dock, or Cmd+1.

## Apps

Each card is one Power Your Process app. The button does the obvious thing:
Install if you do not have it, Update if a newer version is out, Open if you
are current. Installs take a minute or two on a normal connection; the card
shows the download, the unpacking, and the signature check as they happen.

If an app is open when you update it, Hangar Deck asks it to quit first. If
it does not quit (an unsaved document, a dialog), the card says so; close the
app yourself and press Update again.

Click a card to read the full description of an app, with its versions,
Release notes and Website links, and the same Install, Update, or Open
action. OK, Esc, or clicking outside closes it.

Release notes opens the app's release page in your browser.

## Hangar Deck updating itself

When a newer Hangar Deck exists, Update downloads and verifies it, then the
button changes to Restart to Update. The swap happens when Hangar Deck quits,
and it relaunches on its own.

## Menu bar

The hangar icon shows a number when updates are waiting. Click it for the
list of apps and their states; click a row to install, update, or open.

## Settings

- Glass window: see through the window to what is behind it.
- Open at login: start hidden in the menu bar when you log in.
- Notify me about updates: one notification per new version, checked hourly.

## Good to know

- Hangar Deck never touches an app it did not verify: the download must match
  its published checksum and carry the Power Your Process Developer ID
  signature, or it is discarded and the card tells you why.
- Nothing is uploaded, ever. The only network calls are the catalog, each
  app's release feed, and the downloads you start.
