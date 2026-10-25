# ManageMe OTA bundles

Built web bundles for the ManageMe Android app, delivered over the air by
`@capgo/capacitor-updater`. Contains no source code: only the compiled web
bundle that already ships inside every APK.

- `manifest.json` — the current bundle and the Android build codes it may reach.
  Read by `https://api.orbynex.io/api/public/ota/updates`, which the app asks.
- Releases — one zip per bundle.

Published with `npm run ota:publish` in ManageMe-client. Do not edit by hand,
except to stop an update: set `"version": "builtin"` to send phones back to the
code built into their app.
