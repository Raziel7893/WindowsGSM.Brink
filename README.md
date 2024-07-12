# WindowsGSM.GroundBranch
🧩WindowsGSM plugin that provides GroundBranch Dedicated server

## PLEASE ⭐STAR⭐ THE REPO IF YOU LIKE IT! THANKS!

### Notes
- If IP Connect works but no Server Listing, try setting your public IP inside Edit Config Windows under Server IP
- If local connections work but not External: see chapter Portforwarding

### WindowsGSM Installation: 
1. Download  WindowsGSM https://windowsgsm.com/ 
2. Create a Folder at a Location you wan't all Server to be Installed and Run.
3. Drag WindowsGSM.Exe into previously created folder and execute it.

### Plugin Installation:
1. Download [latest](https://https://github.com/Raziel7893/WindowsGSM.GroundBranch/releases/latest) release
2. Either Extract then Move the folder **GroundBranch.cs** to **WindowsGSM/plugins** 
    1. Press on the Puzzle Icon in the left bottom side and press **[RELOAD PLUGINS]** or restart WindowsGSM
3. Or Press on the Puzzle Icon in the left bottom side and press **[IMPORT PLUGIN]** and choose the downloaded .zip

### Official Documentation
🗃️ Didn't find any documentation yet. Please Let me know if you came accros one

### The Game
🕹️ https://store.steampowered.com/app/16900/GROUND_BRANCH/

### Dedicated server info
🖥️ https://steamdb.info/app/476400/info/

### Port Forwarding (YOU NEED THIS, TO BE ABLE TO CONNECT FROM THE INTERNET(only for servers/pcs at home):
- If You don't know How: portforward.com
- 7777 UDP - Default Game Port
- 27015 UDP - Default QueryPort

### Files To Backup
- Save Gane (You could only save serverfiles/GroundBranch/Saved , but that includes many big logs)
  - WindowsGSM\servers\%ID%\serverfiles/GroundBranch/Saved/SaveGames
  - WindowsGSM\servers\%ID%\serverfiles/GroundBranch/Saved/Config/WindowsServer
- WindowsGSM Config
  - WindowsGSM\servers\%ID%\configs

### Available Params
All these params are automatically set by WGSM
- -port=  	 	                 can be change and working (Change via WGSM settings)
- -queryPort=                    can be change and working (Change via WGSM settings)
- -MultiHome=					 Change via WGSM settings, most games need your local AdapterIP, but if you have issues with serverlisting you may try your online IP
- -LOCALLOGTIMES -log            creates logfiles in serverId\serverfiles\GroundBranch\Saved\Logs

### How can you play with your friends without port forwarding?
- Use [zerotier](https://www.zerotier.com/) folow the basic guide and create network
- Download the client app and join to your network
- Create static IP address for your host machine
- Edit WGSM IP Address to your recently created static IP address
- Give your network ID to your friends
- After they've joined to your network
- They can connect using the IP you've created eg: 10.123.17.1:7777
- Enjoy

### Support
[WGSM](https://discord.com/channels/590590698907107340/645730252672335893)

### Give Love!
[Buy me a coffee](https://ko-fi.com/raziel7893)

[Paypal](https://paypal.me/raziel7893)

### License
This project is licensed under the MIT License - see the <a href="https://github.com/raziel7893/WindowsGSM.GroundBranch/blob/main/LICENSE">LICENSE.md</a> file for details

### Thanks
Thanks to ohmcodes for the Enshrouded and Palworld Plugins which i used for guidance to create this one
