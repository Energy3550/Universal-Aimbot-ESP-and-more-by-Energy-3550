local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Ui = Library.CreateLib("Fluid Energy's Hacking Ui", "Sentinel")

--Main
local Main = Ui:NewTab("Main")
local MainSection = Main:NewSection("Bad Buisness")

--Main Buttons
MainSection:NewSlider("Walk Speed", "Changes your walk/run speed", 500, 0, function(s) 
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

MainSection:NewKeybind("Ui Toggle", "Toggle Ui Visibility", Enum.KeyCode.F, function()
	Library:ToggleUI()
end)


MainSection:NewButton("BBUI", "Open Bad Buisness Ui", function()
    loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Loader.lua"))()
end)

MainSection:NewButton("BHRM5", "Open Black Hawk Rescue Mission 5 Ui", function()
    loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Loader.lua"))()
end)

MainSection:NewButton("Fly", "Enables Simple Fly Ui", function()
    loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\40\39\104\116\116\112\115\58\47\47\103\105\115\116\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\109\101\111\122\111\110\101\89\84\47\98\102\48\51\55\100\102\102\57\102\48\97\55\48\48\49\55\51\48\52\100\100\100\54\55\102\100\99\100\51\55\48\47\114\97\119\47\101\49\52\101\55\52\102\52\50\53\98\48\54\48\100\102\53\50\51\51\52\51\99\102\51\48\98\55\56\55\48\55\52\101\98\51\99\53\100\50\47\97\114\99\101\117\115\37\50\53\50\48\120\37\50\53\50\48\102\108\121\37\50\53\50\48\50\37\50\53\50\48\111\98\102\108\117\99\97\116\111\114\39\41\44\116\114\117\101\41\41\40\41\10\10")()
end)
