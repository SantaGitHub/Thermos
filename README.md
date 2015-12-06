# Cauldron 

![Minecraft Forge v10.13.4.1566][forge]
![Minecraft v1.7.10][mc]
![Java JDK v1.8][java]

### Continuation of KCauldron minecraft server

This github was created due to the previous developer for KCauldron being missing for weeks - sometimes months - at a time.  When the dev was missing his gitlab would go offline making it "feel" like the project was abandoned completely.

This repo was based on KCauldron 1492 Build 152.  Some extra patches were added and cherry picked in order to improve and fix up some of the small little flaws that were inherent in the 152 build.

## Downloads
You can download the pre-built packages from https://github.com/spannerman79/KCauldron/releases
I'd suggest that you look at the release notes before downloading.

## Build Requirements
* Java 8 JDK
* `JAVA_HOME` defined on your OS

## Building Cauldron
* Checkout project
  * You can use IDE or clone from console:
  `git clone https://github.com/spannerman79/KCauldron.git`
* Init submodules
  * Since this project uses two other projects we need to download them as well
  `git submodule update --init --recursive`
* Start build process
  * This process downloads minecraft and apply patches
  * If you have gradle integration in IDE - you can still use gui
  `./gradlew setupCauldron jar`

## Updating sources
If you've once checkout source - you not need to do it again
* Update sources
  * `git pull origin master`
* Re apply patches & build binaries
  * `./gradlew clean setupCauldron jar`

[forge]: https://img.shields.io/badge/Minecraft%20Forge-v10.13.4.1566-green.svg "Minecraft Forge v10.13.4.1566"
[mc]: https://img.shields.io/badge/Minecraft-v1.7.10-green.svg "Minecraft 1.7.10"
[java]: https://img.shields.io/badge/Java%20JDK-v1.8-blue.svg "Java JDK 8"