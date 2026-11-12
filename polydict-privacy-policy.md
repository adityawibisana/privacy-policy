# PolyDict Privacy Policy

Last updated: 12 November 2026

PolyDict is an offline dictionary and translator for Android. This policy explains what happens to the information you use in the app.

## No account, no ads

PolyDict has no user accounts, no sign-in and no advertising. The developer does not run a server. The only data the developer receives is the anonymous crash reports and usage statistics described below.

## What is stored on your device

The following is stored only in the app's private storage on your device:

- Translations of words and phrases you looked up, so that they work offline later.
- Dictionary details (meanings, grammar, examples) fetched for those words.
- How often you chose each source language by hand. Only language codes and counts are stored, not the text you typed.
- Your settings, such as the target language and whether offline packs download over Wi-Fi only.

You can remove all of this by clearing the app's storage in Android settings or by uninstalling the app.

## What is sent over the internet

PolyDict uses the internet only for the following:

1. **Dictionary details and language suggestions.** When you look up a word that is not saved yet and your device is online, the word (or its translation) is sent to the services below. When the app can't tell on the device which language a word is in, the word is also sent to Google Translate and Wiktionary to suggest languages.
   - **kaikki.org**, which serves Wiktionary data. See the [kaikki.org website](https://kaikki.org) for its terms.
   - **Google Translate** (`translate.googleapis.com`), to get definitions and examples, and to suggest the language of a word the app can't identify on the device. See the [Google Privacy Policy](https://policies.google.com/privacy).
   - **Wiktionary** (`en.wiktionary.org`), to suggest the language of a word the app can't identify on the device. See the [Wikimedia Foundation Privacy Policy](https://foundation.wikimedia.org/wiki/Policy:Privacy_policy).

   These requests contain the word and its language, plus the standard information any internet request includes, such as your IP address. They do not contain an account, a name or a device identifier from PolyDict.

2. **Offline language packs.** Translation models are downloaded from Google when you choose to install a language.

3. **Crash reports and usage statistics.** PolyDict uses Google Firebase Crashlytics and Google Analytics for Firebase to find bugs and understand which features are used:
   - **Crash reports** contain the error, the state of the app when it crashed, the device model, the Android version and the app version.
   - **Usage statistics** record events such as "a lookup finished", "a source language was picked by hand" and "an offline language pack was downloaded". These events contain only language codes (for example `de` or `en`) and whether the action succeeded. Firebase also records standard information such as app opens, session length, the device model, the Android version, the country, and an app instance ID.

   **The words you type, their translations and dictionary details are never included.** This data is processed by Google on the developer's behalf. See [Firebase privacy and security](https://firebase.google.com/support/privacy) and the [Google Privacy Policy](https://policies.google.com/privacy).

Translation and language detection run on your device with Google ML Kit. The text you type is not sent anywhere for translation, and it is sent for language detection only in the case described in item 1. ML Kit may send Google limited technical information, such as the device model, the Android version, the app version and performance metrics, to keep the service working. See the [ML Kit terms](https://developers.google.com/ml-kit/terms) for details.

## Children

PolyDict is not directed at children under 13 and does not knowingly collect personal information from anyone.

## Changes

If this policy changes, the new version will be published at this address with a new date.

## Contact

Questions about this policy: aditya.wibisana@gmail.com
