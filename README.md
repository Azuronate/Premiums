# Premiums Network
This is a github with all source code and internal documents of PREMIUMS Servers*. Including Images, Skripts, Plugins, Configs, Worlds, and more. 

*Relates to the network, such as Hubs, Skyblock, Farming, and more. 

# How to install
**Installing a local Paper server**
- Install [Java 17](https://www.oracle.com/java/technologies/downloads/#java17)
- Create a folder to put the below items in
- Install [PaperMC 1.17.1](https://papermc.io/legacy)
- Rename the downloaded jar to `paper.jar`
- Copy & Paste GB parameter (Below of all of this) into a `run.txt` file then save as `run.bat` file
- Delete the `run.txt` file
- Run the `run.bat` file
- Once the first set of files appears, close the cmd line
- Open the `eula.txt` file and agree to it by turning `eula=false` -> `eula=true`
- Save the `eula.txt` file
- Run the `run.bat` file and startup the server (You will run this file every time to boot up the server)
**Connecting to the server**
- Open a new cmd line in admin mode
- Type `ipconfig` hit enter
- Copy the address after this: `IPv4 Address. . . . . . . . . . . :`
- Direct connect in Minecraft using that address
**Installing the plugins**
***Made sure you have cloned or downloaded the files from the GitHub***
- Go to `Premiums/<designated server>/plugins` and copy every file
- Go to `<your server folder>/plugins` and paste the copied plugins
- Restart the server, so that it can generate default configs
- Once it has restarted go to `Premiums/<designated server>/plugins/configs`
- Make sure you go to every config folder, copy the files, and replace them within designated plugin config folders.
**Installing worlds**
- Go to `Premiums/<designated server>/Worlds` and copy every folder
- Go to `<your server folder>/` and paste
- Restart the server
- Once rebooted, type `/mv import <world>`
- To teleport type `/mvtp <world>`
**Installing Skripts** 
- Go to `Premiums/<designated server>/skripts` copy every file
- Go to `<your server folder>/plugins/skript/scripts` paste
- You can do `/sk reload scripts` or restart the server

```
1GB Server:
java -Xmx1024M -Xms1024M -jar paper.jar nogui
PAUSE

2GB Server:
java -Xmx2048M -Xms2048M -jar paper.jar nogui
PAUSE

3GB Server:
java -Xmx3072M -Xms3072M -jar paper.jar nogui
PAUSE

4GB Server:
java -Xmx4096M -Xms4096M -jar paper.jar nogui
PAUSE
```

<h1 align="center">DON'T DISTRIBUTE</h1> 
