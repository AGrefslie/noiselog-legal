---
title: NoiseLog Privacy Policy
permalink: /privacy
---

# NoiseLog Privacy Policy

*Last updated: 2026-05-28*

NoiseLog is an **offline-first** noise-incident logging app. This policy explains
what the app collects, where it lives, and what (if anything) leaves your device.

## 1. Short version

- Every incident you log — date, time, decibel level, note, photo, audio,
  location — is stored **only on your device** in a local SQLite database.
- We do **not** operate any servers. There is no NoiseLog account.
  Nothing is uploaded to us.
- The app uses three OS-level services that you can decline at any time:
  microphone (decibel capture), camera / photo library (evidence photos),
  and location (incident geo-tag).
- If you choose to share a PDF report, CSV, or JSON export, *you* decide who
  receives it via your device's share sheet.

## 2. What the app stores locally

| Data | Where | Why |
|------|-------|-----|
| Incident metadata (date, time, dB, category, note) | On-device SQLite database | The case log |
| Photos attached as evidence | On-device file storage (`documentDirectory/photos/`) | The case log |
| Audio recordings | On-device file storage (`documentDirectory/audio/`) | The case log |
| Latitude / longitude / accuracy / reverse-geocoded street label | On-device SQLite database | Incident location tag (Pro feature, opt-in) |
| Case files (name, property, reporter, case number) | On-device SQLite database | Organising incidents |
| Generated PDF reports | On-device file storage (`documentDirectory/reports/`) | The report vault |
| App settings (theme, quiet hours, Pro unlock status) | On-device SQLite settings table | Personalisation |

**None of the above is transmitted to NoiseLog or any third party.**

## 3. Permissions we request

The app asks for these OS permissions only at the moment the feature is used:

- **Microphone** — to measure decibel levels while recording an incident.
- **Camera / Photo library** — to attach a photo as evidence (Pro only).
- **Location (when-in-use)** — to geo-tag the incident as evidence (Pro,
  opt-in via Settings).

You can revoke any of these at any time in your device's system settings.
The app continues to work without them; the corresponding feature is simply
disabled.

## 4. In-app purchases

NoiseLog Pro is a one-time, non-consumable purchase processed by Apple's
App Store or Google Play Billing. **We never see your payment information.**
Purchase verification happens entirely between your device and the platform
store. After a successful purchase, only a local flag (`pro_unlocked = true`)
is written to your device.

## 5. Crash reporting

If a crash reporter is configured for a release, the app may send anonymous
crash diagnostics (stack trace, app version, OS version) to **Sentry** to help
us fix bugs. We strip personally identifying information automatically
(`sendDefaultPii: false`). No incident data, case data, location, audio,
photos, or notes are ever included in crash reports.

Crash reporting is fully disabled when no DSN is configured.

## 6. Sharing data *you* initiate

When you export a PDF / CSV / JSON or share an audio recording, the app
opens your device's standard share sheet. *You* choose the destination
(email, messaging app, file storage, etc.). NoiseLog has no part in that
transmission and keeps no record of it.

## 7. Children

NoiseLog is not directed at children under 13 and does not knowingly collect
data from them. As the app is fully offline and account-less, no data
collection occurs regardless of the user's age.

## 8. Data retention & deletion

You can delete any incident from its detail screen, bulk-delete from the
Records screen, or wipe the entire local database via **Settings → Data →
Delete all data**. Uninstalling the app removes every stored byte.

We retain nothing because we have nothing to retain.

## 9. Changes to this policy

If we change this policy in a way that materially affects you, we will update
the "Last updated" date above and surface the change in the app on next launch.

## 10. Contact

Questions or requests:
**axel.grefslie@obos.no**
