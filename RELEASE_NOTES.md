# Sharkord Desktop v0.3.89

Admin UI polish hotfix.

## Fixed
- English server admin settings no longer leak German fallback strings in storage, users, parity, and update/admin surfaces.
- Users admin panel now uses a responsive grid layout with a stable action column, preventing cramped cards and clipped role/status chips.
- Signed URL TTL presets and storage helper text now translate as whole user-facing phrases.
- Additional regression guards cover English admin screenshots and unwrapped German display strings.

## Verification
- Frontend tests: 183/183 pass on Linux and macOS build host.
- Production frontend build: pass, no chunk-size warning.
- Go tests: pass on Linux and macOS build host.
- Visual smoke: Chromium admin Users screenshot + vision check passed (dark controls, no clipped chips, no overlap, aligned actions, no horizontal scrollbar).
- macOS arm64 app bundle: built on native macOS arm64 host, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Artifacts: Linux amd64, Windows amd64, macOS arm64.
- Checksums: see `SHA256SUMS.txt`.

## Artifacts
- `sharkord-desktop-0.3.89-darwin-arm64.zip`
- `sharkord-desktop-0.3.89-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.89-windows-amd64.exe`
- `SHA256SUMS.txt`
