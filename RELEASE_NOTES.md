# Sharkord Desktop v0.3.82

Hotfix release for the Server Settings → Users panel.

## Fixed
- Prevented Sharkord's deleted-user placeholder from appearing in desktop member/admin user lists.
- Guarded user context menus, moderation actions, role toggles, and voice user rendering against the deleted-user placeholder.
- Fixed the Users admin list layout so role chips no longer clip or overlap rows.

## Verification
- Frontend tests: 177/177 pass.
- Production frontend build: pass.
- Go tests: pass.
- Windows/Linux/macOS local artifacts built from this release.
- Users CSS visual smoke: pass; dark themed rows, no raw white controls, unclipped role chips, right-aligned actions, no horizontal scrollbar.

## Artifacts
- `sharkord-desktop-0.3.82-darwin-arm64.zip`
- `sharkord-desktop-0.3.82-linux-amd64.tar.gz`
- `sharkord-desktop-0.3.82-windows-amd64.exe`
- `SHA256SUMS.txt`
