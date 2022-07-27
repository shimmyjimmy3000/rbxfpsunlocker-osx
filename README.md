# rbxfpsunlocker-osx - UI [![License](https://img.shields.io/badge/License-GPL3.0-green.svg)](https://github.com/lanylow/rbxfpsunlocker-osx/blob/main/LICENSE) ![OS](https://img.shields.io/badge/OS-macOS-green.svg) [![Github All Releases](https://img.shields.io/github/downloads/lanylow/rbxfpsunlocker-osx/total.svg)]()

The first Roblox FPS unlocker for macOS. This UI branch is the first major update to the FPS unlocker. This has been tested and working both on Intel-based Macs and on M1 Macs using Rosetta 2. This update features a new user interface, along with features such as scanning for Roblox and automatically setting the FPS cap. If you want a lighter command line interface then go to the [main](https://github.com/lanylow/rbxfpsunlocker-osx/tree/main) branch.

## Setup
*Note: you must have `sudo` permissions in order to do the steps below. If you do not have `sudo` permissions, either change your account or add yourself to the sudoers file.*
1. Download the latest release from here: https://github.com/lanylow/rbxfpsunlocker-osx/releases.
2. Open the .dmg file and drag and drop the FPS unlocker to your Applications folder.
3. If you want, you can drag the application into your Launchpad on your Dock.

## Compiling (advanced)

1. Open Terminal and clone the repository and change directory.

```
git clone -b ui https://github.com/lanylow/rbxfpsunlocker-osx/ && cd rbxfpsunlocker-osx
```

2. Compile in Xcode by pressing Command+B.


## Disclaimer

**Use at your own risk**, this is new and still in-development, however this uses the same computational/theoretical method as [axstin](https://github.com/axstin/)'s [rbxfpsunlocker](https://github.com/axstin/rbxfpsunlocker) which has been cleared by Roblox as safe to use.

Please note that this is a FPS *unlocker* and not a FPS *booster* and if your frame rate is the same or below 60 FPS, then your machine is not powerful enough to run Roblox at more than 60 FPS. Heavy usage of system resources may occur because of the higher frame rate.

## Credits

 - @fjij - For bringing the idea to our attention
 - @lanylow - For reverse engineering and coding the unlocker
 - @SeizureSaladd - For testing the code and coding the front-end

