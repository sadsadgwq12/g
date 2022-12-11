-- imhappy's craftwars private gui
-- LIBRARY
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("imhappy#7541's private gui", "GrapeTheme")
-- promotion
local args = {
    [1] = "G ",
    [2] = "All"
}

game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))

-- PROPERTIES
local README = Window:NewTab("Read")
local READMESection = README:NewSection("Read")
local Tabs = Window:NewTab("Rates")
local TabsSection = Tabs:NewSection("Rates")
local Tabs2 = Window:NewTab("StarterPacks")
local Tabs2Section = Tabs2:NewSection("Put item in starterpack")
local Fun = Window:NewTab("Fun")
local FunSection = Fun:NewSection("Random stuff")
local Nopvp = Window:NewTab("Nopvp stuff")
local NopvpSection = Nopvp:NewSection("some nopvp stuff")
local Script = Window:NewTab("Scripts")
local ScriptSection = Script:NewSection("here scripts that i found")
local boss = Window:NewTab("Bosses")
local bossesection = boss:NewSection("duplicate a boss when they spawned")
local DataBase = Window:NewTab("Replicated")
local DataBaseSection = DataBase:NewSection("Spawns anything that stores in rep storage")
local MainData = Window:NewTab("Store Monster")
local DataSection = MainData:NewSection("Store monster in rep storage and then can be spawned in Replicated section")
-- Labels
READMESection:NewLabel("Being worked on ong")
READMESection:NewLabel("and don't skid bitch")
READMESection:NewLabel("made by imhappy#7541")
READMESection:NewLabel("Some scripts in this gui are skidded")
READMESection:NewLabel("Credits to scripts that i used in this gui")
READMESection:NewLabel("If you get this gui from me DO NOT give it to somebody else")
READMESection:NewLabel("admin commands are being maked (just mabye lol)")
--rates
DataSection:NewButton("nacker save", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.nacker,
        [2] = game.ReplicatedStorage
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
print("saved nacker")
end)

DataSection:NewButton("zeus save", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Zeus,
        [2] = game.ReplicatedStorage
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
print("saved zeus")
end)

DataSection:NewButton("Medusa save", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Medusa,
        [2] = game.ReplicatedStorage
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
print("saved Medusa")
end)

DataSection:NewButton("cronus save", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Cronus,
        [2] = game.ReplicatedStorage
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
print("saved Cronus")
end)
DataSection:NewButton("zombie boss save", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace:FindFirstChild("Zombie Boss"),
        [2] = game.ReplicatedStorage
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
print("saved Cronus")
end)
DataBaseSection:NewButton("nacker", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game.ReplicatedStorage.nacker,
        [2] = workspace
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
print("spawned nacker")
end)
DataBaseSection:NewButton("zeus", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game.ReplicatedStorage.Zeus,
        [2] = workspace
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
print("spawned zeus")
end)
DataBaseSection:NewButton("Medusa", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game.ReplicatedStorage.Medusa,
        [2] = workspace
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
print("spawned medusa")
end)
DataBaseSection:NewButton("zombie boss", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game.ReplicatedStorage:FindFirstChild("Zombie Boss"),
        [2] = workspace
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
print("spawned zombieboss")
end)
bossesection:NewButton("Medusa Dupe", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Medusa,
        [2] = workspace
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)

bossesection:NewButton("Zeus Dupe", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Zeus,
        [2] = workspace
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
TabsSection:NewButton("Mobrate (1+)", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
bossesection:NewButton("Zombie Boss", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace:FindFirstChild("Zombie Boss"),
        [2] = workspace
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
bossesection:NewButton("cronus dupe", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Cronus,
        [2] = workspace
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
bossesection:NewButton("nacker dupe", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.nacker,
        [2] = workspace
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
TabsSection:NewButton("Mobrate (5+)", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))

end)
TabsSection:NewButton("Mobrate (10+)", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.enemySpawn,
        [2] = workspace.Landscape
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
TabsSection:NewButton("Orerate (10+)", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine.oreSpawn,
        [2] = workspace.Mine
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)

TabsSection:NewButton("Orerate adv mine (10+)", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Mine2.oreSpawn,
        [2] = workspace.Mine2
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
-- Starterpacks
Tabs2Section:NewButton("Scythe StarterPack Everyone", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.OmegaDeathScythe.Tool,
        [2] = game:GetService("StarterPack")
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
Tabs2Section:NewButton("Armour StarterPack Everyone", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.OmegaDeathArmour.Tool,
        [2] = game:GetService("StarterPack")
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)


Tabs2Section:NewButton("Pistol Starterpack everyone", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.OmegaDeathPistol.Tool,
        [2] = game:GetService("StarterPack")
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)

Tabs2Section:NewButton("Royale pickaxe starter pack everyone", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.RoyalPickaxe.Tool,
        [2] = game:GetService("StarterPack")
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)

Tabs2Section:NewButton("minigun starterpack everyone", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.DeathsMinigun.Tool,
        [2] = game:GetService("StarterPack")
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)

Tabs2Section:NewButton("BlackHole StarterPack everyone", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.BlackholeStaff.Tool,
        [2] = game:GetService("StarterPack")
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
--NoPvPs leaderboard
NopvpSection:NewButton("NoPvP Roast", "yes", function()
	local args = {
    [1] = {
        ["value"] = "go",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
-- 1

local args = {
    [1] = {
        ["value"] = "fuck",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
--2

local args = {
    [1] = {
        ["value"] = "yourself",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
--funs
FunSection:NewButton("No COoldown", "yes", function()
		local Cooldown; Cooldown = hookfunction(wait, function(v)
		v = 0;
		return Cooldown(v);
		end)
	end)

FunSection:NewButton("Aura", "yes", function()
	local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.OmegaDeathScythe.Tool.Handle.ParticleEmitter,
        [2] = game:GetService("Players").LocalPlayer.Character.Torso
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.OmegaDeathScythe.Tool.Handle.ParticleEmitter,
        [2] = game:GetService("Players").LocalPlayer.Character:FindFirstChild("Right Arm")
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.OmegaDeathScythe.Tool.Handle.ParticleEmitter,
        [2] = game:GetService("Players").LocalPlayer.Character.Head
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.OmegaDeathScythe.Tool.Handle.ParticleEmitter,
        [2] = game:GetService("Players").LocalPlayer.Character:FindFirstChild("Left Arm")
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.OmegaDeathScythe.Tool.Handle.ParticleEmitter,
        [2] = game:GetService("Players").LocalPlayer.Character:FindFirstChild("Right Leg")
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("ReplicatedStorage").Items.OmegaDeathScythe.Tool.Handle.ParticleEmitter,
        [2] = game:GetService("Players").LocalPlayer.Character:FindFirstChild("Left Leg")
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)

FunSection:NewButton("God mode (nacker armour required..)", "yes", function()
	local args = {
    [1] = "protect",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.Character,
        [2] = game:GetService("Players").LocalPlayer.Character.Humanoid,
        [3] = math.huge
    }
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Nacker's Armour").RemoteFunction:InvokeServer(unpack(args))
end)


NopvpSection:NewButton("Nopvp discord promotion", "yes", function()
local args = {
    [1] = {
        ["value"] = "ADD",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}


game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}
game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
-- 1
wait(2)
local args = {
    [1] = {
        ["value"] = "imhappy",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
--2
wait(2)
local args = {
    [1] = {
        ["value"] = "#7541",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)

FunSection:NewButton("Spam Bubble sea revenge required", "yes", function()
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
	local args = {
    [1] = "shield",
    [2] = game:GetService("Players").LocalPlayer.Character
}
game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
end)
FunSection:NewButton("Spam effects sea revenge required", "yes", function()
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "inserteffect",
    [2] = game:GetService("Players").LocalPlayer.Character
}

game:GetService("Players").LocalPlayer.Character:FindFirstChild("Sea's Revenge").RemoteFunction:InvokeServer(unpack(args))
end)
FunSection:NewButton("crash server lol", "yes", function()
__Player__ = game:GetService("Players").LocalPlayer
__Character__ = __Player__.Character
function __Place__(arg1, arg2)
    __Player__.Backpack.BuildTool.RemoteFunction:InvokeServer("placeobject", { arg1, arg2 })
end
game.RunService.Stepped:Connect(function()
    __Place__(workspace.Mine2.oreSpawn, workspace.Mine2.oreSpawn)
    end)
end)
FunSection:NewButton("nuke server with alot of mesh", "yes", function()
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Water.Mesh,
        [2] = game:GetService("Players").LocalPlayer.Character.Torso
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))

local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Water.Mesh,
        [2] = game:GetService("Players").LocalPlayer.Character.Head
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Water.Mesh,
        [2] = game:GetService("Players").LocalPlayer.Character
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Water.Mesh,
        [2] = workspace.Landscape.tree.Leaves
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Wall.Mesh,
        [2] = workspace.Landscape.Grass
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.tree.Leaves,
        [2] = workspace.Landscape.tree.Log
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Wall.Mesh,
        [2] = workspace.Bases.Base4.objects.center
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.tree.Log,
        [2] = workspace.Bases.Base3.objects.center
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Grass,
        [2] = workspace.Bases.Base2.objects.center
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Water.Mesh,
        [2] = workspace.Bases.Base2.objects.center
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Sand,
        [2] = game:GetService("Players").LocalPlayer.Character.Torso
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Water.Mesh,
        [2] = workspace.Bases.Base4.house.Part
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Grass,
        [2] = workspace.Bases.Base3.house.Part
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Water.Mesh,
        [2] = workspace.Bases.Base2.house.Part
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = workspace.Landscape.Water.Mesh,
        [2] = workspace.Bases.Base1.house.Part
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
NopvpSection:NewButton("nazis flag nopvp", "yes", function()
local args = {
    [1] = {
        ["value"] = "卐",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
NopvpSection:NewButton("uni soviet flag nopvp", "yes", function()
local args = {
    [1] = {
        ["value"] = "☭",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)

NopvpSection:NewButton("sets nopvp to normal", "yes", function()

local args = {
    [1] = {
        ["value"] = "-",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
end)
-- scripts section
ScriptSection:NewButton("Craftwars Fucker", "yes", function()
end)

ScriptSection:NewButton("Grass gui (1)", "yes", function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/sadsadgwq12/g/main/d"))()
end)
ScriptSection:NewButton("inf yield", "yes", function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)
NopvpSection:NewButton("cash, rank, nopvp hack", "yes", function()
local args = {
    [1] = {
        ["value"] = "69000000",
        ["instance"] = game:GetService("Players").LocalPlayer.realstats.Cash,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.realstats.Cash,
        [2] = game:GetService("Players").LocalPlayer.realstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = {
        ["value"] = "69000000000",
        ["instance"] = game:GetService("Players").LocalPlayer.leaderstats.Rank,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.leaderstats.Rank,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = {
        ["value"] = "nigga",
        ["instance"] = game:GetService("Players").LocalPlayer.nopvp,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))

local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.nopvp,
        [2] = game:GetService("Players").LocalPlayer.leaderstats
    }
}

game:GetService("Players").LocalPlayer.Backpack.BuildTool.RemoteFunction:InvokeServer(unpack(args))
local args = {
    [1] = {
        ["value"] = "69000000",
        ["instance"] = game:GetService("Players").LocalPlayer.realstats.Cash,
        ["command"] = "setvalue"
    }
}

game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
local args = {
    [1] = "placeobject",
    [2] = {
        [1] = game:GetService("Players").LocalPlayer.realstats.Cash,
        [2] = game:GetService("Players").LocalPlayer.realstats
    }
}
game:GetService("ReplicatedStorage").MainControl:InvokeServer(unpack(args))
end)
