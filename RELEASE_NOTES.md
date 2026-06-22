# Sharkord Desktop v0.5.14 Beta

## Added

- Adds native two-factor login support for servers requiring TOTP.
- Stores a server-minted remembered-device app password in the existing secure credential store after successful TOTP login.
- Adds profile UI to list and revoke remembered-device app passwords.

## Security

- TOTP codes are not persisted.
- Remembered-device app passwords are stored locally through the existing encrypted credential path.
