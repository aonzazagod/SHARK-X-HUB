if game.PlaceId == 6461766546 then
    local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
    local Window = Library.CreateLib("SHARK X HUB l A Hero's Destiny", "DarkTheme")
	

    -- MAIN
    local Main = Window:NewTab("Autofarm")
    local MainSection = Main:NewSection("Autofarm l function")

	
    MainSection:NewButton("AUTO FARM AGILITY", "AUTO FARM AGILITY l Bypass with SHARK X", function()
        while wait(6) do
local A_1 = "Train"
local Event = game:GetService("ReplicatedStorage").RemoteEvent
Event:FireServer(A_1)
end
    end)
	
	 local autoSection = Main:NewSection("Autofarm l function")
	 
	 autoSection:NewButton("AUTO UpgradeHealth", "AUTO UpgradeHealth l Bypass with SHARK X", function()
        while wait(3) do
local A_1 = "UpgradeHealth"
local A_2 = 1
local Event = game:GetService("ReplicatedStorage").RemoteEvent
Event:FireServer(A_1, A_2)

end
    end)
	
	autoSection:NewButton("AUTO UpgradeStamina", "AUTO UpgradeStamina l Bypass with SHARK X", function()
        while wait(3) do
local A_1 = "UpgradeStamina"
local A_2 = 1
local Event = game:GetService("ReplicatedStorage").RemoteEvent
Event:FireServer(A_1, A_2)

end
    end)
	

	

    -- PLAYER
    local Player = Window:NewTab("Player")
    local PlayerSection = Player:NewSection("Player l funtion")

    PlayerSection:NewSlider("Walkspeed", "Changes WalkSpeed l Shark X Edit.", 250, 16, function(v)
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = v
    end)

    PlayerSection:NewSlider("Jumppower", "Changes JumpPower l Shark X Edit.", 250, 50, function(v)
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = v
    end)
	
	-- Credit
    local Player = Window:NewTab("Misc.")
    local PlayerSection = Player:NewSection("Discord : SHARKXEDIT.#3267")
	 local PlayerSection = Player:NewSection("YOUTUBE : SHARK X")
	
	
elseif game.PlaceId == 3956818381 then
    local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
    local Window = Library.CreateLib("SHARK X HUB l Ninja  Legends", "DarkTheme")

	-- MAIN
	local Mainxd = Window:NewTab("MAIN")
    local MainxdSection = Mainxd:NewSection("MAIN l FUNTION")
	
	MainxdSection:NewButton("INF Shurike", "INF Shurike l Bypass with SHARK X", function()
	while wait() do
        game.Players.LocalPlayer.shurikenAmmoCount.Value = "9999"
	game.Players.LocalPlayer.maxShurikenAmmo.Value = "9999"
	end
    end)
	
    -- AUTOFARM
    local Main = Window:NewTab("AUTOFARM")
    local MainSection = Main:NewSection("Auto farm l FUNTION")

    MainSection:NewToggle("Auto Swing", "Make your player autoswing l Bypass with SHARK X", function(v)
        getgenv().autoswing = v
        while true do
            if not getgenv().autoswing then return end
            for _,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do
                if v:FindFirstChild("ninjitsuGain") then
                    game.Players.LocalPlayer.Character.Humanoid:EquipTool(v)
                    break
                end
            end
            local A_1 = "swingKatana"
            local Event = game:GetService("Players").LocalPlayer.ninjaEvent
            Event:FireServer(A_1)
            wait(0.1)
        end
    end)

    MainSection:NewToggle("Auto Sell", "Makes your player autosell l Bypass with SHARK X", function(v)
        getgenv().autosell = v
        while true do
            if getgenv().autoswing == false then return end
            game:GetService("Workspace").sellAreaCircles["sellAreaCircle16"].circleInner.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
            wait(0.1)
            game:GetService("Workspace").sellAreaCircles["sellAreaCircle16"].circleInner.CFrame = CFrame.new(0,0,0)
            wait(0.1)
        end
    end)

    
    MainSection:NewToggle("Auto buy all swords", "Auto buys all swords l Bypass with SHARK X", function(v)
        getgenv().buyswords = v
        while true do
            if not getgenv().buyswords then return end
            local A_1 = "buyAllSwords"
            local A_2 = "Inner Peace Island"
            local Event = game:GetService("Players").LocalPlayer.ninjaEvent
            Event:FireServer(A_1, A_2)
            wait(0.5)
        end
    end)

    MainSection:NewToggle("Auto buy all belts", "Auto buys all belts", function(v)
        getgenv().buybelts = v
        while true do
            if not getgenv().buybelts then return end
            local A_1 = "buyAllBelts"
            local A_2 = "Inner Peace Island"
            local Event = game:GetService("Players").LocalPlayer.ninjaEvent
            Event:FireServer(A_1, A_2)
            wait(0.5)
        end
    end)
	
	-- Teleport
    local Teleport = Window:NewTab("Teleport")
    local TeleportSection = Teleport:NewSection("Teleport l FUNTION")
	TeleportSection:NewButton("Unlock all islands", "Unlocks all islands", function()
        local oldcframe = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
        for _,v in pairs(game:GetService("Workspace").islandUnlockParts:GetChildren()) do
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.CFrame
            wait(0.1)
        end
        wait(0.1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = oldcframe
    end)
	
	TeleportSection:NewButton("Teleport #1 Island", "Teleport #1 Island l Bypass with SHARK X", function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(10.3072119, 3.19799972, 30.0284615, 0.008823012, 6.67262299e-08, -0.999961078, 7.1362166e-08, 1, 6.7358485e-08, 0.999961078, -7.19536928e-08, 0.008823012)
    end)
	
	TeleportSection:NewButton("Teleport #2 Island", "Teleport #2 Island l Bypass with SHARK X", function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(219.300522, 2013.80908, 263.238495, -0.182153791, -8.21519066e-08, -0.983270049, 2.16322213e-08, 1, -8.75571189e-08, 0.983270049, -3.72191771e-08, -0.182153791)
    end)
	
	TeleportSection:NewButton("Teleport #3 Island", "Teleport #3 Island l Bypass with SHARK X", function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(144.503922, 4047.15601, 70.3039551, 0.477187604, 2.42895837e-08, -0.878801465, -5.37556346e-08, 1, -1.54976798e-09, 0.878801465, 4.7980059e-08, 0.477187604)
    end)
	
	TeleportSection:NewButton("Teleport #3 Island", "Teleport #3 Island l Bypass with SHARK X", function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(144.503922, 4047.15601, 70.3039551, 0.477187604, 2.42895837e-08, -0.878801465, -5.37556346e-08, 1, -1.54976798e-09, 0.878801465, 4.7980059e-08, 0.477187604)
    end)
	
	
	-- Credit
    local Player = Window:NewTab("Misc.")
    local PlayerSection = Player:NewSection("Discord : SHARKXEDIT.#3267")
	 local PlayerSection = Player:NewSection("YOUTUBE : SHARK X")
	
end
