# Sharkord Desktop v0.5.34 Beta

## Fixed

- Adds always-on local voice diagnostics at the React/Wails boundary for voice join/render/realtime events.
- Writes diagnostics to the app config directory instead of sending live debug HTTP payloads.
- Redacts auth fields, message bodies, HTML/content, and bearer/token-like values before writing diagnostic logs.

## Known limitation

- macOS Apple Silicon beta artifact was not produced in this Linux build environment.

Stable channel stays unchanged.
