# Premiums Network
This is a github with all source code and internal documents of PREMIUMS Servers*. Including Images, Skripts, Plugins, Configs, Worlds, and more. 

*Relates to the network, such as Hubs, Skyblock, Farming, and more. 

# How to install
**Installing a local Paper server**
> You don't have to do this if you're using a server provider (Ex: Minehut). Though it has to provide Paper since our servers were built on that. 
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
- Run the `run.bat` file and startup the server **(You will run this file every time to boot up the server)**

**Connecting to the server (Paper only)**
> For a server provider use the ip given to you
- Open a new cmd line in admin mode
- Type `ipconfig` hit enter
- Copy the address after this: `IPv4 Address. . . . . . . . . . . :`
- Direct connect in Minecraft using that address

**Installing the plugins**
> Made sure you have cloned or downloaded the files from the GitHub
- Go to `Premiums/<designated server>/plugins` and copy every file
- Go to `<your server folder>/plugins` and paste the copied plugins
- Restart the server, so that it can generate default configs
- Once it has restarted go to `Premiums/<designated server>/plugins/configs`
- Make sure you go to every config folder, copy the files, and replace them within designated plugin config folders.

**Installing worlds**
> Some worlds like spawns have to have the gamerule `/gamerule randomtickspeed 0` as soon you enter so that leaves don't decay
- Go to `Premiums/<designated server>/Worlds` and copy every folder
- Go to `<your server folder>/` and paste
- Restart the server
- Once rebooted, type `/mv import <world>`
- To teleport type `/mvtp <world>`

**Installing Skripts** 
- Go to `Premiums/<designated server>/skripts` copy every file
- Go to `<your server folder>/plugins/skript/scripts` paste
- You can do `/sk reload scripts` or restart the server

# Witch Skripts do what

<details>
    <summary>Chat.sk</summary>
    Formats the chat to include: Ranks, Item formatting ([item]), Player Statics, Pinging, and Message Blocking (Includes set words + Preventing muted players from messaging) 
</details>
<details>
    <summary>Core.sk</summary>
    Handles first joins, joins/quits, bossbars, and basic commands such as: `/spawn`, `/tp`, and `/clearlag`
</details>
<details>
    <summary>Crates.sk</summary>
    Contains the necessary events and commands to make crates at spawn work. 
</details>
<details>
    <summary>Daily.sk</summary>
    A daily reward system for logging on. Uses our DiSky "API" to make sure the player is linked via Discord, and makes sure to give them rewards. 
</details>
<details>
    <summary>Disky.sk</summary>
    > You do need to make a bot if not already, and put the API key in from discord development panel

    This is our Disky "API". It hosts our bots and connects them to the server. It keeps tracking of linked players, and regular players. It fetches data from Minecraft and presents them on Discord with embeds and or text via commands. There are various commands and discord commands such as: `/link`, `/unlink`, `.link`, `!health`, `!reactions`, `!rules`, `!purge`, `.suggestion`, `.istop`, and `.baltop. *(Note: `!` is an admin command, and `.` is a global command, anyone can use it)*.
</details>
<details>
    <summary>Donor.sk</summary>
    Keeps track of donations from Tebex. It hosts an updating npc with the recent donor at spawn. Though we don't use this often. 
</details>
<details>
    <summary>Eco.sk</summary>
    Hosts most of our economy commands, balance leaderboards, and use of banknotes. Players can also withdraw their money into banknotes, and admins can handel any players balance or gems. 
</details>
<details>
    <summary>Gemshop.sk</summary>
    A GUI shop that allows players to buy various items with their gems. 
</details>
<details>
    <summary>Island.sk</summary>
    > This skript needs a target world, to create this world do `/mv create ul_islands normal -g 
    VoidGenerator:PLAINS -t FLAT`

    This behemoth skript handles ALL island generations, island setups, island co-ops, island chatting, island bounds, island homes, island values, island resetting, island visiting/island control, island upgrades, island leaderboard data, and placement of island value blocks. 
</details>

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
