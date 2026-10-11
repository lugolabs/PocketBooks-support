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

Optional online lookup is off by default. Enable it in Settings to send title/author searches to Open Library. Offline playback and embedded chapter titles do not require it. Unmatched or ambiguous titles retain their local names. Read the [privacy policy](PRIVACY.md) for details.

## Contact

Contact Lugo Labs at [support@lugolabs.com](mailto:support@lugolabs.com). Include the app version, iOS version, what you did and what happened.

You can also report a problem through [Pocket Books GitHub issues](https://github.com/lugolabs/PocketBooks-support/issues). Include the app version, iOS version, what you did and what happened. Issues are public: avoid personal audio, private filenames, account details or device identifiers.
