# Sharkord Desktop v0.4.0

## Changes

- Adds release channels: Stable uses `main/latest.json`, Beta uses `beta/latest.json`.
- Adds startup update checks with a visible update call-to-action when a matching release is available.
- Adds an Update settings view with selected channel, current/available versions, release asset details, changelog, and release link.
- Persists the selected release channel across restarts.
- Localizes channel permission state labels in German: `Vererben`, `Erlauben`, `Verweigern`.
- Cleans public-facing Sharkord Desktop wording to avoid visible Discord-branded copy where neutral Sharkord wording is expected.
- Fixes the Linux-hosted Windows cross-build task so release builds no longer require PowerShell.
