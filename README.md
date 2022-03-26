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
- Copy & Paste GB parameter into a `run.txt` file then save as `run.bat` file
<details>
<summary>GB Parameters</summary>

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
</details>

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
- Go to `Premiums/<designated server>/Skripts` copy every file
- Go to `<your server folder>/plugins/Skript/scripts` paste
- You can do `/sk reload scripts` or restart the server

# Witch Skripts do what
***Note: Skripts not listed are no longer use or non-functional***
<details>
    <summary>chat.sk</summary>
    Formats the chat to include: Ranks, Item formatting ([item]), Player Statics, Pinging, and Message Blocking (Includes set words + Preventing muted players from messaging) 
</details>
<details>
    <summary>core.sk</summary>
    Handles first joins, joins/quits, bossbars, and basic commands such as: `/spawn`, `/tp`, and `/clearlag`
</details>
<details>
    <summary>crates.sk</summary>
    Contains the necessary events and commands to make crates at spawn work. 
</details>
<details>
    <summary>daily.sk</summary>
    A daily reward system for logging on. Uses our DiSky "API" to make sure the player is linked via Discord, and makes sure to give them rewards. 
</details>
<details>
    <summary>disky.sk</summary>
    <pre>You do need to make a bot if not already, and put the API key in from discord development panel </pre>
    This is our DiSky "API". It hosts our bots and connects them to the server. It keeps tracking of linked players, and regular players. It fetches data from Minecraft and presents them on Discord with embeds and or text via commands. There are various commands and discord commands such as: `/link`, `/unlink`, `.link`, `!health`, `!reactions`, `!rules`, `!purge`, `.suggestion`, `.istop`, and `.baltop. *(Note: `!` is an admin command, and `.` is a global command, anyone can use it)*.
</details>
<details>
    <summary>donor.sk</summary>
    Keeps track of donations from Tebex. It hosts an updating npc with the recent donor at spawn. Though we don't use this often. 
</details>
<details>
    <summary>eco.sk</summary>
    Hosts most of our economy commands, balance leaderboards, and use of banknotes. Players can also withdraw their money into banknotes, and admins can handel any players balance or gems. 
</details>
<details>
    <summary>gemshop.sk</summary>
    A GUI shop that allows players to buy various items with their gems. 
</details>
<details>
    <summary>island.sk</summary>
    <pre>This Skript needs a target world, to create this world do `/mv create ul_islands normal -g 
    VoidGenerator:PLAINS -t FLAT`</pre>
    This behemoth Skript handles ALL island generations, island setups, island co-ops, island chatting, island bounds, island homes, island values, island resetting, island visiting/island control, island upgrades, island leaderboard data, and placement of island value blocks. 
</details>
<details>
    <summary>kits.sk</summary>
    A GUI that allows people to get armor sets every set amount of time.
</details>
<details>
    <summary>leaderboards.sk</summary>
    This confusing Skript that goes through island value block data, reaction data, and balance data. To determine the top 10 players and their values for the respective data type. It updates every 15m to reduce lag. It has GUI and holograms to show this outputted and formatted data. It is also sent to our DiSky "API". 
</details>
<details>
    <summary>mobdrops.sk</summary>
    A simple Skript to give more items to certain mob drops. 
</details>
<details>
    <summary>mobkills.sk</summary>
    This Skript handles our crystal system. These "crystals" give gems or cash. They are obtained through killing mobs. 
</details>
<details>
    <summary>npc.sk</summary>
    A Skript that connects to Citizens NPCs to make them better! This Skript gives citizens at spawn GUIs or commands to execute when clicked. 
</details>
<details>
    <summary>payouts.sk</summary>
    A GUI that shows past seasons payouts. This GUI is used when clicking a enchanting table. 
</details>
<details>
    <summary>protection.sk</summary>
    Another behemoth Skript that protects ALL islands and spawn. It contains many checks to prevent: Placing, Breaking, Stealing dropped items, Opening storage containers and or appliances, PvE & PvP, Crop trample, Bows, Offhand, Armor stands, Robots, and Bound Exiting.
</details>
<details>
    <summary>punish.sk</summary>
    A punishment system to ban, tempban, mute, tempmute, and kick players.  
</details>
<details>
    <summary>reactions.sk</summary>
    A chat game created by @NinjaTalonYT (Talon#5793) that contains games such as: math, unscramble, and  first to type. It was supposed to be released on the Minehut marketplace. It is very customizable and effective. 
</details>
<details>
    <summary>redeem.sk</summary>
    This Skript is to redeem codes around spawn to get rewards. By clicking the signs or typing the command in. 
</details>
<details>
    <summary>redis.sk</summary>
    Our connection to our redis database to allow for cross-server staff chat from hub to gamemodes. 
</details>
<details>
    <summary>robotc.sk</summary>
    Handles the GUI menus for robots. Such as coloring, direction, data, and upgrades for them.
</details>
<details>
    <summary>robotf.sk</summary>
    This one handles the command, placing, and breaking of the robots.
</details>
<details>
    <summary>robotf2.sk</summary>
    Handles all logic and what robots do. 
</details>
<details>
    <summary>rules.sk</summary>
    A GUI that showcases our rules on PREMIUMS servers. From little to big offences.  
</details>
<details>
    <summary>scoreboard.sk</summary>
    Displays our scoreboard, shows player data, and server data to the player via a scoreboard. 
</details>
<details>
    <summary>sell.sk</summary>
    Allows the player to sell items for our custom currency. By either `/sell` or `/sell hand`.
</details>
<details>
    <summary>sellwand.sk</summary>
    A custom sellwand that was built to sell items from chest to our custom currency.
</details>
<details>
    <summary>shop.sk</summary>
    A GUI shop built by @KingPr0o7 (KingPr0o7#0007) to let players BUY and SELL items for our custom currency.
</details>
<details>
    <summary>spawnfarm.sk</summary>
    Allows for automatic farming at spawn (If players break crops, it replants them). 
</details>
<details>
    <summary>staff.sk</summary>
    Various staff/admin commands for the server.
</details>
<details>
    <summary>tab.sk</summary>
    Just like scoreboard, just shows different information in TAB.
</details>
<details>
    <summary>welcome.sk</summary>
    Automatic welcoming players to the server. 
</details>

<h1 align="center">DO NOT DISTRIBUTE - PREMIUMS</h1> 
