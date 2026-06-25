# Sharkord Desktop v0.5.47 Beta

## Fixed

- IP-Sicherheit in der Desktop-App funktioniert mit dem aktuellen Kanuracer Server wieder.
- Desktop erkennt `security.getIpRules`, auch wenn Capability-Daten fehlen/alt sind.
- Desktop nutzt die aktuelle `security.getSecurityEvents` Route.
- IP-Regeln werden aus `{ allowed, blocked }` korrekt in die UI normalisiert.
- `unblockIp` sendet das aktuelle `{ ip }` Payload.
