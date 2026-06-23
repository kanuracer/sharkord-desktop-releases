# Sharkord Desktop v0.5.31 Beta

## Changes

- Fixes a Desktop Voice crash/blank grey screen when a second participant joins the same voice channel.
- Voice participant state is now normalized before rendering and before media refresh checks.
- Guards the left channel voice list, main voice grid, camera hints, and screen-share cards against missing/partial voice state from realtime payloads.
- Stable channel stays unchanged.
