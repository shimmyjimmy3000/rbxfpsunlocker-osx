# rbxfpsunlocker-osx [![License](https://img.shields.io/badge/License-GPL3.0-green.svg)](https://github.com/lanylow/rbxfpsunlocker-osx/blob/main/LICENSE) ![OS](https://img.shields.io/badge/OS-macOS-green.svg) [![Github All Releases](https://img.shields.io/github/downloads/lanylow/rbxfpsunlocker-osx/total.svg)]()

The first Roblox FPS unlocker for macOS. This is a very simple and unpolished FPS unlocker with more updates to come. This has been tested and working both on Intel-based Macs and on M1 Macs using Rosetta 2.

## Setup
1. Download the latest release from here: https://github.com/lanylow/rbxfpsunlocker-osx/releases.
2. Extract `rbxfpsunlocker.zip` by double clicking on it, if it wasn't extracted automatically.
3. Place `rbxfpsunlocker` in any folder you want to keep it in.
4. Right click on `rbxfpsunlocker`, then press the Option key, and finally click "Copy rbxfpsunlocker as file name"
5. In a text editor, paste the text in, then add `sudo .` before it. example:
 
```
sudo ./Users/MyUser/Downloads/rbxfpsunlocker
```

6. Then add the FPS cap followed by a space after it. The cap is whatever framerate is desired, e.g. 90, 120, 144, etc. If no framerate is supplied it will automatically be set to 120.

It should look like this, with 999 FPS an `
```
sudo ./Users/MyUser/Downloads/rbxfpsunlocker 999
```
This is the terminal command you will use to run `rbxfpsunlocker`. **Note:** If you move `rbxfpsunlocker` to another folder, you will need to change the path.

8. Open the Terminal App using one of two methods:
	* Press Command + Space, type in `Terminal`, then press enter on the Terminal app. 
	* Go to the Applications then into the Utilities folder. Open Terminal.
9. With a Roblox game open, copy and paste the command into Terminal. Enter your password in if it's asked for.

You must run the command if you leave a Roblox game and join a new one, and after launching Roblox for the first time after logging into macOS. Refer to the sections below to create either a terminal or app shortcut to make the process more convenient. 

### Creating a Terminal shortcut

In this section you will create define alias, a terminal shortcut with a name and command. Entering the name into the terminal will run the command. 
1. In Finder, press Command + Shift + G and enter in `~` (copy and paste that in if necessary), it should say `Go to:` followed by the path to your user folder. Press enter or click on it. 
2. You will need to edit a hidden file. To show hidden files, press Command + Shift + . (period). Then locate the file `.zshrc`. This is the file where Terminal aliases are defined among other things.
3. Open `.zshrc` with a text editor, you may need to right click then press `Open With > Other` and locate the editor you wish to use.
**If there's any text, don't remove it. Write below all the text in new lines.** Write a new line write an alias like this:
```
alias roblox='sudo ./Users/MyUser/Downloads/rbxfpsunlocker 999'
```
The name of the alias is `roblox` but it you can name it whatever you want. Keep the exact format, the terminal command is in single quotation marks and there are no spaces next to `=`. You can create as many alias as you want in separate lines for different framerates.
 
4. Open the Terminal app **(restart Terminal if it's running in order for the alias to apply)**. Enter in the name you chose for your alias and the command should run. In this case, writing `roblox` then hitting enter should run `rbxfpsunlocker` with a cap of 999.

### Creating an App shortcut
In this section you will create a shortcut using the built-in Shortcuts app. **The Shortcuts app is only available on macOS versions, Monterey or newer.**

1. Open the Shortcuts app using one of two methods:
	* Press Command + Space, type in `Shortcuts`, then press enter on the Terminal app. 
	* Go to the Applications folder and open Shortcuts.
2. Create a new shortcut by pressing the + button in the title bar, then search for `Run Shell Script`. 
3. Paste the command in and check `Run as Administrator` (this is required for the command to run. It should look like this:

![Screenshot](ShortcutExample.png)

You can make as many shortcuts as you wish for different framerates. The shortcut can now be launched from either from the Shortcuts app or you can create a shortcut to the Shortcut that can be opened from either the Dock or in Finder:

1. Right click on the shortcut in the shortcuts menu, and press `Add to Dock`. If you wish to have it on the left side of the dock, then continue with the last two steps. 
2. Right click on the shortcut in the Dock, and Click Options > Show in Finder.
3. You can now move the shortcut to any folder you want, or pin it to the dock.

## Compiling (advanced)

1. Open Terminal and clone the repository and change directory.

```
git clone https://github.com/lanylow/rbxfpsunlocker-osx/ && cd rbxfpsunlocker-osx
```

2. Compile. This will fail if you don't have [Xcode Developer tools](https://mac.install.guide/commandlinetools/index.html) installed.

```
make
```

3. Launch the unlocker

```
sudo ./rbxfpsunlocker <cap>
```

## Disclaimer

**Use at your own risk**, this is new and still in-development, however this uses the same computational/theoretical method as [axstin](https://github.com/axstin/)'s [rbxfpsunlocker](https://github.com/axstin/rbxfpsunlocker) which has been cleared by Roblox as safe to use.

Please note that this is a FPS *unlocker* and not a FPS *booster* and if your frame rate is the same or below 60 FPS, then your machine is not powerful enough to run Roblox at more than 60 FPS. Heavy usage of system resources may occur because of the higher frame rate.

## Credits

 - @fjij - For bringing the idea to our attention
 - @lanylow - For reverse engineering and coding the unlocker
 - @SeizureSaladd - For testing the code and coding the front-end

