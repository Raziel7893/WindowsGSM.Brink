# WindowsGSM.BRINK
🧩WindowsGSM plugin that provides BRINK Dedicated server

## PLEASE ⭐STAR⭐ THE REPO IF YOU LIKE IT! THANKS!

### Notes
- Steam musst be installed and started once.
- For ServerListing it also needs to be running and logged in apperantly, as the game does not support GSLT
  - as the game is free i recoomend a seperate server account, but using the same account does also work
- If IP Connect works but no Server Listing, you might be missing a portforwarding. look for chapter Portforwarding
- If local connections work but not External: see chapter Portforwarding

### WindowsGSM Installation: 
1. Download  WindowsGSM https://windowsgsm.com/ 
2. Create a Folder at a Location you wan't all Server to be Installed and Run.
3. Drag WindowsGSM.Exe into previously created folder and execute it.

### Plugin Installation:
1. Download [latest](https://https://github.com/Raziel7893/WindowsGSM.Brink/releases/latest) release
3. Either Extract then Move the folder **BRINK.cs** to **WindowsGSM/plugins** 
    1. Press on the Puzzle Icon in the left bottom side and press **[RELOAD PLUGINS]** or restart WindowsGSM
4. Or Press on the Puzzle Icon in the left bottom side and press **[IMPORT PLUGIN]** and choose the downloaded .zip

### Official Documentation
🗃️ https://developer.valvesoftware.com/wiki/Brink_Dedicated_Server

### The Game
🕹️ [https://store.steampowered.com/app/16900/GROUND_BRANCH/](https://store.steampowered.com/app/22350/BRINK/)

### Dedicated server info
🖥️ https://steamdb.info/app/72780/info/

### Port Forwarding (YOU NEED THIS, TO BE ABLE TO CONNECT FROM THE INTERNET(only for servers/pcs at home):
- If You don't know How: portforward.com. sadly nobody mentions what Protocoll so you need to forward both for all 3 ports
- 27015 UDP/TCP - Default Game Port
- 27016 UDP/TCP - Default QueryPort
- 8766 UDP/TCP - Default Steam Auth Port, can be changed by clinging Edit Config, in Server Start Param  

### Files To Backup
- Save Gane (You could only save serverfiles/BRINK/Saved , but that includes many big logs)
  - WindowsGSM\servers\%ID%\serverfiles/Save
- WindowsGSM Config
  - WindowsGSM\servers\%ID%\configs

### Available Params
All these params are automatically set by WGSM and can be changed via Edit Config Window (don't edit the config Windowsgsm.ini manually
- +set si_name $ServerName 
- +set net_ip $ServerIP
- +set net_serverPort $ServerPort
- +set net_serverPortMaster $ServerQueryPort
- +set si_maxPlayers $ServerMaxPlayer
- +set net_serverDedicated 1 
- +set fs_savepath ./ 
- +set net_serverPortAuth 8766  //can be changed via Server Start Param

### Config
- to adjust configs either go to Server Files (clock on Browse => Server Files), got to folder base and adjust autoexec.cfg 
- or add variables to WindowsGSM by clicking Edit Config and modifing the last box Server Start Param
- to set a password modify autoexec.cfg:
  - set si_needpass to 1
  - remove the // infront of g_password and set a password in the quotes

### Not having an full IPv4 adress ( named CCNAT or DSL Light )
No game or gameserver supports ipv6 only connections. 
- You need to either buy one (most VPN services provide that option. A pal uses ovpn.net for his server, I know of nordvpn also providing that. Should both cost around 7€ cheaper half of it, if your already having an VPN)
- Or you pay a bit more for your internet and take a contract with full ipv4. (depending on your country)
- There are also tunneling methods, which require acces to a server with a full ipv4. Some small VPS can be obtained, not powerfull enough for the servers themself, but only for forwarding. I think there are some for under 5€), the connection is then done via wireguard. but its a bit configuration heavy to setup) 

Or you connect your friends via VPN to your net and play via local lan then.
Many windowsgsm plugin creators recommend zerotier (should be a free VPN designated for gaming) , see chapter below (or tailscale, but no howto there)

## How can you play with your friends without port forwarding?
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
This project is licensed under the MIT License - see the <a href="https://github.com/raziel7893/WindowsGSM.BRINK/blob/main/LICENSE">LICENSE.md</a> file for details

### Thanks
Thanks to user GhettoScouser for providing the idea and the initial config
