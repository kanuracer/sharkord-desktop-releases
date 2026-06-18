# Sharkord Desktop v0.3.99

## Changes

- Fixed the Channel Settings general tab checkbox layout so `Privater Channel` remains a normal inline checkbox and cannot inherit full-width text-input styling.
- Reduced Channel Settings modal vertical stretching by using content-sized rows for the compact general tab and constraining the permissions tab separately.
- Added compatibility fallback for servers without `plugins.getSlots`: plugin slots now render as empty instead of surfacing `No "query"-procedure on path "plugins.getSlots"` in server settings.

## Verification

- Frontend tests: 204/204 passed.
- Frontend production build passed.
- npm audit high: 0 vulnerabilities.
- Go tests passed.
- Browser visual smoke confirmed the checkbox is inline, no giant slider/bar is visible, the modal is compact, and `Bereit` appears only as status text.
- Linux startup smoke under `xvfb-run`: timeout after launch, app stayed up.
- Linux, Windows, and macOS artifacts built from source commit `35efde7482d8afc9d584b2851d79d538c7f378d7`.
- SHA256 checks generated and verified locally.
