# Remote Camera Privacy Policy

Last updated: 19 November 2026

Remote Camera lets a Zepp OS watch control the camera of an Android phone. This policy explains what happens to the information the app uses.

## No account, no ads, no server

Remote Camera has no user accounts, no sign-in and no advertising. The developer does not run a server and receives no data from the app: no analytics, no crash reports, no usage statistics.

## How the watch reaches the phone

The watch app talks to the Zepp app on your phone over Bluetooth. The Zepp app passes the watch's commands to Remote Camera through a local connection on the phone itself (`127.0.0.1`). This connection cannot be reached from the internet or from other devices, and it is protected by a token that the watch and the phone agree on when they pair.

Remote Camera does not send anything to the internet.

## Camera and photos

- **Our Camera mode** uses the phone's camera. Photos are saved on your phone in `DCIM/RemoteCamera`.
- **Stock Camera mode** uses your phone's own camera app. Photos are saved by that app as usual.

Remote Camera does not upload, copy or read your photos.

## Watch preview

When you open the preview page on your watch, the app makes a small, low-resolution picture of the camera view about once a second and sends it to your watch through the Zepp app. These pictures are not stored and are not sent anywhere else.

## Accessibility service (Stock Camera mode)

In Stock Camera mode, and only after you agree and turn it on, Remote Camera uses the Android Accessibility Service API to:

- check which app is in front, to know whether the camera app is open;
- press the shutter button inside the camera app when you tap your watch;
- on Android 11 and newer, take screenshots while the camera app is in front, to show the preview on your watch.

The service does not read, click or capture anything in other apps. Nothing it sees is stored, collected or shared. Screenshots go only to your watch, as described under "Watch preview". You can turn the service off at any time in Android Settings → Accessibility.

## What is stored on your phone

The following is stored only in the app's private storage:

- your settings, such as the camera mode and the camera's shutter position from calibration;
- the pairing token for your watch;
- when the watch last connected and when the last photo was taken, to show setup progress.

You can remove all of this by clearing the app's storage in Android settings or by uninstalling the app.

## Children

Remote Camera is not directed at children under 13 and does not knowingly collect personal information from anyone.

## Changes

If this policy changes, the new version will be published at this address with a new date.

## Contact

Questions about this policy: aditya.wibisana@gmail.com
