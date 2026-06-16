# Sharkord Desktop Releases

Latest: v0.3.92

This repository intentionally keeps only the newest public Sharkord Desktop release in the current tree. Older versions may exist in git history, but current downloads and the GitHub latest release point to v0.3.92.

## v0.3.92

Server Settings > Users card layout hotfix.

### Fixed
- Role chips now use a full-width role section inside each user card.
- `Owner`, `Guest`, `Member`, and `CoAdmin` chips no longer clip at the card edge.
- `Kick`, `Ban`, and `Delete` buttons stay inside each card on their own full-width action row.
- Regression coverage now blocks returning to the capped/right-aligned action layout that squeezed the roles.

### Downloads
- `sharkord-desktop-0.3.92-darwin-arm64.zip`
- `sharkord-desktop-0.3.92-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.92-windows-amd64.exe`
- `SHA256SUMS.txt`

### Verification
- Frontend tests: 184/184 pass on Linux and macOS build host.
- Production frontend build: pass.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Visual/geometry smoke: role chips and action buttons measured fully inside every user card.
- macOS arm64 app bundle: native build, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Checksums: `sha256sum -c SHA256SUMS.txt` pass.

Source repo/tag: https://github.com/kanuracer/sharkord-desktop/tree/v0.3.92
GitHub Release: https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.3.92
