
local ScreenGui = Instance.new("ScreenGui")
local main = Instance.new("Frame")
local quest = Instance.new("Frame")
local TeleportMenu = Instance.new("Frame")
local charqol = Instance.new("Frame")
local tools = Instance.new("Frame")
local TeleMn = Instance.new("Frame")
local SpeedConfig = Instance.new("Frame")
local title = Instance.new("TextLabel")
local TIDTLE = Instance.new("TextLabel")
local QuestTitle = Instance.new("TextLabel")
local TeleportTitle = Instance.new("TextLabel")
local CharTitle = Instance.new("TextLabel")
local toolsTitle = Instance.new("TextLabel")
local SCTitle = Instance.new("TextLabel")
local Text = Instance.new("TextButton")
local healthx = Instance.new("TextButton")
local jumpx = Instance.new("TextButton")
local speedx = Instance.new("TextButton")
local ChatBypasser = Instance.new("TextButton")
local adminC = Instance.new("TextButton")
local ShiftlockS = Instance.new("TextButton")
local PengChar = Instance.new("TextButton")
local FoxChar = Instance.new("TextButton")
local ChickChar = Instance.new("TextButton")
local CharClose = Instance.new("TextButton")
local ccharacter = Instance.new("TextButton")
local discord = Instance.new("TextButton")
local winter = Instance.new("TextButton")
local spider = Instance.new("TextButton")
local infox = Instance.new("TextButton")
local chqst = Instance.new("TextButton")
local fabbi = Instance.new("TextButton")
local pqst = Instance.new("TextButton")
local Te = Instance.new("TextButton")
local SCBtn = Instance.new("TextButton")
local SpeedConf = Instance.new("TextButton")
local farmgold = Instance.new("TextButton")
local farmgoldv2 = Instance.new("TextButton")
local iloader = Instance.new("TextButton")
local TPID = Instance.new("TextButton")
local BeAdmin = Instance.new("TextButton")
local TeleBtn = Instance.new("TextButton")
local close = Instance.new("TextButton")
local QuestClose = Instance.new("TextButton")
local TeleportClose = Instance.new("TextButton")
local toolsClose = Instance.new("TextButton")
local InnerCloud = Instance.new("TextButton")
local openmain = Instance.new("Frame")
local open = Instance.new("TextButton")
local TeleClose = Instance.new("TextButton")
local SCClose = Instance.new("TextButton")
local TeleID = Instance.new("TextBox")
local SpeedC = Instance.new("TextBox")
local JumpConfig = Instance.new("Frame")
local JCTitle = Instance.new("TextLabel")
local JumpConf = Instance.new("TextButton")
local JCClose = Instance.new("TextButton")
local JCBtn = Instance.new("TextButton")
local JumpC = Instance.new("TextBox")
--Properties:
ScreenGui.Parent = game.CoreGui

JumpC.Name = "JumpC"
JumpC.Parent = JumpConfig
JumpC.BackgroundColor3 = Color3.fromRGB(76, 76, 76)
JumpC.BorderSizePixel = 0
JumpC.Position = UDim2.new(0.035518092, 0, 0.30, 0)
JumpC.Size = UDim2.new(0.778996766, 0, 0.26676026, 0)
JumpC.Font = Enum.Font.GothamSemibold
JumpC.PlaceholderText = "Insert Number"
JumpC.Text = ""
JumpC.TextColor3 = Color3.fromRGB(255, 255, 255)
JumpC.TextSize = 14.000

JumpConfig.Name = "JumpConfig"
JumpConfig.Parent = ScreenGui
JumpConfig.BackgroundColor3 = Color3.new(0, 0, 0)
JumpConfig.Position = UDim2.new(0.0203577988, 0, 0.641277611, 0)
JumpConfig.Size = UDim2.new(0, 432, 0, 291)
JumpConfig.Visible = false
JumpConfig.Active = true
JumpConfig.Draggable = true

JCTitle.Name = "JCTitle"
JCTitle.Parent = JumpConfig
JCTitle.BackgroundColor3 = Color3.new(1, 0, 1)
JCTitle.Size = UDim2.new(0, 332, 0, 31)
JCTitle.Font = Enum.Font.GothamBold
JCTitle.Text = "Jump Power Changer"
JCTitle.TextColor3 = Color3.new(0, 0, 0)
JCTitle.TextSize = 14

JumpConf.Name = "JumpConf"
JumpConf.Parent = JumpConfig
JumpConf.BackgroundColor3 = Color3.new(0.333333, 1, 0)
JumpConf.Position = UDim2.new(0.35518092, 0, 0.63, 0)
JumpConf.Size = UDim2.new(0, 110, 0, 50)
JumpConf.Font = Enum.Font.GothamBold
JumpConf.Text = "Change"
JumpConf.TextColor3 = Color3.new(0, 0, 0)
JumpConf.TextScaled = true
JumpConf.TextSize = 14
JumpConf.TextWrapped = true
JumpConf.MouseButton1Down:connect(function()
game.Players.LocalPlayer.Character.Humanoid.JumpPower = JumpC.Text
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Jump Power Changed To";
        Text = JumpC.Text;
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

JCBtn.Name = "JCBtn"
JCBtn.Parent = main
JCBtn.BackgroundColor3 = Color3.new(0.036144577, 1, 0)
JCBtn.Position = UDim2.new(0.679518092, 0, 0.84, 0)
JCBtn.Size = UDim2.new(0, 110, 0, 50)
JCBtn.Font = Enum.Font.GothamBold
JCBtn.Text = "Jump Power Changer"
JCBtn.TextColor3 = Color3.new(0, 0, 0)
JCBtn.TextScaled = true
JCBtn.TextSize = 14
JCBtn.TextWrapped = true
JCBtn.MouseButton1Down:connect(function()
main.Visible = false
JumpConfig.Visible = true
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Info";
        Text = "Insert Number";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

JCClose.Name = "JCClose"
JCClose.Parent = JumpConfig
JCClose.BackgroundColor3 = Color3.new(1, 0, 0)
JCClose.Position = UDim2.new(0.879518092, 0, 0, 0)
JCClose.Size = UDim2.new(0, 40, 0, 31)
JCClose.Font = Enum.Font.GothamBlack
JCClose.Text = "X"
JCClose.TextColor3 = Color3.new(0, 0, 0)
JCClose.TextScaled = true
JCClose.TextSize = 14
JCClose.TextWrapped = true
JCClose.MouseButton1Down:connect(function()
main.Visible = true
JumpConfig.Visible = false
end)

SpeedC.Name = "SpeedC"
SpeedC.Parent = SpeedConfig
SpeedC.BackgroundColor3 = Color3.fromRGB(76, 76, 76)
SpeedC.BorderSizePixel = 0
SpeedC.Position = UDim2.new(0.035518092, 0, 0.30, 0)
SpeedC.Size = UDim2.new(0.78996766, 0, 0.26676026, 0)
SpeedC.Font = Enum.Font.GothamSemibold
SpeedC.PlaceholderText = "Insert Number"
SpeedC.Text = ""
SpeedC.TextColor3 = Color3.fromRGB(255, 255, 255)
SpeedC.TextSize = 14.000

SpeedConfig.Name = "SpeedConfig"
SpeedConfig.Parent = ScreenGui
SpeedConfig.BackgroundColor3 = Color3.new(0, 0, 0)
SpeedConfig.Position = UDim2.new(0.0203577988, 0, 0.641277611, 0)
SpeedConfig.Size = UDim2.new(0, 432, 0, 291)
SpeedConfig.Visible = false
SpeedConfig.Active = true
SpeedConfig.Draggable = true

SCTitle.Name = "SCTitle"
SCTitle.Parent = SpeedConfig
SCTitle.BackgroundColor3 = Color3.new(1, 0, 1)
SCTitle.Size = UDim2.new(0, 332, 0, 31)
SCTitle.Font = Enum.Font.GothamBold
SCTitle.Text = "Speed Changer"
SCTitle.TextColor3 = Color3.new(0, 0, 0)
SCTitle.TextSize = 14

SpeedConf.Name = "SpeedConf"
SpeedConf.Parent = SpeedConfig
SpeedConf.BackgroundColor3 = Color3.new(0.333333, 1, 0)
SpeedConf.Position = UDim2.new(0.35518092, 0, 0.63, 0)
SpeedConf.Size = UDim2.new(0, 110, 0, 50)
SpeedConf.Font = Enum.Font.GothamBold
SpeedConf.Text = "Change"
SpeedConf.TextColor3 = Color3.new(0, 0, 0)
SpeedConf.TextScaled = true
SpeedConf.TextSize = 14
SpeedConf.TextWrapped = true
SpeedConf.MouseButton1Down:connect(function()
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = SpeedC.Text
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "info";
        Text = "Speed Changed to: " .. SpeedC.Text;
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

SCBtn.Name = "SCBtn"
SCBtn.Parent = main
SCBtn.BackgroundColor3 = Color3.new(0.036144577, 1, 0)
SCBtn.Position = UDim2.new(0.036518092, 0, 0.84, 0)
SCBtn.Size = UDim2.new(0, 110, 0, 50)
SCBtn.Font = Enum.Font.GothamBold
SCBtn.Text = "Speed Changer"
SCBtn.TextColor3 = Color3.new(0, 0, 0)
SCBtn.TextScaled = true
SCBtn.TextSize = 14
SCBtn.TextWrapped = true
SCBtn.MouseButton1Down:connect(function()
main.Visible = false
SpeedConfig.Visible = true
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Info";
        Text = "Insert Number";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

SCClose.Name = "SCClose"
SCClose.Parent = SpeedConfig
SCClose.BackgroundColor3 = Color3.new(1, 0, 0)
SCClose.Position = UDim2.new(0.879518092, 0, 0, 0)
SCClose.Size = UDim2.new(0, 40, 0, 31)
SCClose.Font = Enum.Font.GothamBlack
SCClose.Text = "X"
SCClose.TextColor3 = Color3.new(0, 0, 0)
SCClose.TextScaled = true
SCClose.TextSize = 14
SCClose.TextWrapped = true
SCClose.MouseButton1Down:connect(function()
main.Visible = true
SpeedConfig.Visible = false
end)

TeleID.Name = "TeleID"
TeleID.Parent = TeleMn
TeleID.BackgroundColor3 = Color3.fromRGB(76, 76, 76)
TeleID.BorderSizePixel = 0
TeleID.Position = UDim2.new(0.036144577, 0, 0.30, 0)
TeleID.Size = UDim2.new(0.778996766, 0, 0.26676026, 0)
TeleID.Font = Enum.Font.GothamSemibold
TeleID.PlaceholderText = "PlaceID"
TeleID.Text = ""
TeleID.TextColor3 = Color3.fromRGB(255, 255, 255)
TeleID.TextSize = 14.000

TeleMn.Name = "TeleMn"
TeleMn.Parent = ScreenGui
TeleMn.BackgroundColor3 = Color3.new(0, 0, 0)
TeleMn.Position = UDim2.new(0.0203577988, 0, 0.641277611, 0)
TeleMn.Size = UDim2.new(0, 432, 0, 291)
TeleMn.Visible = false
TeleMn.Active = true
TeleMn.Draggable = true

TIDTLE.Name = "TIDTLE"
TIDTLE.Parent = TeleMn
TIDTLE.BackgroundColor3 = Color3.new(1, 0, 1)
TIDTLE.Size = UDim2.new(0, 332, 0, 31)
TIDTLE.Font = Enum.Font.GothamBold
TIDTLE.Text = "Teleport To PlaceID"
TIDTLE.TextColor3 = Color3.new(0, 0, 0)
TIDTLE.TextSize = 14

TPID.Name = "TPID"
TPID.Parent = TeleMn
TPID.BackgroundColor3 = Color3.new(0.333333, 1, 0)
TPID.Position = UDim2.new(0.35518092, 0, 0.63, 0)
TPID.Size = UDim2.new(0, 110, 0, 50)
TPID.Font = Enum.Font.GothamBold
TPID.Text = "Teleport"
TPID.TextColor3 = Color3.new(0, 0, 0)
TPID.TextScaled = true
TPID.TextSize = 14
TPID.TextWrapped = true
TPID.MouseButton1Down:connect(function()
game:GetService("TeleportService"):Teleport(TeleID.Text, LocalPlayer)
end)

TeleBtn.Name = "TeleBtn"
TeleBtn.Parent = main
TeleBtn.BackgroundColor3 = Color3.new(0.333333, 1, 0)
TeleBtn.Position = UDim2.new(0.35518092, 0, 0.84, 0)
TeleBtn.Size = UDim2.new(0, 110, 0, 50)
TeleBtn.Font = Enum.Font.GothamBold
TeleBtn.Text = "Teleport To PlaceID"
TeleBtn.TextColor3 = Color3.new(0, 0, 0)
TeleBtn.TextScaled = true
TeleBtn.TextSize = 14
TeleBtn.TextWrapped = true
TeleBtn.MouseButton1Down:connect(function()
main.Visible = false
TeleMn.Visible = true
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Info";
        Text = "Insert PlaceID";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

TeleClose.Name = "TeleClose"
TeleClose.Parent = TeleMn
TeleClose.BackgroundColor3 = Color3.new(1, 0, 0)
TeleClose.Position = UDim2.new(0.879518092, 0, 0, 0)
TeleClose.Size = UDim2.new(0, 40, 0, 31)
TeleClose.Font = Enum.Font.GothamBlack
TeleClose.Text = "X"
TeleClose.TextColor3 = Color3.new(0, 0, 0)
TeleClose.TextScaled = true
TeleClose.TextSize = 14
TeleClose.TextWrapped = true
TeleClose.MouseButton1Down:connect(function()
main.Visible = true
TeleMn.Visible = false
end)

game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Welcome";
        Text = "Script Loaded :D";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;

main.Name = "main"
main.Parent = ScreenGui
main.BackgroundColor3 = Color3.new(0, 0, 0)
main.Position = UDim2.new(0.0203577988, 0, 0.641277611, 0)
main.Size = UDim2.new(0, 435, 0, 336)
main.Visible = false
main.Active = true
main.Draggable = true

tools.Name = "tools"
tools.Parent = ScreenGui
tools.BackgroundColor3 = Color3.new(0, 0, 0)
tools.Position = UDim2.new(0.0203577988, 0, 0.641277611, 0)
tools.Size = UDim2.new(0, 435, 0, 336)
tools.Visible = false
tools.Active = true
tools.Draggable = true

quest.Name = "quest"
quest.Parent = ScreenGui
quest.BackgroundColor3 = Color3.new(0, 0, 0)
quest.Position = UDim2.new(0.0203577988, 0, 0.641277611, 0)
quest.Size = UDim2.new(0, 432, 0, 291)
quest.Visible = false
quest.Active = true
quest.Draggable = true

charqol.Name = "charqol"
charqol.Parent = ScreenGui
charqol.BackgroundColor3 = Color3.new(0, 0, 0)
charqol.Position = UDim2.new(0.0203577988, 0, 0.641277611, 0)
charqol.Size = UDim2.new(0, 432, 0, 291)
charqol.Visible = false
charqol.Active = true
charqol.Draggable = true

TeleportMenu.Name = "TeleportMenu"
TeleportMenu.Parent = ScreenGui
TeleportMenu.BackgroundColor3 = Color3.new(0, 0, 0)
TeleportMenu.Position = UDim2.new(0.0203577988, 0, 0.641277611, 0)
TeleportMenu.Size = UDim2.new(0, 432, 0, 291)
TeleportMenu.Visible = false
TeleportMenu.Active = true
TeleportMenu.Draggable = true

title.Name = "title"
title.Parent = main
title.BackgroundColor3 = Color3.new(1, 0, 1)
title.Size = UDim2.new(0, 332, 0, 31)
title.Font = Enum.Font.GothamBold
title.Text = "Bacon'§ V4"
title.TextColor3 = Color3.new(0, 0, 0)
title.TextSize = 14

toolsTitle.Name = "toolsTitle"
toolsTitle.Parent = tools
toolsTitle.BackgroundColor3 = Color3.new(1, 0, 1)
toolsTitle.Size = UDim2.new(0, 332, 0, 31)
toolsTitle.Font = Enum.Font.GothamBold
toolsTitle.Text = "Tool Menu"
toolsTitle.TextColor3 = Color3.new(0, 0, 0)
toolsTitle.TextSize = 14

QuestTitle.Name = "QuestTitle"
QuestTitle.Parent = quest
QuestTitle.BackgroundColor3 = Color3.new(1, 0, 1)
QuestTitle.Size = UDim2.new(0, 332, 0, 31)
QuestTitle.Font = Enum.Font.GothamBold
QuestTitle.Text = "Quest Menu"
QuestTitle.TextColor3 = Color3.new(0, 0, 0)
QuestTitle.TextSize = 14

CharTitle.Name = "CharTitle"
CharTitle.Parent = charqol
CharTitle.BackgroundColor3 = Color3.new(1, 0, 1)
CharTitle.Size = UDim2.new(0, 332, 0, 31)
CharTitle.Font = Enum.Font.GothamBold
CharTitle.Text = "Character Menu"
CharTitle.TextColor3 = Color3.new(0, 0, 0)
CharTitle.TextSize = 14

TeleportTitle.Name = "TeleportTitle"
TeleportTitle.Parent = TeleportMenu
TeleportTitle.BackgroundColor3 = Color3.new(1, 0, 1)
TeleportTitle.Size = UDim2.new(0, 332, 0, 31)
TeleportTitle.Font = Enum.Font.GothamBold
TeleportTitle.Text = "Teleport Menu"
TeleportTitle.TextColor3 = Color3.new(0, 0, 0)
TeleportTitle.TextSize = 14

Te.Name = "Te"
Te.Parent = main
Te.BackgroundColor3 = Color3.new(0.333333, 1, 0)
Te.Size = UDim2.new(0, 110, 0, 50)
Te.Font = Enum.Font.GothamBold
Te.Text = "Teleport"
Te.Position = UDim2.new(0.679518092, 0, 0.38, 0)
Te.TextColor3 = Color3.new(0, 0, 0)
Te.TextScaled = true
Te.TextSize = 14
Te.TextWrapped = true
Te.MouseButton1Down:connect(function()
main.Visible = false
TeleportMenu.Visible = true
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Teleport";
        Text = "Teleport To Secret Event";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

PengChar.Name = "PengChar"
PengChar.Parent = charqol
PengChar.BackgroundColor3 = Color3.new(0.333333, 1, 0)
PengChar.Size = UDim2.new(0, 110, 0, 50)
PengChar.Font = Enum.Font.GothamBold
PengChar.Text = "Penguin"
PengChar.Position = UDim2.new(0.679518092, 0, 0.38, 0)
PengChar.TextColor3 = Color3.new(0, 0, 0)
PengChar.TextScaled = true
PengChar.TextSize = 14
PengChar.TextWrapped = true
PengChar.MouseButton1Down:connect(function()
game:GetService("Workspace").ChangeCharacter:FireServer("PenguinCharacter")
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Character";
        Text = "Success to be Penguin";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

speedx.Name = "speedx"
speedx.Parent = tools
speedx.BackgroundColor3 = Color3.new(0.333333, 1, 0)
speedx.Position = UDim2.new(0.679518092, 0, 0.63, 0)
speedx.Size = UDim2.new(0, 110, 0, 50)
speedx.Font = Enum.Font.GothamBold
speedx.Text = "2x walk speed"
speedx.TextColor3 = Color3.new(0, 0, 0)
speedx.TextScaled = true
speedx.TextSize = 10
speedx.TextWrapped = true
speedx.MouseButton1Down:connect(function()
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 32
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Speed";
        Text = "our walk speed is now x2";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

discord.Name = "Discord"
discord.Parent = main
discord.BackgroundColor3 = Color3.new(0.333333, 1, 0)
discord.Size = UDim2.new(0, 110, 0, 50)
discord.Font = Enum.Font.GothamBold
discord.Text = "Discord"
discord.Position = UDim2.new(0.679518092, 0, 0.63, 0)
discord.TextColor3 = Color3.new(0, 0, 0)
discord.TextScaled = true
discord.TextSize = 14
discord.TextWrapped = true
discord.MouseButton1Down:connect(function()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Link";
        Text = "https://discord.gg/uw54YhR94T";
        Icon = "rbxthumb://type=Avatar&id=3044336136&w=150&h=150"})
Duration = 16;
end)

jumpx.Name = "jumpx"
jumpx.Parent = tools
jumpx.BackgroundColor3 = Color3.new(0.333333, 1, 0)
jumpx.Position = UDim2.new(0.35518092, 0, 0.63, 0)
jumpx.Size = UDim2.new(0, 110, 0, 50)
jumpx.Font = Enum.Font.GothamBold
jumpx.Text = "2x hight jump"
jumpx.TextColor3 = Color3.new(0, 0, 0)
jumpx.TextScaled = true
jumpx.TextSize = 10
jumpx.TextWrapped = true
jumpx.MouseButton1Down:connect(function()
game.Players.LocalPlayer.Character.Humanoid.JumpPower = 100
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Jump";
        Text = "our power of jump is now x2";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

winter.Name = "Winter"
winter.Parent = TeleportMenu
winter.BackgroundColor3 = Color3.new(0.333333, 1, 0)
winter.Size = UDim2.new(0, 110, 0, 50)
winter.Font = Enum.Font.GothamBold
winter.Text = "Winter"
winter.Position = UDim2.new(0.679518092, 0, 0.38, 0)
winter.TextColor3 = Color3.new(0, 0, 0)
winter.TextScaled = true
winter.TextSize = 14
winter.TextWrapped = true
winter.MouseButton1Down:connect(function()
game:GetService("TeleportService"):Teleport(1930866268, LocalPlayer)
end)

infox.Name = "InfoX"
infox.Parent = main
infox.BackgroundColor3 = Color3.new(0.333333, 1, 0)
infox.Position = UDim2.new(0.35518092, 0, 0.38, 0)
infox.Size = UDim2.new(0, 110, 0, 50)
infox.Font = Enum.Font.GothamBold
infox.Text = "End Script"
infox.TextColor3 = Color3.new(0, 0, 0)
infox.TextScaled = true
infox.TextSize = 14
infox.TextWrapped = true
infox.MouseButton1Down:connect(function()
openmain.Visible = false
main.Visible = false
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "GoodBye";
        Text = "Script Has Ended";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

FoxChar.Name = "FoxChar"
FoxChar.Parent = charqol
FoxChar.BackgroundColor3 = Color3.new(0.333333, 1, 0)
FoxChar.Position = UDim2.new(0.35518092, 0, 0.38, 0)
FoxChar.Size = UDim2.new(0, 110, 0, 50)
FoxChar.Font = Enum.Font.GothamBold
FoxChar.Text = "Fox"
FoxChar.TextColor3 = Color3.new(0, 0, 0)
FoxChar.TextScaled = true
FoxChar.TextSize = 14
FoxChar.TextWrapped = true
FoxChar.MouseButton1Down:connect(function()
game:GetService("Workspace").ChangeCharacter:FireServer("FoxCharacter")
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Character";
        Text = "Success to be Fox";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

ShiftlockS.Name = "ShiftlockS"
ShiftlockS.Parent = tools
ShiftlockS.BackgroundColor3 = Color3.new(0.333333, 1, 0)
ShiftlockS.Position = UDim2.new(0.35518092, 0, 0.38, 0)
ShiftlockS.Size = UDim2.new(0, 110, 0, 50)
ShiftlockS.Font = Enum.Font.GothamBold
ShiftlockS.Text = "Shiftlock Button"
ShiftlockS.TextColor3 = Color3.new(0, 0, 0)
ShiftlockS.TextScaled = true
ShiftlockS.TextSize = 14
ShiftlockS.TextWrapped = true
ShiftlockS.MouseButton1Down:connect(function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/rdpmakers/RoblosBabft/main/shift"))()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Tool";
        Text = "Shiftlock Button Enabled!";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

ChatBypasser.Name = "ChatBypasser"
ChatBypasser.Parent = tools
ChatBypasser.BackgroundColor3 = Color3.new(0.333333, 1, 0)
ChatBypasser.Size = UDim2.new(0, 110, 0, 50)
ChatBypasser.Font = Enum.Font.GothamBold
ChatBypasser.Text = "Steal Build"
ChatBypasser.Position = UDim2.new(0.679518092, 0, 0.38, 0)
ChatBypasser.TextColor3 = Color3.new(0, 0, 0)
ChatBypasser.TextScaled = true
ChatBypasser.TextSize = 14
ChatBypasser.TextWrapped = true
ChatBypasser.MouseButton1Down:connect(function()
loadstring(game:HttpGet(("https://raw.githubusercontent.com/StenDirt/Trash-Game/main/Script.lua")))()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Tool";
        Text = "U can swear Word now!";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

ccharacter.Name = "CCharacter"
ccharacter.Parent = main
ccharacter.BackgroundColor3 = Color3.new(0.333333, 1, 0)
ccharacter.Position = UDim2.new(0.35518092, 0, 0.63, 0)
ccharacter.Size = UDim2.new(0, 110, 0, 50)
ccharacter.Font = Enum.Font.GothamBold
ccharacter.Text = "Character"
ccharacter.TextColor3 = Color3.new(0, 0, 0)
ccharacter.TextScaled = true
ccharacter.TextSize = 14
ccharacter.TextWrapped = true
ccharacter.MouseButton1Down:connect(function()
main.Visible = false
charqol.Visible = true
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Character";
        Text = "You Can Be Animal Character";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

spider.Name = "spider"
spider.Parent = TeleportMenu
spider.BackgroundColor3 = Color3.new(0.333333, 1, 0)
spider.Position = UDim2.new(0.35518092, 0, 0.38, 0)
spider.Size = UDim2.new(0, 110, 0, 50)
spider.Font = Enum.Font.GothamBold
spider.Text = "SPIDER"
spider.TextColor3 = Color3.new(0, 0, 0)
spider.TextScaled = true
spider.TextSize = 14
spider.TextWrapped = true
spider.MouseButton1Down:connect(function()
game:GetService("TeleportService"):Teleport(1930665568, LocalPlayer)
end)

pqst.Name = "PresentQuest"
pqst.Parent = quest
pqst.BackgroundColor3 = Color3.new(0.333333, 1, 0)
pqst.Position = UDim2.new(0.35518092, 0, 0.38, 0)
pqst.Size = UDim2.new(0, 110, 0, 50)
pqst.Font = Enum.Font.GothamBold
pqst.Text = "Present"
pqst.TextColor3 = Color3.new(0, 0, 0)
pqst.TextScaled = true
pqst.TextSize = 14
pqst.TextWrapped = true
pqst.MouseButton1Down:connect(function()
game.Workspace.QuestMakerEvent:FireServer(99)
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Present Quest";
        Text = "Win= get 150 golds";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

chqst.Name = "ChristmasQuest"
chqst.Parent = quest
chqst.BackgroundColor3 = Color3.new(0.333333, 1, 0)
chqst.Position = UDim2.new(0.679518092, 0, 0.38, 0)
chqst.Size = UDim2.new(0, 110, 0, 50)
chqst.Font = Enum.Font.GothamBold
chqst.Text = "Chirstmas"
chqst.TextColor3 = Color3.new(0, 0, 0)
chqst.TextScaled = true
chqst.TextSize = 14
chqst.TextWrapped = true
chqst.MouseButton1Down:connect(function()
game.Workspace.QuestMakerEvent:FireServer(101)
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "2021 Christmas quest";
        Text = "Win= get free trowel tool";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

Text.Name = "Text"
Text.Parent = main
Text.BackgroundColor3 = Color3.new(0.333333, 1, 0)
Text.Position = UDim2.new(0.036144577, 0, 0.379146934, 0)
Text.Size = UDim2.new(0, 110, 0, 50)
Text.Font = Enum.Font.GothamBold
Text.Text = "Quest"
Text.TextColor3 = Color3.new(0, 0, 0)
Text.TextScaled = true
Text.TextSize = 10
Text.TextWrapped = true
Text.MouseButton1Down:connect(function()
main.Visible = false
quest.Visible = true
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Quest";
        Text = "Spawn Secret Quest";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

BeAdmin.Name = "BeAdmin"
BeAdmin.Parent = tools
BeAdmin.BackgroundColor3 = Color3.new(0.333333, 1, 0)
BeAdmin.Position = UDim2.new(0.036144577, 0, 0.379146934, 0)
BeAdmin.Size = UDim2.new(0, 110, 0, 50)
BeAdmin.Font = Enum.Font.GothamBold
BeAdmin.Text = "Admin"
BeAdmin.TextColor3 = Color3.new(0, 0, 0)
BeAdmin.TextScaled = true
BeAdmin.TextSize = 10
BeAdmin.TextWrapped = true
BeAdmin.MouseButton1Down:connect(function()
loadstring(game:HttpGet(('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'),true))()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Tools";
        Text = "Now u can use admin";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

adminC.Name = "adminC"
adminC.Parent = main
adminC.BackgroundColor3 = Color3.new(0.333333, 1, 0)
adminC.Position = UDim2.new(0.036144577, 0, 0.63, 0)
adminC.Size = UDim2.new(0, 110, 0, 50)
adminC.Font = Enum.Font.GothamBold
adminC.Text = "tools"
adminC.TextColor3 = Color3.new(0, 0, 0)
adminC.TextScaled = true
adminC.TextSize = 10
adminC.TextWrapped = true
adminC.MouseButton1Down:connect(function()
main.Visible = false
tools.Visible = true
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Info";
        Text = "U can use other tool from here";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

healthx.Name = "healthx"
healthx.Parent = tools
healthx.BackgroundColor3 = Color3.new(0.333333, 1, 0)
healthx.Position = UDim2.new(0.036144577, 0, 0.63, 0)
healthx.Size = UDim2.new(0, 110, 0, 50)
healthx.Font = Enum.Font.GothamBold
healthx.Text = "Anti Afk"
healthx.TextColor3 = Color3.new(0, 0, 0)
healthx.TextScaled = true
healthx.TextSize = 10
healthx.TextWrapped = true
healthx.MouseButton1Down:connect(function()
loadstring(game:HttpGet(('https://raw.githubusercontent.com/Proxylol/OtherScripts/main/AntiAfk.lua'),true))()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Anti afk";
        Text = "Enabled!";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

farmgold.Name = "farmgold"
farmgold.Parent = tools
farmgold.BackgroundColor3 = Color3.new(0.333333, 1, 0)
farmgold.Position = UDim2.new(0.036144577, 0, 0.84, 0)
farmgold.Size = UDim2.new(0, 110, 0, 50)
farmgold.Font = Enum.Font.GothamBold
farmgold.Text = "Fly"
farmgold.TextColor3 = Color3.new(0, 0, 0)
farmgold.TextScaled = true
farmgold.TextSize = 14
farmgold.TextWrapped = true
farmgold.MouseButton1Down:connect(function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/rdpmakers/RoblosBabft/main/Fly"))()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Fly";
        Text = "Enabled";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

farmgoldv2.Name = "farmgoldv2"
farmgoldv2.Parent = tools
farmgoldv2.BackgroundColor3 = Color3.new(0.333333, 1, 0)
farmgoldv2.Position = UDim2.new(0.35518092, 0, 0.84, 0)
farmgoldv2.Size = UDim2.new(0, 110, 0, 50)
farmgoldv2.Font = Enum.Font.GothamBold
farmgoldv2.Text = "Afk Farm"
farmgoldv2.TextColor3 = Color3.new(0, 0, 0)
farmgoldv2.TextScaled = true
farmgoldv2.TextSize = 14
farmgoldv2.TextWrapped = true
farmgoldv2.MouseButton1Down:connect(function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/rdpmakers/RoblosBabft/main/FarmV2"))()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Afk Farm";
        Text = "Enabled";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

iloader.Name = "iloader"
iloader.Parent = tools
iloader.BackgroundColor3 = Color3.new(0.333333, 1, 0)
iloader.Position = UDim2.new(0.679518092, 0, 0.84, 0)
iloader.Size = UDim2.new(0, 110, 0, 50)
iloader.Font = Enum.Font.GothamBold
iloader.Text = "Free Animation Script"
iloader.TextColor3 = Color3.new(0, 0, 0)
iloader.TextScaled = true
iloader.TextSize = 14
iloader.TextWrapped = true
iloader.MouseButton1Down:connect(function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/rdpmakers/RoblosBabft/main/TestSc"))()
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Info";
        Text = "u can USE FREE ANIMATION OF WALK";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

ChickChar.Name = "ChickChar"
ChickChar.Parent = charqol
ChickChar.BackgroundColor3 = Color3.new(0.333333, 1, 0)
ChickChar.Position = UDim2.new(0.036144577, 0, 0.379146934, 0)
ChickChar.Size = UDim2.new(0, 110, 0, 50)
ChickChar.Font = Enum.Font.GothamBold
ChickChar.Text = "Chicken"
ChickChar.TextColor3 = Color3.new(0, 0, 0)
ChickChar.TextScaled = true
ChickChar.TextSize = 10
ChickChar.TextWrapped = true
ChickChar.MouseButton1Down:connect(function()
game:GetService("Workspace").ChangeCharacter:FireServer("ChickenCharacter")
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Character";
        Text = "Success to be Chicken";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

fabbi.Name = "FabbiQuest"
fabbi.Parent = quest
fabbi.BackgroundColor3 = Color3.new(0.333333, 1, 0)
fabbi.Position = UDim2.new(0.036144577, 0, 0.379146934, 0)
fabbi.Size = UDim2.new(0, 110, 0, 50)
fabbi.Font = Enum.Font.GothamBold
fabbi.Text = "Fabbi"
fabbi.TextColor3 = Color3.new(0, 0, 0)
fabbi.TextScaled = true
fabbi.TextSize = 10
fabbi.TextWrapped = true
fabbi.MouseButton1Down:connect(function()
game.Workspace.QuestMakerEvent:FireServer(100)
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Fabbi";
        Text = "u Can get bread uf u defeat the boss";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

InnerCloud.Name = "InnerCloud"
InnerCloud.Parent = TeleportMenu
InnerCloud.BackgroundColor3 = Color3.new(0.333333, 1, 0)
InnerCloud.Position = UDim2.new(0.036144577, 0, 0.379146934, 0)
InnerCloud.Size = UDim2.new(0, 110, 0, 50)
InnerCloud.Font = Enum.Font.GothamBold
InnerCloud.Text = "InnerCloud"
InnerCloud.TextColor3 = Color3.new(0, 0, 0)
InnerCloud.TextScaled = true
InnerCloud.TextSize = 10
InnerCloud.TextWrapped = true
InnerCloud.MouseButton1Down:connect(function()
game:GetService("TeleportService"):Teleport(1930863474, LocalPlayer)
end)

close.Name = "close"
close.Parent = main
close.BackgroundColor3 = Color3.new(1, 0, 0)
close.Position = UDim2.new(0.879518092, 0, 0, 0)
close.Size = UDim2.new(0, 40, 0, 31)
close.Font = Enum.Font.GothamBlack
close.Text = "X"
close.TextColor3 = Color3.new(0, 0, 0)
close.TextScaled = true
close.TextSize = 14
close.TextWrapped = true
close.MouseButton1Down:connect(function()
main.Visible = false
openmain.Visible = true
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Info";
        Text = "Menu Closed!";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)

QuestClose.Name = "QuestClose"
QuestClose.Parent = quest
QuestClose.BackgroundColor3 = Color3.new(1, 0, 0)
QuestClose.Position = UDim2.new(0.879518092, 0, 0, 0)
QuestClose.Size = UDim2.new(0, 40, 0, 31)
QuestClose.Font = Enum.Font.GothamBlack
QuestClose.Text = "X"
QuestClose.TextColor3 = Color3.new(0, 0, 0)
QuestClose.TextScaled = true
QuestClose.TextSize = 14
QuestClose.TextWrapped = true
QuestClose.MouseButton1Down:connect(function()
main.Visible = true
quest.Visible = false
end)

TeleportClose.Name = "TeleportClose"
TeleportClose.Parent = TeleportMenu
TeleportClose.BackgroundColor3 = Color3.new(1, 0, 0)
TeleportClose.Position = UDim2.new(0.879518092, 0, 0, 0)
TeleportClose.Size = UDim2.new(0, 40, 0, 31)
TeleportClose.Font = Enum.Font.GothamBlack
TeleportClose.Text = "X"
TeleportClose.TextColor3 = Color3.new(0, 0, 0)
TeleportClose.TextScaled = true
TeleportClose.TextSize = 14
TeleportClose.TextWrapped = true
TeleportClose.MouseButton1Down:connect(function()
main.Visible = true
TeleportMenu.Visible = false
end)

toolsClose.Name = "toolsClose"
toolsClose.Parent = tools
toolsClose.BackgroundColor3 = Color3.new(1, 0, 0)
toolsClose.Position = UDim2.new(0.879518092, 0, 0, 0)
toolsClose.Size = UDim2.new(0, 40, 0, 31)
toolsClose.Font = Enum.Font.GothamBlack
toolsClose.Text = "X"
toolsClose.TextColor3 = Color3.new(0, 0, 0)
toolsClose.TextScaled = true
toolsClose.TextSize = 14
toolsClose.TextWrapped = true
toolsClose.MouseButton1Down:connect(function()
main.Visible = true
tools.Visible = false
end)

CharClose.Name = "CharClose"
CharClose.Parent = charqol
CharClose.BackgroundColor3 = Color3.new(1, 0, 0)
CharClose.Position = UDim2.new(0.879518092, 0, 0, 0)
CharClose.Size = UDim2.new(0, 40, 0, 31)
CharClose.Font = Enum.Font.GothamBlack
CharClose.Text = "X"
CharClose.TextColor3 = Color3.new(0, 0, 0)
CharClose.TextScaled = true
CharClose.TextSize = 14
CharClose.TextWrapped = true
CharClose.MouseButton1Down:connect(function()
main.Visible = true
charqol.Visible = false
end)

openmain.Name = "openmain"
openmain.Parent = ScreenGui
openmain.BackgroundColor3 = Color3.new(1, 1, 1)
openmain.Position = UDim2.new(0.00801973976, 0, 0.423832953, 0)
openmain.Size = UDim2.new(0, 100, 0, 28)
openmain.Active = true
openmain.Draggable = true

open.Name = "open"
open.Parent = openmain
open.BackgroundColor3 = Color3.new(1, 0, 0)
open.Size = UDim2.new(0, 100, 0, 28)
open.Font = Enum.Font.GothamBold
open.Text = "MENU"
open.TextColor3 = Color3.new(0, 0, 0)
open.TextSize = 18
open.TextWrapped = true
open.Draggable = true
open.MouseButton1Down:connect(function()
openmain.Visible = false
main.Visible = true
game:GetService("StarterGui"):SetCore("SendNotification", { 
        Title = "Menu";
        Text = "The menu";
        Icon = "rbxthumb://type=AvatarHeadShot&id=3044336136&w=150&h=150"})
Duration = 16;
end)
