# PterodactylEgg-minecraft-server-hibernation

- [Versions](#Versions)
- [Info](#Info)
- [Description](#Description)
- [Host your own binarys](#Host-your-own-binarys)
- [Known issues](#Known-issues)

## Versions
The EGG auto updates MSH every time you click "Reinstall Server" at your settings tab. However, sometimes stable DEV versions will be used.  
[MSH-EGG](https://github.com/gekware/minecraft-server-hibernation-pterodactyl-egg/blob/main/egg-paper-on-demand-new): All JAVA Versions (Hotspot, J9 and Shenandoah)  
[MSH-EGG-Deprecated](https://github.com/gekware/minecraft-server-hibernation-pterodactyl-egg/blob/main/deprecated/egg-paper-on-demand.json): The old version of the egg for MSH Versions prior 2.4.6  

## Info
 A egg for [MSH](https://github.com/gekware/minecraft-server-hibernation) minecraft server  
 This is a modification of [Parkervcp Minecraft EGG](https://github.com/parkervcp/eggs/tree/master/game_eggs/minecraft/java/paper) and [Parkervcp Forge EGG](https://github.com/parkervcp/eggs/tree/master/game_eggs/minecraft/java/forge/forge)

## Description
 This Egg will create a minecraft server that will only run when a player is online, the servers can be started by joining  
 the server and stops when nobody is online.  
 More info and full credit to [MSH](https://github.com/gekware/minecraft-server-hibernation) and [Parkervcp Minecraft EGG](https://github.com/parkervcp/eggs/)

## Host your own binarys
 Do you want to use your own build of MSH? Thats easy:
 1. Setup a HTTPS werbserver with URL.
 2. Write your URL into the variable "MSH-Download URL" (without the filename)
 3. The names of the files MUST be called as follows:
    - For x86 (64bit): msh_server_new.bin
    - For ARMv8 (64bit): msh_server_new-arm64.bin  
  
If you would like to run the egg on other hardware then look for "arch=$(uname -m)" in the installatiin script and add it below the other archs.

## Known issues
The startup parameters "Hib-Info" and "Hib-Starting" are not working, They are set to read only for now.  
Solution: Edit msh-config with your text. [Issue](https://github.com/gekware/minecraft-server-hibernation/issues/143)  
```json
"InfoHibernation": "My nice text when the server is hibernating",
"InfoStarting": "My nice text when teh server is starting up",
```  
  
The Variable "Vendor" is currently not working, missing start parameter.  
