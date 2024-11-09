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

```lua
-------------------------------------------------------
--                FPS and PING Functions              --
-------------------------------------------------------

-- getfps()

-- Print FPS once:
getfps(function(fps, isContinuous)
    print(string.format("FPS: %d", fps))
end, false)

-- Continuous FPS updates:
getfps(function(fps, isContinuous)
    print(string.format("FPS: %d", fps))  
end, true)

-------------------------------------------------------
--                PING Functions                     --
-------------------------------------------------------

-- getping()

-- Print PING once:
getping(function(ping, isContinuous)
    print(string.format("PING: %d ms", ping))
end, false)

-- Continuous PING updates:
getping(function(ping, isContinuous)
    print(string.format("PING: %d ms", ping))  
end, true)

-------------------------------------------------------
--                Utility Functions                 --
-------------------------------------------------------

-- getPlayerInfo()

local player = game.Players.LocalPlayer -- Local player (or change this to any other player)

local playerInfo = getPlayerInfo(player)

if playerInfo then
    print("Player Name: " .. playerInfo.name)
    print("Player Health: " .. playerInfo.health)
else
    print("Error: Player info could not be retrieved.")
end

-------------------------------------------------------
--                Game Info Function                --
-------------------------------------------------------

-- getGameInfo()

local gameInfo = getGameInfo()
print(string.format("Game Info:\nName: %s\nPlace ID: %d\nJob ID: %d\nPlayers: %d",
    gameInfo.name, gameInfo.placeId, gameInfo.jobId, gameInfo.players))

-------------------------------------------------------
--                Random Player Function            --
-------------------------------------------------------

-- getRandomPlayer()

local randomPlayer = getRandomPlayer()
if randomPlayer then
    print(string.format("Random Player: %s", randomPlayer.Name))  -- DisplayName or Name
else
    print("No random player found.")
end

-------------------------------------------------------
--                Notification Function             --
-------------------------------------------------------

-- showNotify()

-- Show simple Roblox notification:
showNotify("Sample Title", "This is a sample message.", 5) -- duration in seconds

-------------------------------------------------------
--                     Actors                        --
-------------------------------------------------------

-- Creates actor
create_actor("ActorName") -- if not enter name ("NewActor_" .. math.random(1, 1000))

-- Save Actor
save_actor(actor)

- Get running actors
get_running_actors() or get_running_actors(actorName)

-- Run on actor
run_on_actor(actor, callback)

-------------------------------------------------------
--                     Print Info                    --
-------------------------------------------------------

-- Does the same as printing, but instead it looks like that C information print.
rez.print("hi")

-- Does the same as Warning, but instead it looks like that C information warn.
rez.warn("hi")

-- Does the same as assert, but instead it looks like that C information assert.

rez.assert(false, "hi") or rez.assert(true, "hi")

-------------------------------------------------------
--                    Other                          --
-------------------------------------------------------

-- Gets addres of func
rez.get_address(func)

-- Kicks localplayer
rez.kickme(reason)

-- Teleports to player
teleportTo("Name or displayName") if name big teleportTo("doc") \ doctor2044

-- Prints actual RezWare version
print("rez.rezversion()")

```

### Preview

<p>This is the UI of the version v1.4.4:</p>
<img src="UI.png" alt="Preview" width="600" style="box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.5), -10px -10px 20px rgba(255, 255, 255, 0.3);" />
<p>The Current UNC is <span style="color: green;">~88%</span></p>
<img src="UNC.png" alt="Preview" width="600" style="box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.5), -10px -10px 20px rgba(255, 255, 255, 0.3);" />

## Credits: .Rizve, Glosary, danlacho

Based on Xeno Orginal Repo of Xeno https://github.com/Riz-ve/Xeno/

## Note
Big Thanks who helped me with RezWare Thanks .Rizve for injection system. Glosary helped make init!
