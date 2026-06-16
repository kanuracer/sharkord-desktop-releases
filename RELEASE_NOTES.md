# Sharkord Desktop v0.3.86

Hotfix release for desktop interaction, startup auto-connect, and update safety.

## Fixed
- Settings/Add-server UI remains clickable/responsive after switching to English.
- Auto-connect now guards in-flight login per saved server, preventing duplicate startup login attempts.
- Audio & Video dynamic device status text is translated after automatic detection and manual refresh.
- Vite high-severity audit advisory is resolved by updating Vite.
- Production frontend output is split into focused vendor chunks; chunk-size warning is gone.

## Verification
- Frontend tests: 181/181 pass.
- Production frontend build: pass, no chunk-size warning.
- npm audit: 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Production preview click QA: Settings, Audio & Video, Refresh devices, Add server reachable; no blocking overlay.
- Production preview English locale QA: visible Audio & Video page has no German fragments after device refresh.
- macOS arm64 app bundle: built on MacBook, codesigned ad-hoc, `codesign --verify --deep --strict` pass.
- Artifacts: Linux amd64, Windows amd64, macOS arm64.
- Checksums: see `SHA256SUMS.txt`.

## Artifacts
- `sharkord-desktop-0.3.86-darwin-arm64.zip`
- `sharkord-desktop-0.3.86-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.86-windows-amd64.exe`
- `SHA256SUMS.txt`
