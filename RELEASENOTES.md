# Release notes

### 3.1.7 [Apr  01, 2025]

This release aligns with version 2.1.7 and includes the following updates:

* Added `onPlaybackSpeedChange` callback in `TPStreamPlayerListener`.
* Refactored and optimized code for better performance and maintainability.

### 3.1.6 [Mar  28, 2025]

This release aligns with version 2.1.6 and includes the following updates:

* Optimized offline DRM license fetching.
* Fixed an issue with access token reauthentication for offline DRM licenses.
* Refactored and optimized code for better performance and maintainability.

### 3.1.5 [Mar  19, 2025]

This release aligns with version 2.1.5 and includes the following updates:

* Updated Sentry DNS value.
* Improved Player Control view UI.
* Fixed Night theme issues in the Resolution selection sheet and Download selection sheet.
* Fixed player detachment when releasing to prevent conflicts and ensure clean reinitialization.
* Optimized and refactored code for better performance and maintainability.

### 3.1.4 [Feb  28, 2025]

This release aligns with version 2.1.4 and includes the following updates:

* Fixed an issue with reauthentication of the access token in `onAccessTokenExpired`.
* Add deprecated `onDeviceInfoChanged()` in `TPStreamPlayerListener`.
* Add deprecated `onVideoSizeChanged()` in `TPStreamPlayerListener`.
* Add deprecated `onPositionDiscontinuity()` in `TPStreamPlayerListener`.
* Add deprecated `onTimelineChanged()` in `TPStreamPlayerListener`.
* Optimized and refactored code for improved performance and maintainability.

### 3.1.3 [Feb  07, 2025]

This release aligns with version 2.1.3 and includes the following updates:

* Improved error messages to be more user-friendly.
* Enabled asynchronous buffer queueing to reduce dropped frames and audio underruns.
* Optimized and refactored code for improved performance and maintainability.

### 3.1.2 [Oct  18, 2024]

This release aligns with version 2.1.2 and includes the following updates:

* Added support for H.265 video codec.
* Optimized and refactored code for improved performance and maintainability.

### 3.1.1 [Oct  03, 2024]

This release aligns with version 2.1.1 and includes the following updates:

* Resolved incorrect media size display in the download selection sheet.
* Added validation to prevent crashes during repeated player initialization.
* Optimized and refactored code for improved performance and maintainability.

### 3.1.0 [Sep  23, 2024]

This release aligns with version 2.1.0 and includes the following updates:

* Added 1.75x playback speed option in the player.
* Available resolution and playback speed are displayed based on device capabilities.
* Enabled secure screen for L3 devices during DRM video playback via `TpStreamPlayerFragment.enableSecureView()`.
* Introduced the option to enable software decoding using `TpStreamPlayerFragment.useSoftwareDecoder()`.
* Optimized and refactored code for better performance and maintainability.

### 3.0.24 [Aug  13, 2024]

This release aligns with version 2.0.24 and includes the following updates:

* Playback Initial Resolution: Introduced the ability to set the initial playback resolution when configuring TpInitParams.
* Code Improvements: Optimized and refactored code for better performance and maintainability.

### 3.0.23 [Aug  06, 2024]

This release corresponds to the 2.0.23

* Fixed issue with renewing offline DRM licenses only if they are expired.
* Display player error codes instead of custom codes for player errors.
* Added the option to set `userId` when building `TpInitParams`.
* Added Sentry log with a custom object.
* Removed the default implementation of the `onAccessTokenExpired` callback in `TPStreamPlayerListener`.
* Fixed video playback issues on Android 7.0 or earlier.
* Code optimization and refactoring.

### 3.0.22 [Jul  20, 2024]

This release corresponds to the 2.0.22

* Added `onAccessTokenExpired` callback in `TPStreamPlayerListener`.
* Fixed issue where the download button did not appear for completed livestreams.
* Improved error messages to be more user-friendly.
* Resolved crash issue related to renewing offline DRM licenses.
* Added an option to set the offline license expiration time when building `TpInitParams`.
* Code optimization and refactoring.

### 3.0.21 [Jul  15, 2024]

This release corresponds to the 2.0.21

* Added validation to ensure `videoId` and `accessToken` are neither null nor empty.
* Fixed a NullPointerException that occurred when updating the download button image.
* Introduced an API to start downloads in `TpStreamDownloadManager`.
* Displayed appropriate notice messages according to the livestream status.
* Optimized and refactored code.

### 3.0.20 [Jul  03, 2024]

This release corresponds to the 2.0.20

* Added permission for foregroundServiceType in the manifest.
* Added validation for `TpInitParams` before playing downloaded videos.
* Code optimization and refactoring.

### 3.0.19 [Jun  19, 2024]

This release corresponds to the 2.0.19

* Updated the compile and target SDK versions to 33.
* Fixed order changing issue in downloaded assets.
* Added option to store metadata with the download asset.
* Added folderTree field in Asset model to fetch the video folder path.
* Code optimization and refactoring.

### 3.0.18 [Jun  10, 2024]

This release corresponds to the 2.0.18

* Added `getDownloadAsset()` method in `TpStreamDownloadManager` to fetch a single download asset.
* Added `showFullscreenButton()` and `hideFullscreenButton()` methods in TPStreamPlayerView.
* Code optimisation and refactoring.

### 3.0.17b [Apr  15, 2024]

This release corresponds to the 2.0.17b

* Moved `com.tpstream.player.enum.PlaybackError` to `com.tpstream.player.constants.PlaybackError`.
* Removed deprecated `onMetadata()` method from `TPStreamPlayerListener`.
* Removed deprecated `onPlayerErrorChanged()` method from `TPStreamPlayerListener`.
* Added subtitle support.

### 3.0.16b [Apr  04, 2024]

This release corresponds to the 2.0.16b

* Added `setPreferredExitFullscreenOrientation` to specify preferred orientation upon exiting fullscreen mode.

### 3.0.15b [Feb  26, 2024]

This release corresponds to the 2.0.15b

* Introduced support for Livestream.
* Introduced a new Asset class and incorporated the existing Video class as an attribute within the Asset.
* Download callbacks will take the Asset object as an argument instead of a Video.
* Conducted code optimization, refactoring, and miscellaneous bug fixes.

### 3.0.14b [Jan  31, 2024]

This release corresponds to the 2.0.14b

* Fix resolution not listing in advance resolution sheet

### 3.0.13b [Jan  6, 2024]

This release corresponds to the 2.0.13b

* Add consumer rules to avoid removal of essential libraries.

### 3.0.12b [Dec  29, 2023]

This release corresponds to the 2.0.12b

* Add `getPlayWhenReady()` and `setPlayWhenReady()` in `TpStreamsPlayer`.
* Add deprecated `onMetadata()` in `TPStreamPlayerListener`.
* Add deprecated `onPlayerErrorChanged()` in `TPStreamPlayerListener`.

### 3.0.11b [Dec  14, 2023]

This release corresponds to the 2.0.11b

* Fix Fragment Attachment Check in `onPlaybackError()`.

### 3.0.10b [Dec  13, 2023]

This release corresponds to the 2.0.10b

* Fix Error message displayed when player is loading.
* Changed user-friendly error messages on player errors.

### 3.0.9b [Dec  13, 2023]

This release corresponds to the 2.0.9b

* Add `showErrorMessage()` in `TPStreamPlayerView` to show the custom error message on the player view.

### 3.0.8b [Dec  11, 2023]

This release corresponds to the 2.0.8b

* Add `getPlayBackSpeed()` in `TpStreamsPlayer`.
* Resolve WindowLeaked exception in `TpStreamPlayerFragment`.

### 3.0.7b [Dec  6, 2023]

This release corresponds to the 2.0.7b

* Fix App not responding after the video buffer end when device has no Internet connection.

### 3.0.6b [Dec  6, 2023]

This release corresponds to the 2.0.6b

* Code optimisation and refactoring.

### 3.0.5b [Dec  1, 2023]

This release corresponds to the 2.0.5b

* Add `getMaxResolution()` and `setMaxResolution()` in `TpStreamsPlayer` to restrict the maximum playback resolution.
* Fix Playback speed button UI in `TPStreamPlayerView`.

### 3.0.4b [Nov 29, 2023]

This release corresponds to the 2.0.4b

* Add `setMaxVideoSize()` in `TpStreamsPlayer` to restrict the playback video size

### 3.0.3b [Nov 23, 2023]

This release corresponds to the 2.0.3b

* Add support to change seek bar color in `TPStreamPlayerView`.
* Move `TpStreamsPlayer.TPStreamPlayerListener` to `TPStreamPlayerListener`
* Add new `PlaybackError`.
* Add `onPlayerError(playbackError: PlaybackError)` as a replacement for `onPlayerError(error: PlaybackException)`.
* Code optimisation and refactoring.

### 3.0.2b [Nov 21, 2023]

This release corresponds to the 2.0.2b

* Add `showFullScreen()` and `exitFullScreen()` APIs in the `TpStreamPlayerFragment` to programmatically control fullscreen mode.
* Add `onFullScreenChanged()` callback event in `TPStreamPlayerListener`.
* Add sentry error log with playerId tag.
* Add option set custom time for seek forward and seek backward.
* Code optimisation and refactoring.

### 3.0.1b [Nov 17, 2023]

This release corresponds to the 2.0.1b

* Upgraded media3 dependency to 1.1.1.
* Code optimisation and refactoring.

### 2.0.0 [Nov 2, 2023]

* Add new `TPStreamsSDK`.
* Remove `orgCode` param in `TpInitParams`.
* Code optimisation and refactoring.

### 1.0.14b [Jul 25, 2023]

* Add `TpStreamPlayer.load()` as a replacement for `TpStreamPlayerFragment.load()`. The load method in fragment will be deprecated in the next release.
* Added `play()` and `pause()` APIs in the `TpStreamsPlayer` to programmatically control the playback.
* Add new `TPStreamPlayerView`.
* Add support to Enable and Disable seekBar in `TPStreamPlayerView`.
* Add support to show and hide fast forward button and rewind button in `TPStreamPlayerView`.
* Fix Night theme in Resolution selection sheet and Download selection sheet.
* Fix duplicate resolution names in Resolution selection sheet.
* Upgraded media3 dependency to 1.0.2.
* Add Marker support in `TPStreamPlayerView`.
* Move `com.tpstream.player.TpStreamPlayerFragment` to `com.tpstream.player.ui.TpStreamPlayerFragment`.
* Move `com.tpstream.player.models.Video` to `com.tpstream.player.data.Video`.
* Move `com.tpstream.player.TpStreamDownloadManager` to `com.tpstream.player.offline.TpStreamDownloadManager`.
* Move `com.tpstream.player.models.DownloadStatus` to `com.tpstream.player.data.source.local.DownloadStatus`.
* Move `com.tpstream.player.InitializationListener` to `com.tpstream.player.ui.InitializationListener`.
* Code optimisation and refactoring.

### 1.0.13b [Mar 14, 2023]

*   Remove playerFragment.playbackStateListener. Use player.setListener(TPStreamPlayerListener) instead.
*   Rename TPPlayerListener to TPStreamPlayerListener.
*   Rename OfflineVideoState to DownloadStatus.
*   Rename OfflineVideoInfo to Video.
*   Code optimisation and refactoring.

### 1.0.12b [Feb 10, 2023]

*   Fix stop background music when the video starts playing.
*   Fix app crash when turning off the internet while downloading video.
*   Refactor.

### 1.0.11b [Feb 4, 2023]

*   Add sentry error logs.
*   Misc bug fixes.
*   Refactor.

### 1.0.10b [Jan 23, 2023]

*   Fix not able to replace expired DRM license key.
*   Fix not able to download single track in non-DRM videos.
*   Fix AES encrypted video not downloading.

### 1.0.9b [Dec 29, 2022]

*   Fix not able to download AES encrypted video.

### 1.0.8b [Dec 23, 2022]

*   Fix video not playing after minimize and reopening the app.
*   Fix non-DRM video is not getting downloaded.
*   Refactor.

### 1.0.7b [Dec 20, 2022]

*   Misc bug fixes.

### 1.0.5b [Dec 17, 2022]

*   Added Event Listener to player.

### 1.0.4b [Dec 12, 2022]

*   Misc bug fixes.

### 1.0.2b [Dec 7, 2022]

*   Added support for AES encrypted video.

### 1.0.1b [Dec 6, 2022]

*   Added support to change resolution for video.
*   Added support to full screen.

### 1.0.0b

*   No notes provided.