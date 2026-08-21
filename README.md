

# «Don't Cry Baby» Fix for Mercenaries 2: World in Flames 


![Main picture](https://github.com/FrostMoonEcho/Mercenaries_2_Comprehensive_Fix_Dont_Cry_Baby/blob/main/assets/Main.png?raw=true)

  
  
## Navigation

 - [What you can find in this patch](#what-you-can-find-in-this-patch)
 - [Prerequisites](#prerequisites)
 - [Installation](#installation)
 - [Pro Tips for Best Quality](#pro-tips-for-best-quality)

## What you can find in this patch
The collection includes:
- Fix for blur caused by DoF
- Fix which disables aim assist
- Fix which enables permanent death for NPCs
- Improvement which increases the fine for killing an NPC to $25,000
- Fix for a bug which happens after a kick or a collision with an NPC, it's like it gets up and then falls dead again
- Corpses don't disappear immediately anymore
- Various fixes for shadows
- All outfits in your wardrobe will be unlocked including:
	- Basic outfits
	- Cheat outfits such as Ewan, Misha, Fiona and Eva
	- Pre-order only outfits
- Optionally you can download my ReShade preset.

## Prerequisites
![Preview](https://github.com/FrostMoonEcho/Mercenaries_2_Comprehensive_Fix_Dont_Cry_Baby/blob/main/assets/Preview.png?raw=true)


**(!)** It's extremely important to check your serial numbers on an every step, because this patch expects only certain ones. Otherwise, there is a big chance that you will experience bugs/crashes and other bad stuff.

**(!!)** This patch was tested in a single-player mode only.

**Nice things that you need to start:**
- RPCS3 Emulator ([Download](https://rpcs3.net/download) or [the build which I used for testing](https://github.com/RPCS3/rpcs3-binaries-win/releases/download/build-8fd2ae954d80d867fd2d58795848c77d1954574b/rpcs3-v0.0.42-19815-8fd2ae95_win64_msvc.7z))

- Mercenaries 2: World In Flames dump

  > **Important:** the serial number should be **BLES00323**
  > Also known as Mercenaries 2 - WiF (Europe) (En,Fr,De,Es,It,**Ru**)

- Update v1.03 for Mercenaries 2 
  > **Important:** should be for **BLES00323**
  
- Blow it Up Again Pack (DLC)
  > **Important:** the serial number should be **NPEB00053**

- `(optionally)` ReShade for better graphics  ([download](https://reshade.me/))
- `(optionally)` Lossless Scaling for frame generation and scaling  ([download](https://store.steampowered.com/app/993090/Lossless_Scaling/))
- `(optionally)` Gamepad for better experience 


## Installation

 - Download RPCS3 and install the base game. Make sure that:
	 - The serial number of the game is **BLES00323**
	 - You created Custom configuration from Database Settings
	 - You created Custom configuration for gamepad
	 
 - Install the update v1.03 and DLC. Make sure that:
 ![Preview](https://github.com/FrostMoonEcho/Mercenaries_2_Comprehensive_Fix_Dont_Cry_Baby/blob/main/assets/Packages.png?raw=true)

 - Download [BLES00323_patch.yml](/BLES00323_patch.yml) from this repository and put it in the folder `<RPCS3_folder>/patches`. So your structure should look like: 
 ```text
		RPCS3 
		├── patches
			├── BLES00323_patch.yml
```

- **Right-click on the game** -> **Manage game patches** -> **Enable the following game patches**:
 ![Preview](https://github.com/FrostMoonEcho/Mercenaries_2_Comprehensive_Fix_Dont_Cry_Baby/blob/main/assets/Patches.png?raw=true)

- Set **your RPCS3 upscaling value** in `Self-Shadowing Fix`

You are ready to blow someting up!

## Pro Tips for Best Quality
I recommend to use Vulkan and enable the following settings for the game:

![RPCS3 Settings](https://github.com/FrostMoonEcho/Mercenaries_2_Comprehensive_Fix_Dont_Cry_Baby/blob/main/assets/RPCS3_3.png?raw=true)

Don't use blindly 300% for upscaling. It costs a lot!

### Use excessive upscaling in RPCS3
Let's assume the following:
- You set the game upscaling resolution to 225% (or any resolution that will be more than the one for window)
- You launched the game in the window mode with resolution 1280x720

Then your game will be automatically downsampled by your system and this will improve anti-aliasing in the game.

You have to configure upscaling in the game settings. (Example is available on the previous screenshot)

You have to enable the window-mode for the game:

![RPCS3 Settings](https://github.com/FrostMoonEcho/Mercenaries_2_Comprehensive_Fix_Dont_Cry_Baby/blob/main/assets/RPCS3_2.png?raw=true)

And configure the main window parameters:

![RPCS3 Settings](https://github.com/FrostMoonEcho/Mercenaries_2_Comprehensive_Fix_Dont_Cry_Baby/blob/main/assets/RPCS3_1.png?raw=true)

Then restart RPCS3.

### Use Lossless Scaling to scale the window and generate 60 fps
The next questions are how to play in a full-screen mode preserving the quality and how to have more than 30fps?
You have to use ([Lossless Scaling](https://store.steampowered.com/app/993090/Lossless_Scaling/)) to get to this point. Here are the settings that I use:

![Lossless Scaling Settings](https://github.com/FrostMoonEcho/Mercenaries_2_Comprehensive_Fix_Dont_Cry_Baby/blob/main/assets/LS.png?raw=true)

But be careful, because the settings that will work best on your hardware will be different. Use this as a hint.

### Use ReShade to improve graphics
- Download [my ReShade Preset](ReShadePreset.ini) 
- [Download](https://reshade.me/) and install ReShade. 
- Choose your `rpcs3.exe`
- Choose Vulkan
- Choose the preset and install it
- Then when you launch the game you should press `Home` button and make sure that all effects are enabled.
