# Pocket Books support

Pocket Books is an offline iPhone player for your own MP3, M4B and M4A audiobooks.

## Add books

Connect your unlocked iPhone to a Mac. In Finder, select the iPhone, choose Files and drop audio files or a folder onto Pocket Books. Wait for the transfer to finish, then open the app. Each folder becomes one book; embedded M4B chapters are shown when present.

## Finder cannot find the required file

A development app update can leave Finder with a stale sharing connection. Your files may still be intact. Reopen the device’s Files tab and retry. If the problem persists after an update, finish any transfer, then restart Finder and its sharing helper on your Mac:

```sh
killall AMPDevicesAgent Finder
```

Finder windows may close and reopen. Unlock the iPhone, reopen its Files tab and retry. Do not uninstall Pocket Books to troubleshoot: uninstalling removes its audio and saved progress.

## Listening and progress

Library taps open book details without starting another book. Press the Play icon to resume, or tap a chapter to start it from the beginning. The mini player and full-page player can seek within the current chapter. Headphone next/previous commands skip forward 30 seconds and back 15 seconds when supported by the headphones’ configuration.

Percentages use audio duration and your saved position. Blue means not started, orange means in progress and green means completed. A dash means duration is unavailable. Keep original copies of your files; the app has no independent backup service.

## Book details and privacy

Optional online lookup is off by default. Enable it in Settings to send title/author searches to Open Library. Offline playback and embedded chapter titles do not require it. Unmatched or ambiguous titles retain their local names. Covers use embedded artwork first, then a cover.jpg/cover.png transferred in the book folder, then a cached Open Library cover when available. Online cover retrieval follows the lookup setting; downloaded covers remain available offline. Read the [privacy policy](PRIVACY.md) for details.

## Connect Hardcover

Open Library → Settings → Connect Hardcover, then approve access in the browser. Settings shows the connected username and links to your Hardcover profile. Check connection verifies access; Disconnect Hardcover removes the saved connection and attempts to revoke access. If the service is unavailable during disconnect, remove Pocket Books from Hardcover’s Authorized Apps page.

Existing profile-only connections need Reconnect Hardcover to approve book access. Tap Find on Hardcover or the Hardcover status icon to search. The popup shows the top five results with titles and authors, plus the number shown. Tap the right book to save it and close the popup. Audiobooks are preferred automatically; no extra choices are needed. Done closes the popup at any time.

Matched books automatically send status and supported progress to the connected account after listening starts. Tap the Hardcover status on the book page and turn Sync reading progress off to stop updates; this choice survives reopening and rematching. The app uses the available book details to send progress. Where numeric progress is unavailable, it sends reading status and completion only. Sync runs while the app is open and catches up after offline listening; Sync now retries immediately. New online entries are private. Conflicting or further-ahead/finished reading progress stops sync with an explanation. There is no automatic reread or two-way position sync. Removing local audio never deletes the online entry. Use View on Hardcover to write a review there. Playback works without connecting. Development builds show a setup message until a Hardcover developer client ID is configured.

## Contact

Contact Lugo Labs at [support@lugolabs.com](mailto:support@lugolabs.com). Include the app version, iOS version, what you did and what happened.

You can also report a problem through [Pocket Books GitHub issues](https://github.com/lugolabs/PocketBooks-support/issues). Include the app version, iOS version, what you did and what happened. Issues are public: avoid personal audio, private filenames, account details or device identifiers.

With Look up book details enabled and Hardcover connected, ISBNs from Open Library automatically link unambiguous Hardcover books and download their covers. Audiobooks are preferred automatically. Use Change Hardcover match to choose a different book. Sync starts automatically after listening begins unless you turn it off for that book. Existing matches are preserved, and removing a match prevents automatic relinking. Missing/ambiguous ISBN matches remain available for manual search.

Starting playback also searches Hardcover directly using ISBNs when available, then title and author if needed. A confident match links automatically and syncs to your connected account; ambiguous matches need manual selection. This works without Open Library lookup. Per-book sync-off and manually removed matches are respected.

A compact sync symbol appears inside the library’s percentage ring, and beside the status in book details and the player. A green check means the current supported progress was acknowledged; orange indicates pending work or an error. Disconnected and disabled states are grey. Tap Hardcover needs attention to open book search; the Hardcover details screen also shows the error explanation. While playing, the icon can switch to pending until the next saved-progress update is sent.

Hardcover is ahead means its saved progress is later than your local position; updates wait for you to catch up. Marked Read on Hardcover means the book is marked Read online; the explanation on the book page shows why updates are paused. Both use grey status badges and preserve your online history. Selecting the same book again does not reset that history. Needs attention is reserved for other failures.

On the book page, tap the Hardcover status for sync controls, matching, publication information and the website link. The status itself opens the details screen; there is no separate link. Paused/waiting sync uses a clock symbol inside the Library percentage ring.
