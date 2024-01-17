local Spawner = loadstring(game:HttpGet("https://raw.githubusercontent.com/RegularVynixu/Utilities/main/Doors%20Entity%20Spawner/Source.lua"))()
local entityTable = Spawner.createEntity({
    CustomName = "A-120", -- Custom name of your entity
    Model = "https://github.com/tonyBflako/vynixusdoors/blob/main/A120edit.rbxm?raw=true", -- Can be GitHub file or rbxassetid
    Speed = 75, -- Percentage, 100 = default Rush speed
    DelayTime = 2, -- Time before starting cycles (seconds)
    HeightOffset = 1.5,
    CanKill = false,
    KillRange = 10,
    BackwardsMovement = true,
    BreakLights = false,
    FlickerLights = {
        false
    },
    Cycles = {
        Min = 1,
        Max = math.random(1,2),
        WaitTime = 2.5,
    },
    CamShake = {
        true, -- Enabled
        {20, 15, 0.1, 1}, -- Shake values (don't change if you don't know)
        100, -- Shake start distance (from Entity to you)
    },
    Jumpscare = {
        false, -- Enabled/Disabled
    },
   CustomDialog = {" "},
})


Spawner.runEntity(entityTable)
