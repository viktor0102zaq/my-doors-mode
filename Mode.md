local Mode = loadstring(game:HttpGet("https://github.com/MuhXd/DoorSuff/blob/main/HardcoreTempate/TemplateCode.lua?raw=true"))()
-- Messages in a Table And Launches The Main Loader
Mode.StartCode({'Made by viktor0102zaq#3412',"Have fun! (you want)"})
Mode.StartCode{'also join to my dc server https://discord.com/channels/1079384215034019901/1079384215034019903'})
--[[
WaitTime Is How Long it Takes to Spawn
DisableSeek Makes it Not Appear In Seek and DisableFigure Does The same Thing Just for Figure
If the Room Is More then RoomMax Then it Won't Spawn but If the Room is Less Then RoomMin Then it Won't Spawn
--]]
loadstring(game:HttpGet("https://raw.githubusercontent.com/MuhXd/DoorSuff/main/OtherSuff/Sprint"))()


Mode.Loader({['WaitTime'] = 60,['DisableSeek'] = true,['DisableFigure'] = true,['RoomMax'] = 100,['RoomMin'] = 0},function()
    ---====== Define spawner ======---

local Spawner = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors/Entity%20Spawner/Source.lua"))()

---====== Create entity ======---

	local entity = Spawner.createEntity({
    CustomName = "Depth",
    Model = "(rbxassetid://11535848347",
    Speed = 161,
    MoveDelay = 9,
    HeightOffset = 1,
    CanKill = true,
    KillRange = 50,
    SpawnInFront = false,
    ShatterLights = true,
    FlickerLights = {
        Enabled = true,
        Duration = 2
    },
    Cycles = {
        Min = 2,
        Max = 2,
        Delay = 2
    },
    CamShake = {
        Enabled = true,
        Values = {2.5, 54, 0.1, 1},
        Range = 1231
    },
    ResistCrucifix = false,
    BreakCrucifix = true,
    IsCuriousLight = false
})



---====== Debug ======---

entity.Debug.OnEntitySpawned = function()
    print("Entity has spawned")
end

entity.Debug.OnEntityDespawned = function()
    print("Entity has despawned")
end

entity.Debug.OnEntityStartMoving = function()
    print("Entity started moving")
end

entity.Debug.OnEntityFinishedRebound = function()
    print("Entity finished rebound")
end

entity.Debug.OnEntityEnteredRoom = function(room)
    print("Entity entered room:", room)
end

entity.Debug.OnLookAtEntity = function()
    print("Player looking at entity")
end

entity.Debug.OnDeath = function()
    print("Player has died")
end

--[[
    NOTE: By overwriting 'OnUseCrucifix', the default crucifixion will be ignored and this function will be called instead
    entity.Debug.OnUseCrucifix = function()
        print("Custom crucifixion script here")
    end
]]--

---====== Run entity ======---

Spawner.runEntity(entity)
wait(13)

---====== Define spawner ======---

local Spawner = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors/Entity%20Spawner/Source.lua"))()

---====== Create entity ======---

	local entity = Spawner.createEntity({
    CustomName = "A-200",
    Model = "(rbxassetid://12304855811",
    Speed = 90,
    MoveDelay = 6,
    HeightOffset = 1,
    CanKill = true,
    KillRange = 50,
    SpawnInFront = true,
    ShatterLights = true,
    FlickerLights = {
        Enabled = true,
        Duration = 0.5
    },
    Cycles = {
        Min = 2,
        Max = 2,
        Delay = 2
    },
    CamShake = {
        Enabled = true,
        Values = {2.5, 54, 0.1, 1},
        Range = 1203999
    },
    ResistCrucifix = true,
    BreakCrucifix = true,
    IsCuriousLight = false
})
wait(10)


---====== Debug ======---

entity.Debug.OnEntitySpawned = function()
    print("Entity has spawned")
end

entity.Debug.OnEntityDespawned = function()
    print("Entity has despawned")
end

entity.Debug.OnEntityStartMoving = function()
    print("Entity started moving")
end

entity.Debug.OnEntityFinishedRebound = function()
    print("Entity finished rebound")
end

entity.Debug.OnEntityEnteredRoom = function(room)
    print("Entity entered room:", room)
end

entity.Debug.OnLookAtEntity = function()
    print("Player looking at entity")
end

entity.Debug.OnDeath = function()
    print("Player has died")
end

--[[
    NOTE: By overwriting 'OnUseCrucifix', the default crucifixion will be ignored and this function will be called instead
    entity.Debug.OnUseCrucifix = function()
        print("Custom crucifixion script here")
    end
]]--

---====== Run entity ======---

Spawner.runEntity(entity)
end)
