# Savaru Affixes (Fabric 1.21.1)

MVP: rarities + affixes stored in CUSTOM_DATA + tooltip + commands + combat effects.

## Commands
- `/savaru_affixes give_mythic minecraft:netherite_sword`
- `/savaru_affixes reroll` (hold item in main hand)

## Build (Windows)
```bat
cd /d "C:\Users\User\Downloads\savaru_affixes_fabric1211_BOOTSTRAP_FULL_v10_COMBAT"
set "JAVA_HOME=C:\Program Files\Eclipse Adoptium\jdk-21.0.9.1-hotspot"
set "PATH=%JAVA_HOME%\bin;%PATH%"
build-with-bootstrap.bat
```
Output: `build\libs\savaru-affixes-0.1.0.jar`


## Combat pipeline
Route A enabled: modifies original melee hit via mixin into PlayerEntity#attack.
