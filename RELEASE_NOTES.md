# Sharkord Desktop v0.4.20 Beta

## Changes

- Refreshes the Sharkord auth token before WebSocket reconnects after idle time so realtime subscriptions keep working instead of failing with `You must be auth`.
- Uses fresh auth for uploads after long-running sessions.
- Keeps stable channel unchanged.
