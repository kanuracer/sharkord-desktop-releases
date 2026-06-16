# Sharkord Desktop Releases

Latest: v0.3.95

This repository intentionally keeps only the newest public Sharkord Desktop release in the current tree. Older versions may exist in git history, but current downloads and the GitHub latest release point to v0.3.95.

## v0.3.95

Hotfix release for profile/settings polish, global search styling, voice user move drag/drop, and English profile text fallback.

### Fixed / Polished
- Account footer opens the editable profile popup directly instead of routing through server settings.
- Server logo management lives in Server Settings > General, no longer in the profile section.
- Global Search and profile popups use existing Sharkord panel tokens and avoid undefined dark fallbacks.
- Account identity button no longer overflows its footer grid.
- English fallback translation no longer recursively turns profile strings into `Profileeeee...`.

### Added
- Privileged users can drag a voice member onto another voice channel to move that member.
- Voice move API fallback supports current and legacy server route names.

### Downloads
- `sharkord-desktop-0.3.95-darwin-arm64.zip`
- `sharkord-desktop-0.3.95-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.95-windows-amd64.exe`
- `SHA256SUMS.txt`

### Verification
- Testserver smoke: connected to Sharkord Desktop Testserver; Global Search and profile dialog verified.
- Frontend tests: 192/192 pass on Linux; 192/192 pass on macOS build host.
- Production frontend build: pass on Linux and macOS build host.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Browser/visual smoke: no horizontal overflow in profile popup, global search, server logo card, and account footer.
- macOS arm64 app bundle: native build, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Checksums: `sha256sum -c SHA256SUMS.txt` pass.

Source repo/tag: https://github.com/kanuracer/sharkord-desktop/tree/v0.3.95
GitHub Release: https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.3.95
