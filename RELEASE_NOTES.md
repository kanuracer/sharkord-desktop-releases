# Sharkord Desktop v0.3.92

Server Settings > Users role-card layout hotfix.

## Fixed
- Role chips now live in a full-width roles section inside each user card.
- The `Owner` chip and other role pills no longer clip/cut off at the left/top card edge.
- Moderation buttons (`Kick`, `Ban`, `Delete`) use their own full-width action row inside the card.
- Regression coverage rejects the old capped/right-aligned action grid and cramped role layout.

## Verification
- Frontend tests: 184/184 pass on Linux and macOS build host.
- Production frontend build: pass.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Browser fixture geometry: every role chip and action group stays inside each user-card bounds; no row overflow.
- Visual smoke: patched fixture shows no clipped role chips/actions.
- macOS arm64 app bundle: built on native macOS arm64 host, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Artifacts: Linux amd64, Windows amd64, macOS arm64.
- Checksums: see `SHA256SUMS.txt`.

## Artifacts
- `sharkord-desktop-0.3.92-darwin-arm64.zip`
- `sharkord-desktop-0.3.92-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.92-windows-amd64.exe`
- `SHA256SUMS.txt`
