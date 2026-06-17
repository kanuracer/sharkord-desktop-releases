# Sharkord Desktop v0.3.96

Hotfix release for profile/settings placement and own-profile modal polish.

## Fixed / Polished
- Profile editing now lives only in the account footer popup, not in Server Settings.
- Server Settings tabs no longer expose a Profile tab; server logo management remains in General.
- Own-profile popup uses dedicated modal CSS instead of inheriting welcome-dialog geometry.
- Profile modal close button, banner/avatar preview, three-card layout, sticky footer, and disabled password action styling are polished and viewport-safe.

## Verification
- Frontend tests: 193/193 pass on Linux; 193/193 pass on macOS build host.
- Production frontend build: pass on Linux and macOS build host.
- npm audit high: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Browser/visual smoke: own-profile modal close button, banner/avatar preview, balanced cards, readable disabled password button, and footer passed.
- macOS arm64 app bundle: native build, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Artifacts: Linux amd64, Windows amd64, macOS arm64.
- Checksums: see `SHA256SUMS.txt`.

## Artifacts
- `sharkord-desktop-0.3.96-darwin-arm64.zip`
- `sharkord-desktop-0.3.96-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.96-windows-amd64.exe`
- `SHA256SUMS.txt`
