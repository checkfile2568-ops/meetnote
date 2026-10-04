# MeetNote entry page

Public GitHub Pages entry page for MeetNote. All signed-in Google users may use the app; each has a separate private archive in their own Drive.
Only this wrapper is published here. Audio, meeting records, reports and API keys are stored by the private app, never by this page.

The iframe uses the existing deployment URL. Google authentication, user authorization and server-side checks remain required. If embedded Google sign-in is unavailable, use the top-right direct link to sign in and authorize the app, then return and reload this page.

The Google Apps Script creator banner is absent in the embedded view; the original direct `/exec` page retains Google's banner. The Apps Script iframe sandbox remains active.

MeetNote's Apps Script `doGet()` allows embedding with `XFrameOptionsMode.ALLOWALL`. This permits third-party pages to embed the app; it does not grant access to another user's private archive. System and AI settings are restricted to the administrator account, including server-side checks. PrintHub PIN/SSO is not implemented in this wrapper.
