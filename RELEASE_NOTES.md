# Sharkord Desktop v0.3.85

English locale cleanup release.

## Fixed
- Removed remaining German UI chrome when English is selected.
- Language selector now shows `German` instead of `Deutsch` while in English mode.
- Add-server modal labels/placeholders/auto-connect text are translated.
- Audio & Video dynamic status and screen-sharing/simulcast messages are translated.
- Import/Export explanatory copy is translated as one complete phrase to avoid mixed German/English text.

## Verification
- Frontend tests: 180/180 pass.
- Production frontend build: pass.
- Go tests: pass on Linux and macOS build host.
- Production preview visual/DOM QA: English Settings tabs and Add-server modal show no German fragments.
- Linux packaged app startup: pass under Xvfb from final tarball.
- macOS arm64 app bundle: built on MacBook, codesigned ad-hoc, `codesign --verify --deep --strict` pass.
- Artifacts: Linux amd64, Windows amd64, macOS arm64.
- Checksums: see `SHA256SUMS.txt`.

## Artifacts
- `sharkord-desktop-0.3.85-darwin-arm64.zip`
- `sharkord-desktop-0.3.85-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.85-windows-amd64.exe`
- `SHA256SUMS.txt`
