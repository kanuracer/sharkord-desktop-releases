# Sharkord Desktop v0.3.100

## Changes

- Fixed the Channel Settings permissions loader so missing `channels.getPermissions` on older Sharkord servers falls back to an empty override list instead of showing `No "query"-procedure on path "channels.getPermissions"`.
- Added localized unsupported-server handling for channel permission save/delete endpoints when those tRPC procedures are missing.
- Polished the Channel Settings permissions UI with a constrained modal body, stable scroll gutters, safer long status/error wrapping, and clearer active `Inherit` / `Allow` / `Deny` button states.
- Improved the profile edit popup preview: existing banner color is used, banner images render in the preview, selected banner files preview immediately, and multiline bio text wraps/clamps cleanly without horizontal clipping.

## Verification

- Frontend tests: 204/204 passed.
- Frontend production build passed.
- npm audit high: 0 vulnerabilities.
- Go tests passed.
- Browser visual smoke confirmed Channel Settings permissions layout and profile banner/bio preview are clean.
- Linux startup smoke under `xvfb-run`: timeout after launch, app stayed up.
- Linux, Windows, and macOS artifacts built from source commit `4701dad70dfa2a55d54673dfdccf4f1ca7cae501`.
- SHA256 checks generated and verified locally.
