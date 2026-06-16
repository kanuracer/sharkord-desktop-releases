# Sharkord Desktop Releases

Latest: v0.3.91

This repository intentionally keeps only the newest public Sharkord Desktop release in the current tree. Older versions may exist in git history, but current downloads and the GitHub latest release point to v0.3.91.

## v0.3.91

Users admin layout hotfix.

### Fixed
- Server Settings > Users now uses a dedicated single-column user-card layout.
- Role chips (`Owner`, `Guest`, `Member`, `CoAdmin`) wrap inside their own roles row instead of being squeezed under the moderation buttons.
- Moderation actions stay right-aligned inside each user card without clipping role pills.

### Downloads
- `sharkord-desktop-0.3.91-darwin-arm64.zip`
- `sharkord-desktop-0.3.91-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.91-windows-amd64.exe`
- `SHA256SUMS.txt`

### Verification
- Frontend tests: 184/184 pass on Linux and macOS build host.
- Production frontend build: pass.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Visual/geometry smoke: admin Users role chips/actions have no measured overflow or clipping.
- macOS arm64 app bundle: native build, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Checksums: `sha256sum -c SHA256SUMS.txt` pass.

Source repo/tag: https://github.com/kanuracer/sharkord-desktop/tree/v0.3.91
GitHub Release: https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.3.91
