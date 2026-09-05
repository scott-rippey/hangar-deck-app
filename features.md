# Hangar Deck: Feature Overview

Present tense; what runs today.

## The window

A single glass window. The header carries the app icon, the last-checked time
(or the count of updates available), an Apps / Settings switch, and Check Now.

## Apps

One card per product from the catalog: the app's own icon (read from the
installed bundle; from the catalog when not installed), name, status pill,
tagline, installed version, latest version when different, and a Release
notes link. The single action button follows the status:

- Not installed: Install x.y.z
- Update available: Update to x.y.z
- Up to date: Open
- Installing: a progress bar with the stage (downloading with byte counts,
  unpacking, verifying the Developer ID signature, installing)
- Quit it to update: the app was open and did not quit when asked; the button
  offers the update again
- Install failed: a plain-English reason and Try Again
- Feed unreachable: the installed state stays visible and Open still works
  when the app is installed; no install or update until the next check
- Hangar Deck itself: Update stages the new version and the button becomes
  Restart to Update; the swap happens at quit.

Click anywhere on a card (outside its buttons) to open the details panel:
the icon, the full description, installed and latest versions, Release notes
and Website links, the app's one action, and OK. Esc, OK, or a click outside
closes it.

A footer line says whether the catalog is live from GitHub or the built-in copy.

## Menu bar

A hangar glyph (template image, so it follows light and dark menu bars) with
a badge count when updates are available. Its menu lists every product with
its state as a clickable row (install, update, open, or restart), Open Hangar
Deck, Check for Updates Now, and Quit. Closing the window leaves the app
running in the menu bar.

## Checks and notifications

Every product's feed is checked at launch and every hour. A new version that
is newer than the installed one produces one notification per version;
clicking it opens the window. A finished install notifies too; clicking opens
the app.

## Settings

Glass window (on by default; recreates the window), Open at login (the app
registers itself as a login item; when the OS launches it at login it stays
in the menu bar with no window until you click), Notify me about updates. The About row shows the Power Your
Process mark, the product name, the running version, and the newer version
when one exists.

## Safety

Every download is streamed with a sha512 check against the feed, unpacked by
ditto, verified by codesign against a designated requirement (Developer ID
anchor, exact bundle id, and the Power Your Process Team ID built into the app), and its Info.plist
version must equal the feed's. Only then is the bundle swapped into place by
rename, with rollback. Nothing is ever uploaded.
