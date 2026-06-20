# Sharkord Desktop v0.5.1 Beta

## Fixes

- Reconnects the full Sharkord session when protected realtime subscriptions report authentication failure.
- Resubscribes after reconnect so `categories.onDelete` and similar idle subscription errors recover automatically.
- Keeps the active channel selected after the reconnect.
- Keeps stable channel unchanged.
