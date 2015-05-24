# HudPixel UpToDate
**Advanced Update Prevention and Handling Technique for the [HudPixel Minecraft Mod](https://github.com/palechip/HudPixel/)**

### How it works
##### `update.json`
This file is unique and contains information about which version is the latest in a specific channel and for a specific Minecraft verison. It also contains download-links and fields to state the reason for the update.
This file is downloaded by every version of the mod.

#### `version/v*.*.*.*.json`
Each released stable version gets a file in this pattern. Only the version which the file belongs to will download it and must be able to read it. This file contains version information of other components saved in this repository. It also has switches for remotely deactivating the version in case of severe bugs or disallowed features.

#### `games/v*.json`
Remote equivalent of [games.json](https://github.com/palechip/HudPixel/blob/master/src/main/resources/HudPixelUpToDateFiles/games.json). Holds information about Hypixel Games and the used Components.
