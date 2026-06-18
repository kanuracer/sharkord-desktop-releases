# Sharkord Desktop v0.4.0

## Changes

- Adds release channels: Stable uses `main/latest.json`, Beta uses `beta/latest.json`.
- Adds startup update checks with a visible update call-to-action when a matching release is available.
- Adds an Update settings view with selected channel, current/available versions, release asset details, changelog, and release link.
- Persists the selected release channel across restarts.
- Localizes channel permission state labels in German: `Vererben`, `Erlauben`, `Verweigern`.
- Cleans public-facing Sharkord Desktop wording to avoid visible Discord-branded copy where neutral Sharkord wording is expected.
- Fixes the Linux-hosted Windows cross-build task so release builds no longer require PowerShell.

## Verification

- Frontend tests: 211/211 passed.
- Frontend production build passed.
- npm audit high: 0 vulnerabilities.
- Go tests passed.
- Linux and Windows artifacts built from source commit `24fb176`.
- macOS Apple Silicon artifact built on the macOS build host from the exact source archive for commit `24fb176`; codesign verification passed.
- SHA256 checks generated and verified locally.
- Stable and Beta update feeds both point to v0.4.0.
