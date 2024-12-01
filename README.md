# FNF - Melody Engine

**MelodyEngine** is a modified version of the popular [**Psych Engine**](https://github.com/ShadowMario/FNF-PsychEngine) created with the goal of making FNF modding over the base Funkin' content easier and more customizable. The engine provides users with full control over the base game through softcoding, allowing them to easily create mods and adjust the game's visual themes.

## Installation

1. **Download Source Code**: Since I do NOT know how to use git, I posted the source code on a google drive folder, which can be found [here](https://drive.google.com/drive/u/1/folders/1is07b16H-FujScjXZdZTf0PHhYonZhdq).

2. **Download Haxe**: To get started, you'll need to download [Haxe](https://haxe.org/). We recommend using version 4.3.4 to 4.3.6 (the most recent stable version at the time).

3. **Obtain SScript**: SScript (SuperlativeScript) is the game's HaxeScript parser library. However, it has been taken down. You can still obtain it by going to [Cobalt's SScript Archive](https://github.com/CCobaltDev/SScript-Archive). Download **version 19.0.618** and move the `SScript-19,0,618.zip` file into the source code repository after unzipping it.

4. **Follow Building Instructions**: After obtaining SScript, refer to the [building instructions](./BUILDING.md) for detailed setup steps.

## Compiling

To compile the engine, the necessary files for Windows are located in the `compile` folder. However, to compile for other operating systems, you can run:

```
haxelib run lime test [your-os]
```

For example, for a Linux build of MelodyEngine, execute:

```
haxelib run lime test linux
```

This will compile and test the engine for your specific operating system.

## Softmodding/Lua Usage

- To tell if you're using MelodyEngine, you can use the `versionME` variable in lua scripts, similar to how you would normally use the `version` variable to track what version of Psych Engine you're using. All Psych `version` variables have now been renamed to `versionPE` here.

- In softcoded modpacks, you would normally use `pack.png` and `pack.json` to store metadata and the mods menu icon in vanilla Psych. This has been changed in melodyEngine to a more traditional `icon.png` and `meta.json` [thanks Rozebud for the filename idea].

- Otherwise you can refer to [this](https://github.com/BobbyDrawz/psych-engine-modding-docs-unofficial/blob/main/README.md) for modding help.

## Softmodding/Lua Usage

Just like base FNF, this engine runs on the Apache 2.0 License. If you want to know more [which i highly doubt], click [here](./LICENSE).

## Credits

- **bobbyDX_** - Lead developer (the only one, in fact)
- **jarekboho** - Created the `ChartingState.hx` modification
- **ledonic** - Made some fixes and worked on porting Weekend 1
- **mikolka** - Recreated the vanilla FNF legacy content

```

               .__             .___                           .__               
  _____   ____ |  |   ____   __| _/__.__. ____   ____    ____ |__| ____   ____  
 /     \_/ __ \|  |  /  _ \ / __ <   |  |/ __ \ /    \  / ___\|  |/    \_/ __ \ 
|  Y Y  \  ___/|  |_(  <_> ) /_/ |\___  \  ___/|   |  \/ /_/  >  |   |  \  ___/ 
|__|_|  /\___  >____/\____/\____ |/ ____|\___  >___|  /\___  /|__|___|  /\___  >
      \/     \/                 \/\/         \/     \//_____/         \/     \/ 

                    just have fun the way you want to
```
