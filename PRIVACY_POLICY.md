# OmniPose Fit privacy note

Last updated: October 10, 2026. Applies to the sideload APKs in this repository (package `com.grloepr.pushtrack`). This is a plain-language description, not a store-approved policy.

- **Camera:** with your permission, the app uses the camera to estimate body landmarks during a training session. App code does not record, store or upload camera video or images. Frames are processed on your device by Google's bundled ML Kit pose detector.
- **Network:** the app has no account system, ads, billing, or developer-operated analytics or server. However, its manifest declares `INTERNET` and `ACCESS_NETWORK_STATE`, added by the Google ML Kit / Google Play services libraries. Per Google's ML Kit documentation, these libraries can contact Google for compatibility/model information and send API performance and usage metrics. Camera input and pose outputs are not sent by ML Kit. See [Google's ML Kit data disclosure](https://developers.google.com/ml-kit/android-data-disclosure).
- **Local data:** skill progression and settings (such as the audio mute) are stored in Android shared preferences on your device. Android backup is enabled for the app, so your device's backup settings may retain this data. Uninstalling or clearing app data removes the local copy.
- **Controls:** revoke camera access in Android settings at any time.
- **Questions or requests:** use the [issue tracker](https://github.com/grloper/OmniPose-Fit-releases/issues). There is no developer-hosted account to erase.
