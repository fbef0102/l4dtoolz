# L4DToolz

https://forums.alliedmods.net/showthread.php?t=93600

Metamod plugin to unlock the max player limit on L4D and L4D2.

# How
* Download package from [Release page](https://github.com/fbef0102/l4dtoolz/releases)
* Unzip all files to your server same folder, press yes if ask override. You will have ```l4dtoolz``` folder in addons folder
  <br/>![image](https://github.com/fbef0102/l4dtoolz/assets/12229810/3c98c6e3-8909-42c8-b6ba-a18083f3bb2b)
* Write down cfg/server.cfg (Create it if file does not exist)
  ```
  // Max Human Players, free to modify value (1~31)
  // How many human players can joins server
  sv_maxplayers 18

  // Overrides the max players reported to prospective clients
  sv_visiblemaxplayers 18

  // If 1, Players may only join this server from matchmaking lobby, may not connect directly.
  sv_allow_lobby_connect_only 0
  
  // If 1, Disallow lobby reservation cookie
  sv_force_unreserved 1
  ```

* By default, the game engine only allow 18 max players. To change max players, please input ```-maxplayers 32```in server launch paramater 
  * Max. players = Human player + AI Survivor Bot + AI Infected Bot + Spectators
  <br/>![image](https://github.com/fbef0102/l4dtoolz/assets/12229810/5357e7f0-485b-4217-99d5-839ef50c5291)

