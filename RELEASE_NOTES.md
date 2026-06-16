# Sharkord Desktop v0.3.93

Server Settings > Users height-clipping hotfix.

## Fixed
- User cards now auto-size vertically instead of clipping wrapped role chips and moderation buttons.
- Restored the accepted width layout: `Rollen:` label beside role chips and compact/right-aligned action buttons.
- Regression coverage now checks the exact height failure: role chips and action groups must fit inside each card.

## Verification
- Frontend tests: 185/185 pass on Linux and macOS build host.
- Production frontend build: pass.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Browser fixture geometry: each role chip and action group stays inside each user-card bounds; rows auto-size to content.
- Visual smoke: patched fixture shows full card height and no clipped role chips/actions.
- macOS arm64 app bundle: built on native macOS arm64 host, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Artifacts: Linux amd64, Windows amd64, macOS arm64.
- Checksums: see `SHA256SUMS.txt`.

## Artifacts
- `sharkord-desktop-0.3.93-darwin-arm64.zip`
- `sharkord-desktop-0.3.93-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.93-windows-amd64.exe`
- `SHA256SUMS.txt`
