# Sharkord Desktop v0.3.98

## Changes

- Added thread/reply parity: reply controls, parent-message previews, thread sidebar/panel, thread compose, and reply-aware typing notifications.
- Added rich composer parity with native content-editable compose, formatting actions, plugin command affordances, dynamic height behavior, and Arrow-Up edit support.
- Added channel permission override management in channel settings, including role/user override targets, update/delete wrappers, and public-channel safety warning.
- Added native plugin UI slots for topbar, chat actions, connect, and content-wrapper surfaces, plus plugin admin slot visibility.
- Preserved native rendering only for plugin slots; no iframe/webview embedding.

## Verification

- Frontend tests: 202/202 passed.
- Frontend production build passed.
- npm audit high: 0 vulnerabilities.
- Go tests passed.
- Linux, Windows, and macOS artifacts built from the final v0.3.98 commit.
- SHA256 checks generated and verified locally.
