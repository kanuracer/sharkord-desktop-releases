# Sharkord Desktop v0.3.88

English UI hardening release.

## Fixed
- Fresh/reset desktop installs default to English instead of restoring the old German fallback.
- Remaining German UI/status phrases are covered by i18n entries or dynamic fallback translations.
- Voice, admin, storage, update, and native dialog status text now stays English in English locale.
- macOS microphone/camera/screen-recording permission prompts are English in the app bundle.

## Verification
- Frontend tests: 182/182 pass on Linux and macOS build host.
- Production frontend build: pass, no chunk-size warning.
- npm audit: 0 high vulnerabilities / 0 vulnerabilities.
- Go tests: pass on Linux and macOS build host.
- Production preview click QA: Settings and Audio & Video tab respond; Add-server path reachable; no blocking overlay observed.
- Production preview English locale QA: visible Settings/Audio & Video text scan found no German fragments.
- macOS arm64 app bundle: built on native macOS arm64 host, ad-hoc signed, `codesign --verify --deep --strict` pass.
- Artifacts: Linux amd64, Windows amd64, macOS arm64.
- Checksums: see `SHA256SUMS.txt`.

## Artifacts
- `sharkord-desktop-0.3.88-darwin-arm64.zip`
- `sharkord-desktop-0.3.88-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.88-windows-amd64.exe`
- `SHA256SUMS.txt`
