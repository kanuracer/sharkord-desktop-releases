# Sharkord Desktop v0.5.9 Beta

## Fixed

- Updates live member presence immediately when a user comes online while the desktop app is already open.
- Forces `users.onJoin` realtime events to mark the joined user as online, matching the webclient behavior and avoiding stale offline state until restart.
- Stable channel remains unchanged.

## Notes

- Linux and Windows assets are included in this beta. macOS requires a native macOS build host and is not included in this package.
