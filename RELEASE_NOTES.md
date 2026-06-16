# Sharkord Desktop v0.3.91

Users admin layout hotfix.

## Fixed
- Server Settings > Users no longer squeezes role pills beside the action button column.
- Role chips now live in a dedicated roles row and wrap cleanly inside each user card.
- Moderation buttons stay inside the card, right-aligned, with a capped width.
- Regression coverage locks the new Users admin layout against returning to the cramped two-column grid.

## Verification
- Frontend tests: 184/184 pass on Linux and macOS build host.
- Production frontend build: pass.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Visual/geometry smoke: no measured role-chip overflow/clipping and action buttons stay inside cards.
- macOS arm64 app bundle: built on native macOS arm64 host, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Artifacts: Linux amd64, Windows amd64, macOS arm64.
- Checksums: see `SHA256SUMS.txt`.

## Artifacts
- `sharkord-desktop-0.3.91-darwin-arm64.zip`
- `sharkord-desktop-0.3.91-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.91-windows-amd64.exe`
- `SHA256SUMS.txt`
