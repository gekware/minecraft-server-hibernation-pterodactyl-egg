# PterodactylEgg-minecraft-server-hibernation
 A egg for [MSH](https://github.com/gekigek99/minecraft-server-hibernation) minecraft server  
 This is a modification of [Parkervcp Minecraft EGG](https://github.com/parkervcp/eggs/tree/master/minecraft/java)  
## Description
 This Egg will create a minecraft server that will only run when a player is online, the servers can be started by joining  
 the server.  
 More info and full credit to [MSH](https://github.com/gekigek99/minecraft-server-hibernation) and [Parkervcp Minecraft EGG](https://github.com/parkervcp/eggs/)
 
 ## API to generate config files
 Documentation at [EBG API](https://docs.ebg.pw/#msh-configgenerator)  
 The Egg install script simply runs:
 ```sh
 curl -o config.json -X GET "https://api.ebg.pw/api/v1/MSH-ConfigGenerator/2-3-3?FileName=${SERVER_JARFILE}&ServerType=${VENDOR}&Version=${MINECRAFT_VERSION}&RAM=${SERVER_MEMORY}&Port=${SERVER_PORT}&StopTime=${TBSES}"
 ```
 
[Source to the API](https://github.com/EBG-PW/EBG-API-Plugins/tree/master/MinecraftServerHibernationConfigGenerator)  