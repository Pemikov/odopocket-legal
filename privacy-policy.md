---
title: OdoPocket Privacy Policy
---

# OdoPocket Privacy Policy

**Last updated: 22 November 2026**

OdoPocket ("the app", "we", "our") is a mileage and expense tracking app, built for tracking
business journeys and expenses for tax/expense claims. This policy explains what data the app
collects, why, where it's stored, who else sees it, how long it's kept, and what rights and
choices you have.

OdoPocket is currently developed and operated by a single independent developer ("the
developer"), not a company. For data protection purposes, the developer is the data controller.
Contact: **odopocket@gmail.com**.

## Summary

- Your journey, expense, receipt, and profile **content** is stored only on your own device —
  there is no OdoPocket server or cloud database for that content today, and we cannot see or
  recover it for you.
- The app uses your **location** (including in the background while auto-tracking is turned on)
  to automatically detect and log business journeys for mileage claims. Manual entry mode never
  uses background location.
- Creating an account (optional) is handled by **Firebase Authentication (Google)** — if you
  sign in with email/password or Google Sign-In, your email/name and sign-in credentials are
  stored by Google on our behalf, separately from your journey/expense content.
- We use **Firebase Crashlytics (Google)** to get crash and error reports so we can fix bugs.
  This is on by default and sends basic device/crash data to Google; you can turn it off at any
  time in Settings.
- **Google Maps Platform** (Maps, Directions, Roads, Places) and the device's own system
  geocoder are used to show maps, resolve addresses, and calculate routes/distances — this sends
  location coordinates to Google as a normal part of using those services, governed by
  [Google's own Privacy Policy](https://policies.google.com/privacy).
- We do not sell your data, and we do not use any advertising SDK or behavioural/marketing
  analytics. The only data sent off-device goes to the specific Google services listed in this
  policy, for the specific purposes listed.

## What we collect, and why

### Location data
The app requests fine, coarse, and (for auto-tracking) background location access, plus activity
recognition (to detect when you're driving) and Bluetooth (to detect connecting to a vehicle).
This is used to:
- Automatically detect when a drive starts and ends, and record the route/distance as a mileage
  entry for you to review.
- Show your current position and journey routes on the in-app map.
- Resolve addresses and business names near a location.

Background location only runs while auto-tracking is turned on in the app — it is never running
silently without your knowledge, and can be turned off entirely in favour of manual entry at any
time in Settings. Before Android's own background-location permission prompt appears, the app
explains in-app why the permission is being requested.

### Notification access (optional)
If you grant "Notification access" to help detect when a navigation app (Google Maps or Waze) is
actively guiding you, the app only checks which app owns an ongoing navigation notification — it
does not read the content/text of your notifications, and this is unrelated to any other
notifications on your device. This permission is optional and can be revoked at any time in
Android's own Settings > Apps > Special app access > Notification access.

### Photos (camera)
The app can capture photos of receipts (for expense claims), courier labels/serial numbers (for
the serial-scan feature), and odometer readings. Photos are processed on-device — including text
recognition and document-edge detection via Google's ML Kit, which runs on-device — and stored
locally with the associated expense/scan record. Photos are not uploaded anywhere by this
feature.

### Profile and journey data you enter
Name, employee number, cost centre, home address, vehicle details, customer/site names, journey
purposes, odometer readings, and expense amounts/categories — all typed or captured by you,
stored locally on your device.

### Account and sign-in data (optional)
Creating an OdoPocket account is optional — the app is fully usable without signing in. If you
choose to sign in (email/password or Google Sign-In) or enable two-factor authentication (TOTP),
this is handled by Firebase Authentication, a Google service. Depending on how you sign in, this
can include: your email address, display name, a Google account identifier/ID token, your
password (Google stores this hashed, we never see the plain password), and, if you enable 2FA, a
TOTP (authenticator-app) enrollment secret. This account/identity data is stored and managed by
Google on our behalf and is kept separate from your locally-stored journey and expense content.

### Crash and error reports
We use Firebase Crashlytics (Google) to automatically receive crash reports and error logs when
something goes wrong, so we can find and fix bugs. This includes crash stack traces, the app
version, your device model and OS version, and an anonymous installation identifier — it does not
include your journey, expense, or profile content. This is **on by default**; you can turn it off
at any time in Settings > Connection and data use > Crash & error reporting.

### Diagnostic logs
The app keeps a local, on-device log of auto-tracking activity (e.g. when a drive was detected,
connectivity/permission state) to help diagnose tracking issues. This log stays on your device
unless you explicitly choose to share/export it (e.g. to send to the developer for support), or
have turned on the optional "auto-send diagnostics when something looks wrong" setting, which is
off by default.

## Where your data lives

Your journey, expense, receipt, and profile **content** is stored in a local database on your
device. There is currently no OdoPocket server or cloud sync for that content — we do not have
access to it, cannot see it, and cannot recover it for you if your device is lost (you can create
your own backup/export file within the app).

If you create an account, your sign-in/identity data described above (email, sign-in credentials,
2FA enrollment) is stored by Firebase Authentication on Google's infrastructure, not on your
device and not on a server we operate ourselves.

**Coming in a future update**: we are building an optional cloud backup/sync feature for your
journey and expense content. It is not available yet, is off by default, and this policy will be
updated with full details — what's synced, where it's stored, and how to turn it off — before
that feature is released to any user.

## Third parties

- **Google Maps Platform** (Maps SDK, Directions API, Roads API, Places API) — receives location
  coordinates (and, for Places lookups, nearby-place queries) to provide mapping, routing, and
  address/business resolution.
- **Device's own system geocoder** — used for some address lookups; on most Android devices this
  is backed by a Google Play Services network geocoding service, even though it is not a direct
  call through our own Google Maps Platform key.
- **Google ML Kit** — on-device text recognition and document-edge detection for receipt/label
  photos. Processing happens on your device; the recognition model itself may be downloaded via
  Google Play Services the first time it's used.
- **Firebase Authentication (Google)** — only if you create an account or enable 2FA, as described
  above.
- **Firebase Crashlytics (Google)** — crash/error and basic device data, as described above,
  unless you turn it off.

All of the above are governed by [Google's Privacy Policy](https://policies.google.com/privacy).
We do not use any advertising SDK, and we do not use any behavioural/marketing analytics SDK. We
do not sell your data, and we do not share it with any other third party for their own marketing
or advertising purposes.

## How long we keep your data

- **Local content** (journeys, expenses, receipts, profile) — kept on your device until you
  delete it, delete your backup/export files, or uninstall the app.
- **Account/sign-in data** (if you create an account) — kept until you ask us to delete your
  account (see "Your choices" below).
- **Crash/error reports** — retained by Google under Firebase Crashlytics' own data-retention
  policy (historically around 90 days on Google's dashboard; see
  [Firebase's documentation](https://firebase.google.com/docs/crashlytics) for current details).
  We do not separately archive this data ourselves.
- **Diagnostic logs you choose to share** — kept only as long as needed to diagnose the issue you
  reported, then deleted.

## Legal basis for processing (UK/EU GDPR)

- Recording and showing your own journeys/expenses, and the location/camera access that requires:
  **performance of a contract** (providing the feature you're using) and, for background
  location specifically, your **explicit consent**, given through Android's own permission
  prompt after our in-app explanation — which you can withdraw at any time in Settings.
- Account creation and sign-in: **performance of a contract**, entered into when you choose to
  create an account.
- Crash reporting: our **legitimate interest** in keeping the app working correctly and fixing
  bugs, balanced against your right to opt out at any time (see above).

## International data transfers

Google's services (Maps Platform, ML Kit, Firebase Authentication, Firebase Crashlytics) may
process and store data outside your own country, including in the United States. Google provides
its own safeguards for these transfers (including the EU-US and UK-US data transfer frameworks
and standard contractual clauses) under its own privacy policy and terms. We do not otherwise
transfer your data internationally ourselves, since your core journey/expense content stays on
your device.

## Your choices

- **Auto-tracking is optional** — you can use the app in fully manual entry mode, in which case
  background location is never used.
- **Crash & error reporting can be turned off** at any time in Settings > Connection and data use
  > Crash & error reporting.
- **Notification access** (if granted) can be revoked at any time in Android's own system
  Settings.
- **Signing in is optional** — you can use all of the app's local features without creating an
  account.
- **Delete your local data**: uninstalling the app removes all locally stored journey, expense,
  receipt, and profile data from your device. Within the app, you can also delete individual
  records, or use Options > App & support > Backup & restore to manage/delete your data.
- **Delete your account**: if you've created an OdoPocket account, email
  odopocket@gmail.com to request deletion of your account and associated sign-in data
  (email, Google ID, 2FA enrollment) from Firebase. This does not delete your locally-stored
  journey/expense content, which stays on your device until you delete it separately.
- **Diagnostics sharing** is opt-in and can be turned off in Settings > Diagnostics at any time.

## Your privacy rights

**If you are in the UK or EEA**, you have the right to: access a copy of your data, correct it,
ask us to delete it, restrict or object to our processing, and (where processing is based on
consent) withdraw that consent at any time. You can exercise any of these rights by emailing
odopocket@gmail.com. You also have the right to complain to your local data protection authority
— in the UK, the [Information Commissioner's Office](https://ico.org.uk) — if you believe we
haven't handled your data properly.

**If you are a California resident**, you have the right to know what personal information we
collect, to request its deletion, and to request correction of inaccurate information, without
being discriminated against for exercising these rights. We do not sell personal information and
do not share it for cross-context behavioural advertising, so there is no "opt-out of sale/
sharing" link to provide. Requests can be made by emailing odopocket@gmail.com.

These rights apply equally to anyone, regardless of location — we handle all requests the same
way; the above simply names the specific legal rights that UK/EEA and California law guarantee.

## Security

Your local journey/expense/receipt data benefits from standard Android app-sandboxing (no other
app can read it), and you can additionally protect the app itself with a biometric/PIN app lock in
Settings. Account and crash data handled by Google (Firebase) are protected under Google's own
security standards for those services. No method of storage or transmission is 100% secure, but we
take reasonable steps appropriate to the data involved.

## Children

OdoPocket is a business expense/mileage tool, intended for adults carrying out business journeys
and expense claims. It is not directed at, and must not be knowingly used by, children under 16.
If you believe a child has provided us with personal data (e.g. via an account sign-in), contact
us at odopocket@gmail.com and we will delete it.

## Changes to this policy

If this policy changes, the "Last updated" date above will be revised and, for material changes
(for example, when cloud sync becomes available), we will also note the change within the app.

## Contact

Questions about this policy, or to exercise any of the rights above: **odopocket@gmail.com**.
