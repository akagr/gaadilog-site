---
layout: page
title: Privacy Policy
permalink: /privacy-policy/
---

**Effective date**: 2026-05-05
**App**: GaadiLog (`me.akashagrawal.gaadilog`)
**Developer**: Akash Agrawal
**Contact**: akagr@outlook.com

This is a short, plain-English description of how GaadiLog handles your data. There is no legalese boilerplate because there is no data collection to describe in legalese.

## What we collect

**Nothing.**

GaadiLog stores everything you log — vehicles, fuel-ups, services, documents, reminders, photos — only on your device. We do not have a server. We do not have an account system. There is no sign-up, no login, no cloud sync, no backup to our infrastructure, and no way for us to read what you log even if we wanted to.

## What permissions we ask for, and why

| Permission | Why we ask | What we do with it |
|---|---|---|
| Camera (iOS + Android) | To photograph your vehicle, service invoices, and document scans (RC, insurance, PUC) directly from inside the app | The image is saved into the app's private storage on your device. It is not uploaded anywhere. |
| Photo library (iOS + Android) | To attach photos you already have (e.g., existing invoice scans) to a service or document record | The image is copied into the app's private storage. The original in your library is unchanged. |
| Notifications (iOS + Android) | To remind you when a document is about to expire, or when a service interval is due | All reminder scheduling happens on your device via the operating system's local-notification system. No push servers are involved. |
| Receive boot completed (Android only) | To re-arm your scheduled reminders after you reboot your phone | We do not run any background work other than re-scheduling the reminders you already set up. |

## What we share

Nothing. There is no third-party analytics SDK, no crash-reporting SDK, no advertising SDK, no tracking pixel, no telemetry of any kind in the app. The app's only network use is downloading the Material 3 system fonts via Flutter's standard rendering — and only if your device hasn't cached them already.

## Where your data lives

In the app's private storage on your device, in a SQLite database file. Specifically:

- iOS: in the app's container directory, accessible only to GaadiLog itself and to iOS system tools.
- Android: in the app's internal storage directory, accessible only to GaadiLog itself.

If you delete the app, this data is deleted along with it. There is no remote copy.

## Export

You can export your data at any time as CSV (per vehicle, or for all vehicles) and as PDF (a per-vehicle service-history report). The OS share sheet then hands the file to whichever app you choose. Once it leaves GaadiLog's share sheet, the receiving app's privacy policy applies — not ours.

## Children

GaadiLog has no age gate because it does not collect personal information from anyone. The Indian-market context (the primary target audience) means most users will be adults registering vehicles, but there is nothing in the app that identifies, tracks, or profiles users of any age.

## Changes to this policy

If the policy changes — for example, when v1.1 ships cloud sync as an opt-in feature — the new version will appear at the same URL with an updated "Effective date". Material changes (anything that affects what data leaves your device) will also surface in-app the next time you open it.

## Contact

Questions, concerns, or notice of any kind: **akagr@outlook.com**.