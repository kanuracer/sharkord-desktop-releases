# Sharkord Desktop v0.3.97

## Changes

- Added a Discord-like left-click profile popover for other users.
- Profile popover appears from member lists, voice sidebar users, voice call user cards, and message author avatar/name clicks.
- Popover displays avatar, banner or banner color, name, identity, status, role count, and bio.
- Right-click user context menus remain separate and unchanged for admin/moderation actions.
- Deleted-user placeholders are guarded and do not open profile popovers.
- Popover positioning clamps to the viewport to avoid offscreen menus.

## Verification

- Frontend tests: 195/195 passed.
- Frontend production build passed.
- npm audit high: 0 vulnerabilities.
- Go tests passed.
- Linux, Windows, and macOS artifacts built.
- SHA256 checks generated and verified locally.
