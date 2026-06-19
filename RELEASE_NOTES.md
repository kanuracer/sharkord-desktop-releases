# Sharkord Desktop v0.4.20

## Changes

- Promotes the v0.4.20 build to the Stable update channel.
- Refreshes the Sharkord auth token before WebSocket reconnects after idle time so realtime subscriptions keep working instead of failing with `You must be auth`.
- Uses fresh auth for uploads after long-running sessions.
