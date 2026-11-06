# Forge – Installationsdateien

Hier liegen nur die fertigen Installationsdateien der Forge-Apps, kein Quellcode:

| App | Zweck |
|---|---|
| **Pixelforge** | Bildbearbeitung |
| **Vectorforge** | Vektorgrafik |
| **Pageforge** | Layout und Satz |
| **Clipforge** | Videoschnitt |
| **Docforge** | PDF-Bearbeitung |

Jedes Release enthält je App:

- `<Name>_<Version>_x64-setup.exe` und `<Name>_<Version>_x64_en-US.msi` für Windows
- `<Name>-android-arm64.apk` für Android (arm64)
- `<ordner>-latest.json` und `.sig`-Dateien: Darüber finden die installierten Apps neue Versionen und prüfen, dass das Update echt ist.

Die Apps suchen beim Start selbst nach Updates: unter Windows installieren sie sie auf Wunsch direkt, unter Android öffnen sie die neue APK im Browser.

## Signatur unter Windows

Die Windows-Dateien sind mit einem selbst ausgestellten Zertifikat signiert („Marvin Hahl (Forge-Apps)“). Windows kennt es nicht und warnt deshalb beim ersten Start. Wer dem Herausgeber vertraut, kann `forge-codesignatur.cer` aus dem Release als vertrauenswürdigen Herausgeber importieren.

## Lizenz

MIT. Der Quellcode liegt in einem privaten Repository.
