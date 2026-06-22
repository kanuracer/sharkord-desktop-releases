# Sharkord Desktop v0.5.15 Beta

## Added

- Adds native Desktop TOTP setup and disable controls in the account/profile popup.
- Replaces the inline optional login 2FA field with a focused two-factor verification dialog.
- Keeps Desktop in parity with the Webclient TOTP setup flow.

## Security

- TOTP one-time codes are not stored.
- Remembered-device app passwords remain revocable and stored through the existing secure credential path.
