# Sharkord Desktop v0.3.90

Admin text and settings layout hotfix.

## Fixed
- English server settings now translate the full password-first-join phrase atomically: `Ask for password only on first join` instead of mixed-language `Nur beim ersten Beitritt nach Password fragen`.
- Server settings checkbox rows are scoped and aligned inline so the checkbox stays beside its label.
- Users admin role chips/actions keep stable spacing and avoid clipping in the compact dark settings panel.
- Regression coverage now locks the i18n replacement ordering and admin settings/users CSS layout.

## Verification
- Frontend tests: 184/184 pass on Linux and macOS build host.
- Production frontend build: pass, no chunk-size warning.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Visual smoke: Chromium admin settings fixture + vision check passed (no German text visible, checkbox inline, role chips/actions unclipped, no horizontal overflow).
- macOS arm64 app bundle: built on native macOS arm64 host, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Artifacts: Linux amd64, Windows amd64, macOS arm64.
- Checksums: see `SHA256SUMS.txt`.

## Artifacts
- `sharkord-desktop-0.3.90-darwin-arm64.zip`
- `sharkord-desktop-0.3.90-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.90-windows-amd64.exe`
- `SHA256SUMS.txt`
