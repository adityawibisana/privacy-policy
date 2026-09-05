# Privacy Policy — Enough

**App:** Enough (`com.aw.enough`)
**Developer:** Aditya Wibisana
**Contact:** aditya.wibisana@gmail.com
**Last updated:** 5 September 2026

Enough helps you set daily time limits on apps you choose and blocks them once the
limit is spent. This policy explains what the app touches, what leaves your device,
and what does not.

## Summary

- Enough has **no account, no login, and no server of its own**. Your limits and usage
  figures stay on your device.
- The app **does not sell or share your personal data** with third parties for
  advertising, and it contains no ad SDKs.
- The only data that leaves the device is **anonymous crash and product-analytics data**
  sent to Google Firebase, described below.

## Information the app handles on your device

**App usage statistics.** With the "Usage access" permission
(`PACKAGE_USAGE_STATS`), Enough reads Android's per-app foreground time
(`UsageStatsManager`) about once a minute to know how long you have used each limited
app today. These figures are read on the device and are not uploaded.

**The list of apps installed on your device.** The `QUERY_ALL_PACKAGES` permission lets
the app show you a picker of launchable apps so you can choose which ones to limit. The
full list is not uploaded.

**Your limits.** The apps you limit and the minutes you allow each one are stored in a
local DataStore file
(`files/datastore/screen_time.preferences_pb`). If you have Android
Backup enabled, Android may include this file in your own Google account backup, under
Google's control and your device's backup settings — see `backup_rules.xml` and
`data_extraction_rules.xml` in the app.

Uninstalling Enough removes this local data from the device.

## Information sent off the device

**Crash reports — Firebase Crashlytics.** When the app crashes, a report is sent
containing the stack trace, device model, OS version, app version, and a randomly
generated installation identifier. It does not contain your app list or your limits.

**Product analytics — Google Analytics for Firebase.** Enough records a small,
fixed set of events so the developer can tell whether the app works:

| Event / property | What it contains |
| --- | --- |
| `app_limited` | The package name and display name of the app you limited, the limit in minutes, whether the limit is new, and the packages currently under a limit (truncated) plus their count |
| `app_blocked` | The package name and display name of an app whose limit ran out, and the packages currently under a limit (truncated) plus their count |
| `perm_*` user properties | Whether each permission (usage access, display over other apps, ignore battery optimization, notifications) has been granted |

These events carry **no name, email address, phone number, contacts, location, message
content, or browsing history**. They are tied only to the anonymous Firebase
installation identifier, not to you. Note that the package names above are names of
apps you chose to limit — for example `com.instagram.android` — which may indirectly
reveal which apps you use.

Analytics and crash collection are **disabled entirely in debug builds** of the app.

Firebase processes this data on Google's infrastructure as a service provider. See
Google's privacy policy: https://policies.google.com/privacy and Firebase's data
disclosure: https://firebase.google.com/support/privacy

## Permissions and why they are needed

| Permission | Why |
| --- | --- |
| Usage access (`PACKAGE_USAGE_STATS`) | Measure how long you have used each limited app today |
| Query all packages (`QUERY_ALL_PACKAGES`) | List installed apps so you can pick which to limit |
| Display over other apps (`SYSTEM_ALERT_WINDOW`) | Draw the blocking screen over an app that has hit its limit |
| Ignore battery optimization | Keep the once-a-minute check running while the device is idle |
| Foreground service | Keep the enforcement service alive between checks |
| Notifications | Show the required foreground-service notification |
| Receive boot completed | Restart enforcement after a reboot or app update |

Enough does not use the camera, microphone, location, contacts, SMS, or call logs.

## Data retention and deletion

Local data lives on your device until you remove a limit or uninstall the app.
Firebase Crashlytics retains crash reports for up to 90 days; Analytics event data is
retained according to the project's Firebase retention setting (default 2 months for
user-level data). To request deletion of analytics or crash data associated with your
installation, email aditya.wibisana@gmail.com with your request; because the data is
keyed to an anonymous installation identifier, please include the approximate date and
device model so it can be located. You can also stop all future collection by
uninstalling the app.

## Children

Enough is not directed at children under 13 and does not knowingly collect personal
information from them.

## Your rights

Depending on where you live (for example the EEA/UK under the GDPR, or California under
the CCPA/CPRA), you may have the right to access, correct, delete, or object to the
processing of your personal data. Because Enough holds no account data, most such
requests concern the Firebase data above; write to aditya.wibisana@gmail.com and it will
be handled within 30 days. Enough does not sell or share personal information as those
terms are defined by the CCPA/CPRA.

## Changes to this policy

If this policy changes, the "Last updated" date above changes with it, and a material
change will be noted in the app's Play Store release notes.

## Contact

Questions about this policy: **aditya.wibisana@gmail.com**
