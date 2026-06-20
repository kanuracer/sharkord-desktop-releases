# Sharkord Desktop v0.5.2 Beta

## Fixes

- Keeps WebSocket reconnects on the server-joined token so protected realtime subscriptions stay authenticated after idle reconnects.
- Fixes `categories.onDelete: You must be authenticated to perform this action.` after reconnects where the server had not marked a freshly refreshed token as joined.
- Leaves upload/auth refresh behavior intact for non-WebSocket calls.
- Stable channel unchanged.
