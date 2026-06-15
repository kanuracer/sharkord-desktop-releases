# Sharkord Desktop Releases

Latest: v0.3.80

## v0.3.80

Admin/UI regression release.

- Fix: Server-Einstellungen > Users löscht Benutzer mit webclient-kompatiblem `wipe` Flag.
- Fix: Server-Einstellungen Modal und Users-Liste bleiben viewport-safe mit themed Scrollbars.
- Fix: Member-Kontextmenü wird am Viewport geklemmt und schneidet rechts nicht mehr ab.
- Fix: Kategorie Drag & Drop trägt Drag-Daten, zeigt Drop-Ziel und hat klaren Drag-Handle.
- Builds: Linux amd64, Windows amd64, macOS arm64.

Assets:
- `releases/v0.3.80/sharkord-desktop-0.3.80-linux-amd64.tar.gz`
- `releases/v0.3.80/sharkord-desktop-0.3.80-windows-amd64.exe`
- `releases/v0.3.80/sharkord-desktop-0.3.80-darwin-arm64.zip`
- `releases/v0.3.80/SHA256SUMS.txt`

## v0.3.74

Server-scoped settings placement and visual polish fix.

- Moved Profile and Parity out of global Settings into Server Settings.
- Kept global Settings app-wide only.
- Polished Profile/Parity tabs for dark Discord-like UI: no native white controls, no number spinners, no clipped cards.

Assets:
- `releases/v0.3.74/sharkord-desktop-0.3.74-linux-amd64.tar.gz`
- `releases/v0.3.74/sharkord-desktop-0.3.74-windows-amd64.exe`
- `releases/v0.3.74/sharkord-desktop-0.3.74-darwin-arm64.zip`
- `releases/v0.3.74/SHA256SUMS.txt`

## v0.3.73

Visual-Fix Release for Discord-like settings parity panels.

Assets:

- `releases/v0.3.73/sharkord-desktop-0.3.73-linux-amd64.tar.gz`
- `releases/v0.3.73/sharkord-desktop-0.3.73-windows-amd64.exe`
- `releases/v0.3.73/sharkord-desktop-0.3.73-darwin-arm64.zip`
- `releases/v0.3.73/SHA256SUMS.txt`

## v0.3.72

- Desktop parity sprint: Server-Logo Upload, i18n-Grundsystem, Profil/Avatar/Banner, Passwort ändern und Notifications.
- Chat parity: Pins-Popover mit Jump-to-message, Recent/Custom-fähige Reactions, Readstate/Unread-Badges.
- Plugin/Voice parity: Plugin Commands, Actions, Logs, Settings, External Streams, Consumer Quality und Popout-Status.
- Assets: Linux amd64, Windows amd64, macOS arm64.

Downloads:

- Linux: `releases/v0.3.72/sharkord-desktop-0.3.72-linux-amd64.tar.gz`
- Windows: `releases/v0.3.72/sharkord-desktop-0.3.72-windows-amd64.exe`
- macOS arm64: `releases/v0.3.72/sharkord-desktop-0.3.72-darwin-arm64.zip`
- Checksums: `releases/v0.3.72/SHA256SUMS.txt`

Source repo/tag: https://github.com/kanuracer/sharkord-desktop/tree/v0.3.72  
GitHub Release: https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.3.72

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

