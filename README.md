# Half-Life Alyx SDK Description
The purpose of this repo is to automate the process of enabling the SteamVR environments tools to be used to create and compile maps for use with Half Life Alyx.  Big credit for this script goes to Gvarados [twitch](https://www.twitch.tv/gvarados) as I learned how to do this by watching his live stream while he set this up and painstakingly recreated it on my own.

# How-To Use
This repo includes a batch (.bat) script that you can run on your machine to faciliate the creation of a Alyx SDK sourcemod.  This can be run as a standalone application that will enable you to use all of the Half-Life Alyx assets to start creating custom Half Life Alyx maps before the official toolkit arrives!  This works because the existing SteamVR environments editor is ALSO based on source 2 and fairly compatible with HL Alyx assets.

## Run the hl-alyx-sdk-setup.bat script
The script tries to locate where your steam/alyx/steamvr installs are located, but should prompt you if any/all of those don't exist.  The script will copy over files that it needs (¬2x48GB) to launch the editor. 

## Follow additional instructions at the end of .bat script

You MUST download the `.FGD` files required by Half-Life Alyx to load entities into Hammer or none of the entities will show up correctly on your map.  You can download those from [Gvarados1 FGD repo](https://github.com/gvarados1/Half-Life-Alyx-FGD)

## Modify and run Editor launch script
Edit the `launch-hl-alyx.bat` file and update the path to match your `sourcemods` directory ***if needed***.  Double click the bat file to launch the editor.

# Known issues
- Navmesh doesn't appear to be working - see other guides for fixes
- Running in editor WILL crash the editor
- Random crashes

# Compiling maps
Maps *should* compile from the hammer editor, note that you will have to COPY them over to your REAL Half-Life Alyx maps folder in order to actually try them out.  This is possible with +sv_cheats and the `map` command in the console of Half Life Alyx.  

# Why?
Valve initially promised us SDK tools that would launch side-by-side with Half-Life Alyx, but it turns out that wasn't the case, although they have now informed us they are hard at work at releasing the SDK and/or editor.
Turns out they already shipped the SDK tools on Dota 2, Destinations and SteamVR Home which happen to be compatible with HL:A.

# DISCLAIMER
Not everything works, probably lots of it doesn't, you will most likely encounter crashes periodically.  Save often.

I'm not responsible for anything that happens to your machine if you run this script, please don't sue me.  In addition I'm a complete novice to the Hammer editor, so I have no notion of what is/isn't functioning properly when it comes to that,  but basic world building and assett dropping seems to be working perfectly fine. 
