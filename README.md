# TeleportService_But_Easier_Docs

```
Module.IsServerPrivate()  
    - arguments required:  
        - none  
    - optional arguments:  
        - none  
    - returns:  
        - table(dictionary):  
            {  
                customPrivate : bool,  
                ownedPrivate : bool,   
                public : bool   
            } (one of the bools is true, two are false, customPrivate servers are servers made in script, ownedPrivate are ones that are afforded on the roblox website)  





Module.SingleTeleport()  
    - arguments required:  
        - placeid : int (place id of the place to teleport to)  
        - player : player instance (player to be teleported)  
    - optional arguments:  
        - teleportData : teleportData (data you can retrieve at the location of teleportation)  
        - loadingScreen : GuiInstance (gui that the player can see while being teleported)  
        - instanceid : int (if this is provided, the player will be teleported to the server the id belongs to, if not, the player will get teleported to a random server)  
        - spawnName : string (name of the spawn the player will spawn at in the place they teleported to; only works if instanceid is provided)  
    returns:  
        - none  





Module.GroupTeleport()  
    - arguments required:  
        - placeid : int (place id of the place to teleport to)  
        - players : table(array) of player instances (players to be teleported)  
    - optional arguments:  
        - teleportData : teleportData (data you can retrieve at the location of teleportation)  
        - loadingScreen : GuiInstance (gui that the player can see while being teleported)  
        - instanceid : int (if this is provided, the player will be teleported to the server the id belongs to, if not, the player will get teleported to a random server)  
        - spawnName : string (name of the spawn the player will spawn at in the place they teleported to; only works if instanceid is provided)  
    returns:  
        - none  





Module.MakePrivate()  
    - arguments required:  
        - placeid : int (place id of the place to make a private server at)  
    - optional arguments:  
        - none  
    - returns:  
        - table(dictionary):  
            {  
                code : string (access code which is needed to teleport players to the private server),  
                serverid : string (server id of the private server)  
            }  





Module.TeleportToPrivate()  
    - arguments required:  
        - placeid : int (place id of the place to teleport to)  
        - accessCode : string (access code to teleport user to private server (you can get this code from Module.MakePrivate()))  
        - players : table(array) (table of players that should get teleported)  
    - optional arguments:  
        - spawnName : string (name of the spawn the player will spawn at in the place they teleported to; only works if instanceid is provided)  
        - teleportData : teleportData (data you can retrieve at the location of teleportation)  
        - loadingScreen : GuiInstance (gui that the player can see while being teleported)  
    - returns:  
        - none  





Module.MakeAndTeleportToPrivate()  
    - arguments required:  
        - placeid : int (place id of the place to teleport to)  
        - players : table(array) (table of players that should get teleported)  
    - optional arguments:  
        - spawnName : string (name of the spawn the player will spawn at in the place they teleported to; only works if instanceid is provided)  
        - teleportData : teleportData (data you can retrieve at the location of teleportation)  
        - loadingScreen : GuiInstance (gui that the player can see while being teleported)  
    - returns:  
        - none  





Module.TeleportPartyAndGetServerId()  
    - arguments required:  
        - placeid : int (place id of the place to teleport to)  
        - players : table(array) (table of players that should get teleported)  
    - optional arguments:  
        - teleportData : teleportData (data you can retrieve at the location of teleportation)  
        - loadingScreen : GuiInstance (gui that the player can see while being teleported)  
    - returns:  
        - table:  
            {  
                serverid : string (the id of the server to which the players got teleported)  
            }  
  
```
