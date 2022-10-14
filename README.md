local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Southwest Florida gui", "Sentinel")
--Player
local Player = Window:NewTab("Player")
local PlayerSection = Player:NewSection("Player")

PlayerSection:NewSlider("Walk speed", "makes u walk more fast", 500, 16, function(s) -- 500 (MaxValue) | 16 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

PlayerSection:NewSlider("Jumppower", "makes u jump more high", 350, 50, function(s) -- 350 (MaxValue) | 50 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)

PlayerSection:NewButton("God Mode", "God Mode", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/trem2goated/god-mode-/main/README.md'))()
end)

--TP
local Tp = Window:NewTab("Tp")
local TpSection = Tp:NewSection("Tp")

TpSection:NewButton("Tp to spawn", "Tp to spawn", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2433.873, 24, -265.673)
end)

TpSection:NewButton("Tp to police station", "Tp to police station", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(5918.935, 21.5, 728.596)
end)

TpSection:NewButton("Tp to dealership", "Tp to dealership", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(8936.538, 24.689, 3091.896)
end)

TpSection:NewButton("Tp to Mcbloxxer's", "Tp to Mcbloxxer's", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(9614.148, 22.65, 1263.306)
end)
