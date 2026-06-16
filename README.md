# Sharkord Desktop Releases

Latest: v0.3.94

This repository intentionally keeps only the newest public Sharkord Desktop release in the current tree. Older versions may exist in git history, but current downloads and the GitHub latest release point to v0.3.94.

## v0.3.94

Global search and first-run profile setup parity release.

### Added
- Global Search dialog via Ctrl/Cmd+K for server-wide message and file search.
- Message search results can jump directly to the matched message in its channel.
- Welcome/Profile Setup dialog opens when the server requests onboarding and lets users set display name, bio, banner color, and optional avatar.

### Fixed / Polished
- Global Search and Welcome/Profile Setup dialogs use Sharkord dark modal styling and remain viewport-safe.
- Search response normalization accepts legacy `messages`, `files`, `results`, `items`, and array response shapes.
- Welcome/Profile Setup stores completion per server/user so it does not re-open after save or skip.

### Downloads
- `sharkord-desktop-0.3.94-darwin-arm64.zip`
- `sharkord-desktop-0.3.94-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.94-windows-amd64.exe`
- `SHA256SUMS.txt`

### Verification
- Frontend tests: 187/187 pass on Linux; 187/187 pass on macOS build host.
- Production frontend build: pass on Linux and macOS build host.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Browser/visual smoke: Global Search + Welcome/Profile Setup dialogs show no horizontal overflow, clipped actions, or overlap.
- macOS arm64 app bundle: native build, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Checksums: `sha256sum -c SHA256SUMS.txt` pass.

Source repo/tag: https://github.com/kanuracer/sharkord-desktop/tree/v0.3.94
GitHub Release: https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.3.94
