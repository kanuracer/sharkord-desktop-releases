# Sharkord Desktop Releases
## v0.3.28

- Fix macOS updater compatibility: darwin ZIP now contains `.app/Contents/MacOS/sharkord-desktop`, matching existing updater validation.
- Keeps stable macOS bundle identifier `eu.kanuracer.sharkord-desktop`.
- Assets: Linux amd64, Windows amd64, macOS arm64.


## v0.3.27

- Remote media refresh when webcam/screen flags arrive without a producer event.
- Server deletion removes the server from UI/native state before credential cleanup.
- Assets: Linux amd64, Windows amd64, macOS arm64.


## v0.3.26

- Fix: Serverliste wird zusätzlich nativ unter `state.json` gespeichert und beim Start wieder geladen. Dadurch verschwinden Server nicht mehr, wenn WebView LocalStorage/Bundles/Profiles wechseln.
- Migration: vorhandener LocalStorage-State wird nach erstem Start in die native State-Datei gespiegelt.
- Builds: Linux amd64, Windows amd64, macOS arm64.

Assets: `releases/v0.3.26/`

## v0.3.25

- Fix: Remote Kamera-/Bildschirmstream wird nicht mehr als aktiver, aber leerer Tile angezeigt. Producer-Events werden nur im aktuell beigetretenen Voice-Channel konsumiert, eigene Producer ignoriert, frühe Producer bis zum fertigen Consumer-Transport gequeued.
- Fix: Video-Tiles starten Playback explizit und zeigen Playback-Fehler sichtbar an.
- Builds: Linux amd64, Windows amd64, macOS arm64.

Assets: `releases/v0.3.25/`

Latest: v0.3.24

## v0.3.24

- Linux: `releases/v0.3.24/sharkord-desktop-0.3.24-linux-amd64.tar.gz`
- Windows: `releases/v0.3.24/sharkord-desktop-0.3.24-windows-amd64.exe`
- macOS arm64: `releases/v0.3.24/sharkord-desktop-0.3.24-darwin-arm64.zip`
- Checksums: `releases/v0.3.24/SHA256SUMS.txt`

Source repo/tag: https://github.com/kanuracer/sharkord-desktop/tree/v0.3.24
GitHub Release: https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.3.24

## v0.3.23

- Linux: `releases/v0.3.23/sharkord-desktop-0.3.23-linux-amd64.tar.gz`
- Windows: `releases/v0.3.23/sharkord-desktop-0.3.23-windows-amd64.exe`
- macOS arm64: `releases/v0.3.23/sharkord-desktop-0.3.23-darwin-arm64.zip`
- Checksums: `releases/v0.3.23/SHA256SUMS.txt`

Source repo/tag: https://github.com/kanuracer/sharkord-desktop/tree/v0.3.23
GitHub Release: https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.3.23

## v0.3.22

- Linux: `releases/v0.3.22/sharkord-desktop-0.3.22-linux-amd64.tar.gz`
- Windows: `releases/v0.3.22/sharkord-desktop-0.3.22-windows-amd64.exe`
- macOS arm64: `releases/v0.3.22/sharkord-desktop-0.3.22-darwin-arm64.zip`
- Checksums: `releases/v0.3.22/SHA256SUMS.txt`

Source repo/tag: https://github.com/kanuracer/sharkord-desktop/tree/v0.3.22
GitHub Release: https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.3.22

