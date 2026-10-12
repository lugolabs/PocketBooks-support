# Pocket Books privacy policy

Updated 12 October 2026.

Pocket Books is developed by Lugo Labs and plays audio files you provide. Account connection is optional. It has no advertising or analytics SDK. The app does not upload your audio to us.

## Information on your device

Your audio files, filenames, library details, chapter titles, listening positions, bookmarks and preferences are stored in the app’s container on your iPhone. The app reads file sizes and modification times to detect completed transfers. These file timestamps are not included in metadata searches.

Your device’s backup settings may include app data in an Apple or computer backup. We do not operate a cloud-sync service for your library.

## Optional book details lookup

Online lookup is off by default. If you enable Look up book details in Settings, the app sends the book title and author name to Open Library at openlibrary.org to find matching catalog information. These names may come from your filenames or existing book details. For matched books, requests can also include the Open Library book identifier. The app can request cover images from covers.openlibrary.org using a cover identifier, and save them on your device for offline display. Embedded artwork and cover images transferred with your audio are read locally. Requests also expose your IP address and standard network request information to that service.

The app does not include your audio, listening position, bookmarks, account information or a unique device identifier in the search request. It does not sign in to Open Library. Returned catalog details and the last successful check time are saved on your device.

Open Library is operated by the Internet Archive. Its handling of requests is governed by its [terms and privacy policy](https://archive.org/about/terms). Do not enable lookup for titles you do not want to send to that service.

## Optional Hardcover connection

If you choose Connect Hardcover, sign-in and consent take place through Hardcover in a secure browser session. Pocket Books requests permission to read your profile, search the catalog, read your library and update your reading list. Updates require a separate opt-in for each matched book. It saves those details and access/refresh tokens in this iPhone’s Keychain so the connection can be restored. Tokens are restricted to this device and are not stored in the audio library or sent to Lugo Labs. Your password is entered only on Hardcover.

Hardcover receives authenticated profile and catalog requests, search terms you submit, Open Library ISBNs used for automatic matching when online lookup is enabled, selected book/edition identifiers, token exchanges, your IP address and standard network information. Matching a book saves its catalog details locally and can download a cover from assets.hardcover.app for offline display. Its handling is governed by [Hardcover’s policies](https://hardcover.app/pages/policies).

If you enable Sync reading progress for a matched audiobook, Pocket Books reads that book’s entry in your Hardcover library and sends its listening progress, reading status and completion date. Progress is sent as seconds or approximate pages for the selected edition; without an edition, only status and completion are sent. New online entries are created privately; existing entries keep their privacy settings. The app sends updates while open and retries after offline listening when reopened. Audio files, local bookmarks and reviews are not uploaded. Turning sync off stops future updates, but cannot undo requests already received. Deleting a local book does not delete its Hardcover library entry.

Disconnect Hardcover removes the connection from this iPhone and attempts to revoke its refresh token online. If revocation cannot be confirmed, the app tells you to remove Pocket Books from Hardcover’s [Authorized Apps](https://hardcover.app/account/api/authorized-apps). Keychain credentials can survive deleting the app; disconnect before uninstalling or revoke access on Hardcover. Disconnecting does not delete your Hardcover account or library.

## Your choices and deletion

You can turn lookup off at any time in Settings. This stops future requests and cancels a lookup in progress; it cannot undo a request already received by Open Library. Previously retrieved details remain on your device.

You can delete a book in the app or remove its shared files through Finder. In-app deletion also removes the transferred file or whole folder after confirmation. If deletion cleanup fails, remaining audio is kept in private app storage and cleanup retries when the app reopens. Removing the app deletes its local container. Backups are managed separately through your device or computer settings. Keep your own copies of audio you want to retain.

## Support and external links

Opening privacy, support or service links in a browser sends a normal web request to the destination. GitHub hosts this policy and the support page, under [GitHub’s privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

For privacy questions or support, email [support@lugolabs.com](mailto:support@lugolabs.com) or use the [support page](SUPPORT.md). Messages you send may include your email address and the details you choose to provide. We use those messages to respond and resolve your request; do not send personal audio or other sensitive information. Include only information you want to share. Public GitHub issues are visible to others; do not upload personal audio, private filenames, account details or device identifiers.

## Updates

This policy will be updated when the app’s data handling changes. The date above identifies the current version.
