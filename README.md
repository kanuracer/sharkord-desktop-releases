# Sharkord Desktop Releases

Latest: v0.3.93

This repository intentionally keeps only the newest public Sharkord Desktop release in the current tree. Older versions may exist in git history, but current downloads and the GitHub latest release point to v0.3.93.

## v0.3.93

Server Settings > Users height-clipping hotfix.

### Fixed
- User cards in Server Settings > Users now auto-size vertically so wrapped role chips and moderation buttons are not cut off.
- Restored the accepted v0.3.91/v0.3.92 width behavior: `Rollen:` label stays beside role chips and the `Kick`, `Ban`, `Delete` button group remains compact/right-aligned.
- Regression coverage now blocks fixed-height admin user rows that clip role chips or action buttons.

### Downloads
- `sharkord-desktop-0.3.93-darwin-arm64.zip`
- `sharkord-desktop-0.3.93-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.93-windows-amd64.exe`
- `SHA256SUMS.txt`

### Verification
- Frontend tests: 185/185 pass on Linux and macOS build host.
- Production frontend build: pass.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Browser geometry smoke: all user rows are `max-content` height; role chips and action buttons stay inside each card.
- Visual smoke: all three user cards show full height with no bottom clipping.
- macOS arm64 app bundle: native build, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Checksums: `sha256sum -c SHA256SUMS.txt` pass.

Source repo/tag: https://github.com/kanuracer/sharkord-desktop/tree/v0.3.93
GitHub Release: https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.3.93
