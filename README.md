# MeetNote entry page

Public GitHub Pages entry page for the existing private MeetNote Apps Script web app.
Only this wrapper is published here. Audio, meeting records, reports and API keys are stored by the private app, never by this page.

The iframe uses the existing deployment URL. Google owner-only authentication and server-side authorization remain required. If embedded Google sign-in is unavailable, use the top-right direct link to sign in as the owner, then return and reload this page.

The Google Apps Script creator banner is absent in the embedded view; the original direct `/exec` page retains Google's banner. The Apps Script iframe sandbox remains active.

MeetNote's Apps Script `doGet()` allows embedding with `XFrameOptionsMode.ALLOWALL`. This permits third-party pages to embed the app; it does not grant their users access to the private archive. PrintHub PIN/SSO is not implemented in this wrapper.
