> [!WARNING]
> You are most likely going to be banned since this is detected by Byfron. Use an alt account while running RezWare. Use the repository to understand what's happening and how it works.
> I am not liable for any bans


# RezWare
An executor made for the web version | RobloxPlayer of Roblox.

### Socials
https://discord.gg/rezware

## Features
- Fast execution
- Multi-instance compatibility
- Supports executing most scripts including Lua Armor scripts
- Uses extremely fast virtual filesystem that syncs to the external
- No in-game performance change & no high CPU usage
- Custom functions

## Custom Functions

```
# getfps()

-- For printing FPS once:
getfps(function(fps, isContinuous)
    print("FPS: " .. fps)
end, false)

-- For continuous FPS updates:
getfps(function(fps, isContinuous)
    print("FPS: " .. fps)  
end, true)

--------------/-\--------------

# getping()

-- For printing PING once:
getfps(function(ping, isContinuous)
    print("PING: " .. ping)
end, false)

-- For continuous FPS updates:
getfps(function(ping, isContinuous)
    print("PING: " .. ping)  
end, true)

--------------/utlls\--------------

# getPlayerInfo()

local player = game.Players.LocalPlayer -- Get the local player (you can change this to any player)

local playerInfo = getPlayerInfo(player)

if playerInfo then
    print("Player Name: " .. playerInfo.name)
    print("Player Health: " .. playerInfo.health)
else
    print("Player info could not be retrieved.")
end

# getGameInfo()

local gameInfo = getGameInfo()
print("Game Info:", gameInfo.name, "Place ID:", gameInfo.placeId, "Job ID:", gameInfo.jobId, "Players:", gameInfo.players)

# getRandomPlayer()

print("Random Player:", getRandomPlayer() and getRandomPlayer().Name) -- (DisplayName or Name)

# showNotify()

-- Shows simple roblox notify
showNotify("title", "message", duration)

```lua

### Preview

<p>This is the UI of the version v1.4.4:</p>
<img src="UI.png" alt="Preview" width="600" style="box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.5), -10px -10px 20px rgba(255, 255, 255, 0.3);" />
<p>The Current UNC is <span style="color: green;">~88%</span></p>
<img src="UNC.png" alt="Preview" width="600" style="box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.5), -10px -10px 20px rgba(255, 255, 255, 0.3);" />

## Credits: .Rizve, Glosary, danlacho

Based on Xeno Orginal Repo of Xeno https://github.com/Riz-ve/Xeno/

## Note
Big Thanks who helped me with RezWare Thanks .Rizve for injection system. Glosary helped make init!
