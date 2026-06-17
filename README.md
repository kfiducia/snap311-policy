# Snap311 Privacy Policy

_Last updated: June 16, 2026_

Snap311 ("the app") is an independent, unofficial mobile client for filing
service requests with the District of Columbia 311 system. The app is not
affiliated with or endorsed by the DC Office of Unified Communications or any
DC government agency.

## What we collect

Snap311 collects only what's needed to file a service request and to make the
app work reliably:

- **Contact info you enter** (first/last name, email or phone). Stored locally
  on your device using iOS encrypted storage. Sent to DC's official 311 API at
  `dc311-api.herokuapp.com` only when you submit a report.
- **Address and location data** for the report you're filing. Extracted from
  the GPS in your chosen photo's EXIF metadata, or typed by you, or picked on
  a map. Sent to DC's 311 API as part of the report.
- **Photos you choose to attach.** Uploaded to DC's official 311 worker at
  `dc311-api-worker.herokuapp.com`, which stores them in DC's Salesforce
  system as part of the service request.
- **Diagnostic / crash reports** (optional, can be disabled). Sentry SDK
  events about errors and slow API calls, scrubbed of API keys and personal
  data. Used only to fix bugs. You can disable this in **Settings → Send
  diagnostics**.

## What we do NOT collect

- We do not track your location in the background.
- We do not sell, share, or monetize any of your data.
- We do not use advertising SDKs or third-party trackers (no Google Analytics,
  Meta SDK, etc.).
- We do not require an account with us. There is no Snap311 account; your
  contact info stays on your device and is only attached to the reports you
  submit to DC.

## Third parties

When you submit a report, the data you've entered is sent to:

- **DC's official 311 API** (`dc311-api.herokuapp.com`) — the same backend the
  official DC 311 app and 311.dc.gov web portal use. Their handling of your
  data is governed by DC government policy.
- **DC's official 311 worker** (`dc311-api-worker.herokuapp.com`) — for photo
  attachments, stored in DC's Salesforce.

If you opt in (or leave on by default) to diagnostics:

- **Sentry** (sentry.io) — receives error reports with breadcrumbs of what you
  did right before the error. API keys are scrubbed before send. Personal
  info (name, email, contact info) is never sent. You can disable any time.

## Your choices

- **Disable diagnostics**: Settings → Send diagnostics → off.
- **Remove your saved info**: Delete the app. Local storage is erased with
  the app on iOS.
- **Remove a submitted report**: Snap311 can't do this — submissions live in
  DC's Salesforce system after you file. Contact DC 311 directly to request
  a record correction.

## Children

Snap311 is not directed at children under 13 and does not knowingly collect
personal information from children.

## Changes

If this policy changes materially, the new version will be posted at
https://github.com/kfiducia/snap311-policy/blob/main/privacy-policy.md
with an updated date. Continued use after a change indicates acceptance.

## Contact

Open an issue: https://github.com/kfiducia/snap311-policy/issues
