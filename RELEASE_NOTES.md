# Sharkord Desktop v0.5.10 Beta

## Fixed

- Completes English locale coverage for the reported update/settings, server update, direct-message delete, storage, and voice move UI surfaces.
- Moves these strings into the i18n language table/fallbacks instead of leaking mixed German/English text when English is selected.
- Adds regression coverage for the reported screenshots so phrases like `Direktnachricht delete`, `Herunterladen`, `URL kopieren`, `Server-Update`, and `verschoben nach` stay translated.
- Stable channel remains unchanged.

## Verification

- Frontend tests: 286/286 passing.
- Frontend production build: passing.
- Go tests: 27/27 passing.
- npm audit high/prod: 0 vulnerabilities.
- govulncheck: 0 reachable vulnerabilities.

## Notes

- Linux and Windows assets are included in this beta. macOS requires a native macOS build host and is not included in this package.
