# mauzcraft-java-edition
Mauzcraft Java Edition is a sandbox block-building game inspired by classic voxel adventures. Explore infinite worlds, mine resources, build massive structures, survive dangerous nights, and create your own adventures in the world of Mauzcraft.

# Mauzcraft Java Edition

Desktop-Java-Edition als eigenstaendiges Multi-File-Projekt (Gradle).

## Start

### LWJGL (Gradle Wrapper)

```powershell
cd JavaEdition
.\gradlew.bat run
```

Hinweis: Erstes `run` laedt Dependencies (Maven Central).

## Java 26 Hinweise

Wir setzen `--enable-native-access=ALL-UNNAMED` und `-Dorg.lwjgl.system.JNINativeInterfaceSize=233` automatisch (siehe `JavaEdition/build.gradle`), um LWJGL-Warnungen unter Java 26 zu reduzieren.

## Texturen

Lege Block-Texturen hier ab (am besten 16x16 PNG):
- `JavaEdition/assets/textures/blocks/grass.png`
- `JavaEdition/assets/textures/blocks/dirt.png`
- `JavaEdition/assets/textures/blocks/stone.png`
- `JavaEdition/assets/textures/blocks/wood.png`
- `JavaEdition/assets/textures/blocks/sand.png`
- `JavaEdition/assets/textures/blocks/cobblestone.png`
- `JavaEdition/assets/textures/blocks/planks.png`
- `JavaEdition/assets/textures/blocks/bricks.png`
- `JavaEdition/assets/textures/blocks/clay.png`
- `JavaEdition/assets/textures/blocks/snow.png`
- `JavaEdition/assets/textures/blocks/leaves.png`
- `JavaEdition/assets/textures/blocks/water.png`

Wenn Dateien fehlen, benutzt Mauzcraft prozedurale Platzhalter-Texturen.

## Saves

Welten werden gespeichert unter:
- Windows: `%APPDATA%\\MauzcraftJava\\saves`

Im Startmenue:
- Welt anklicken → `Laden / Start`
- Seed tippen (Zahlen) und/oder Name tippen → `Neue Welt + Start`
- `Welt loeschen` entfernt den Save-Ordner.
