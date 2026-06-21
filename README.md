# Sharkord Desktop Releases

Offizielle öffentliche Release-Ablage für **Sharkord Desktop**, den nativen Desktop-Client für selbst gehostete Sharkord-Server.

**Aktuelle stabile Version:** `v0.5.13`

**Release-Seite:** <https://github.com/kanuracer/sharkord-desktop-releases/releases/tag/v0.5.13>

**Source-Repo:** <https://github.com/kanuracer/sharkord-desktop>

**Server-Fork:** <https://github.com/kanuracer/sharkord-server>

Sharkord Desktop ist kein iframe und kein Electron-Webwrapper. Die App nutzt einen nativen Wails/Go-Backend-Shell, React/TypeScript im Frontend, verschlüsselte lokale Credential-Speicherung und GitHub-Releases für Updates.

---

## Screenshots

### Start / Onboarding

![Sharkord Desktop welcome screen](docs/screenshots/01-welcome.png)

Beim ersten Start ist die App leer und führt direkt zum Server-Hinzufügen. Keine Default-Server, keine versteckten Beispiel-Credentials.

### Server hinzufügen

![Add Sharkord server dialog](docs/screenshots/02-add-server.png)

Server können mit URL, optionalem Invite-Code und optionalem Server-Passwort hinzugefügt werden. Login-Daten können verschlüsselt gespeichert werden, damit Auto-Connect möglich ist.

### Appearance & Accessibility

![Appearance and accessibility settings](docs/screenshots/03-appearance-settings.png)

Dark/Light-Theme, Sprache, kompakte Darstellung, reduzierte Animationen, High-Contrast und Font-Größe sind direkt in der Desktop-App einstellbar.

### Audio, Video & Screen Sharing

![Audio and video settings](docs/screenshots/04-audio-video-settings.png)

Die App bringt eigene Desktop-Settings für Mikrofon, Playback, Webcam, Voice-Filter, Echo-Cancellation, Screen-Sharing-Auflösung, FPS, Codec, Bitrate und System-Audio mit.

### Import / Export

![Import and export settings](docs/screenshots/05-import-export.png)

Einstellungen können als JSON exportiert/importiert werden. User-Daten/Credentials sind optional und müssen bewusst eingeschlossen werden.

> Screenshots sind mit generischem Demo-/Empty-State aufgenommen. Keine privaten Server, Accounts, Nachrichten oder Tokens sichtbar.

---

## Download

| Plattform | Datei | Direktlink |
|---|---|---|
| Windows amd64 | `sharkord-desktop-0.5.13-windows-amd64.exe` | [Download](https://github.com/kanuracer/sharkord-desktop-releases/releases/download/v0.5.13/sharkord-desktop-0.5.13-windows-amd64.exe) |
| Linux amd64 | `sharkord-desktop-0.5.13-linux-amd64.tar.gz` | [Download](https://github.com/kanuracer/sharkord-desktop-releases/releases/download/v0.5.13/sharkord-desktop-0.5.13-linux-amd64.tar.gz) |
| macOS arm64 | `sharkord-desktop-0.5.13-darwin-arm64.zip` | [Download](https://github.com/kanuracer/sharkord-desktop-releases/releases/download/v0.5.13/sharkord-desktop-0.5.13-darwin-arm64.zip) |

Checksums stehen in [`SHA256SUMS.txt`](SHA256SUMS.txt).

```text
1d5e3a021951c5e4b81083fef4a7ac7e8932a54f33afa6bff45ccca153eed362  sharkord-desktop-0.5.13-darwin-arm64.zip
2b53af8e7bb26956e89e4403710011843ddf4daf6fd50a3ac52618c5f81c67dc  sharkord-desktop-0.5.13-linux-amd64.tar.gz
8a85605419802a315821b3cddb16985683e7eda080a1aca33fc3c64a1ac8167a  sharkord-desktop-0.5.13-windows-amd64.exe
```

### Checksum prüfen

Linux/macOS:

```bash
sha256sum -c SHA256SUMS.txt
```

Windows PowerShell:

```powershell
Get-FileHash .\sharkord-desktop-0.5.13-windows-amd64.exe -Algorithm SHA256
```

Der Hash muss `8a85605419802a315821b3cddb16985683e7eda080a1aca33fc3c64a1ac8167a` sein.

---

## Installation

### Windows

1. `sharkord-desktop-0.5.13-windows-amd64.exe` herunterladen.
2. Datei starten.
3. Falls Windows SmartScreen warnt: Herausgeber/Signatur prüfen, dann bewusst fortfahren.
4. Server hinzufügen und mit deiner Sharkord-Identity anmelden.

### Linux

```bash
tar -xzf sharkord-desktop-0.5.13-linux-amd64.tar.gz
./sharkord-desktop
```

Je nach Distribution werden WebKit/GTK-Laufzeitbibliotheken benötigt, weil Sharkord Desktop auf Wails basiert.

### macOS arm64

1. `sharkord-desktop-0.5.13-darwin-arm64.zip` herunterladen.
2. ZIP entpacken.
3. `.app` nach `/Applications` ziehen.
4. Beim ersten Start ggf. Rechtsklick → Öffnen nutzen, wenn Gatekeeper die App blockiert.

---

## Was Sharkord Desktop kann

### Native Desktop-Shell

- Native Wails/Go-App statt Electron.
- Kein iframe um die Web-App.
- Persistente Fensterposition/-größe.
- Lokale Settings für Theme, Sprache, Audio/Video, Notifications und Updates.

### Multi-Server & Login

- Mehrere Sharkord-Server speichern.
- Server per URL oder Invite-Link hinzufügen.
- Auto-Connect mit gespeicherten Credentials.
- Credentials werden lokal verschlüsselt gespeichert:
  - Windows: DPAPI
  - Linux/macOS: AES-GCM über App-Backend-Speicher

### Chat & Channels

- Text-Channels und Channel-Gruppen.
- Nachrichten senden, bearbeiten und löschen.
- Rich-Text/HTML-kompatible Composer-Ausgabe.
- Replies/Threads.
- Reactions.
- Message-Pins.
- Typing-Status.
- Read-State/Unread-State.
- Dateiuploads und Attachment-Lightbox für Bilder/Storage-Vorschau.

### Direct Messages

- Direct-Message-Übersicht.
- Neue DMs öffnen.
- DM-Unread-Zähler.
- **DM-Konversation löschen** auf kompatiblen Kanuracer-Servern.
- Auf nicht kompatiblen Servern bleibt die Aktion sauber capability-gated und zeigt einen Unsupported-Hinweis statt kaputt zu mutieren.

### Voice, Video & Screen Sharing

- Voice-Channel beitreten/verlassen.
- Mikrofon stummschalten.
- Audio-Ausgabe stummschalten.
- Webcam aktivieren.
- Screen Sharing.
- Screen-Share-Systemaudio, wenn Plattform/WebView es unterstützt.
- Device-Auswahl für Mikrofon, Playback und Webcam.
- Echo-Cancellation, Noise-Suppression, Auto-Gain und Voice-Isolation.
- Resolution/FPS/Bitrate/Codec-Settings für Video und Screen Sharing.
- Externe Stream-/Popout-Ansicht.
- **Voice-User verschieben** auf kompatiblen Kanuracer-Servern mit passender `MOVE_MEMBERS`-Permission.

### Suche & Navigation

- Command Palette mit `Ctrl/Cmd + K`.
- Schnelle Navigation zu Servern, Channels, DMs und App-Aktionen.
- Globale Suche für Nachrichten und Dateien, wenn der Server Search unterstützt.

### Server-Admin & Moderation

Je nach Server-Rechten und Server-Capabilities bietet die App Admin-Oberflächen für:

- Server-Settings.
- Server-Name, Beschreibung und Logo.
- Rollen und Permissions.
- Channel- und Category-Verwaltung.
- Channel-Permission-Overrides.
- Benutzerverwaltung und Moderation.
- Invites.
- Emojis.
- Storage-Settings, Quotas und eigene gespeicherte Dateien.
- Plugins, Plugin-Marketplace und Plugin-Kommandos.
- **Owner-Token nutzen** auf kompatiblen Kanuracer-Servern.
- **Server-Self-Update** auf kompatiblen Kanuracer-Servern.

### Kanuracer-Fork Features

Sharkord Desktop erkennt nach Login die Server-Capabilities. Originale Sharkord-Server und Kanuracer-Server werden nicht per Domain oder Versionsstring erraten, sondern über den Capability-Endpunkt.

Capability-gated Features:

| Feature | Capability | Verhalten |
|---|---|---|
| DM-Konversation löschen | `directMessageDelete` | Löscht DMs nur, wenn Server Route/Capability anbietet. |
| Owner-Token | `ownerToken` | Owner-Aktionen nur auf kompatiblen Servern. |
| Server-Self-Update | `serverSelfUpdate` | Server-Update UI nur mit Server-Support. |
| Voice-User verschieben | `voiceUserMove` | Drag/Move nur mit Server-Support und Permission. |

Dadurch bleibt die Desktop-App mit originalem Sharkord nutzbar, schaltet Fork-Extras aber frei, wenn `kanuracer/sharkord-server` sie bereitstellt.

### Updates

- Stable/Beta Release-Channel.
- In-App Update-Check über GitHub Releases.
- Plattformfilter für Windows/Linux/macOS Assets.
- Changelog-Anzeige in Settings → Updates.
- Manuelle Downloads bleiben hier im Repo verfügbar.

### Import / Export

- App-Settings als JSON exportieren.
- Import über native Datei-Dialoge.
- Optionaler Export gespeicherter User-Daten/Credentials nur nach bewusster Auswahl.
- Import validiert Datei-Typ und Schema.

### Sprache & Accessibility

- Deutsch und Englisch.
- Dark/Light Theme.
- Font-Größe.
- Compact Mode.
- Reduced Motion.
- High Contrast.
- Laufende i18n-Regressionstests gegen gemischte DE/EN UI-Texte.

---

## Kompatibilität

| Ziel | Status |
|---|---|
| Original Sharkord Server | Basisfunktionen, Fork-Extras ausgeblendet/unsupported. |
| `kanuracer/sharkord-server` | Basisfunktionen plus capability-gated Fork-Features. |
| Windows amd64 | Release-Asset vorhanden. |
| Linux amd64 | Release-Asset vorhanden. |
| macOS arm64 | Release-Asset vorhanden. |
| macOS amd64 | Kein aktuelles Asset in `v0.5.13`. |

---

## Update-Feed

Die App nutzt GitHub Releases als Update-Quelle. Zusätzlich liegt [`latest.json`](latest.json) im Repo für maschinenlesbare Release-Metadaten.

Aktuelle GitHub API:

```text
https://api.github.com/repos/kanuracer/sharkord-desktop-releases/releases/latest
```

Aktueller Release-Download-Pfad:

```text
https://github.com/kanuracer/sharkord-desktop-releases/releases/download/v0.5.13/<asset-name>
```

---

## Release Notes

Kurzfassung für `v0.5.13`:

- Unsaved lokale Rollen-/Permission-Edits bleiben erhalten, während Realtime-Role-Updates ankommen.
- Enthält die 0.5.12 English-Locale-Fixes für kaputte Fallback-Texte wie `Privatee Voice Channels` und `3 Categoryn`.

Volltext: [`RELEASE_NOTES.md`](RELEASE_NOTES.md)

---

## Häufige Fragen

### Ist das der Server?

Nein. Dieses Repo enthält Desktop-Release-Artefakte. Der Server liegt hier:

- <https://github.com/kanuracer/sharkord-server>

### Ist das der Desktop-Source-Code?

Nein. Der Source-Code liegt hier:

- <https://github.com/kanuracer/sharkord-desktop>

### Warum sehe ich DM Delete / Server Update / Voice Move nicht?

Diese Features hängen vom verbundenen Server ab. Die Desktop-App schaltet sie nur frei, wenn der Server die passende Capability meldet. Mit originalem Sharkord oder einem alten Kanuracer-Server bleiben sie ausgeblendet oder zeigen einen Unsupported-Hinweis.

### Welche Version soll ich installieren?

Nimm immer das neueste GitHub Release für deine Plattform. Aktuell: `v0.5.13`.

### Kann ich Beta nutzen?

Die App unterstützt Release-Channels. Dieses Repo zeigt primär den aktuellen stabilen Stand. Beta-Releases können je nach Veröffentlichungsstand im Release-Verlauf oder Feed auftauchen.

---

## Projektstatus

Sharkord selbst ist Alpha-Software. Sharkord Desktop folgt diesem Stand: Features können sich ändern, Server-APIs können neue Capabilities bekommen, und alte Server können manche Desktop-Aktionen nicht unterstützen.

Für beste Ergebnisse: Desktop-App und `kanuracer/sharkord-server` gemeinsam aktuell halten.
