local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Robojini/Tuturial_UI_Library/main/UI_Template_1"))()
local Window = Library.CreateLib("Menu For nikitaukoi2", "RJTheme3")
local Tab = Window:NewTab("Main")
local Section = Tab:NewSection("Scripts")


Section:NewTextBox("Speed", "Super Speed", function(txt)
	game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = txt
end)


Section:NewTextBox("Jump", "JumpPower", function(txt)
	game.Players.LocalPlayer.Character.Humanoid.JumpPower = txt
end)


Section:NewButton("BTools", "Gives You BTools", function()
    loadstring(game:HttpGet("https://scriptblox.com/raw/Universal-Script-BTOOLS-8904", true))()
end)


Section:NewButton("VFly", "you can fly cars", function()
    loadstring(game:HttpGet("https://pastebin.com/raw/MHE1cbWF"))()
end)



Section:NewButton("Noclip", "Noclip Menu", function()
    local Workspace = game:GetService("Workspace")
local CoreGui = game:GetService("CoreGui")
local Players = game:GetService("Players")
local Noclip = Instance.new("ScreenGui")
local BG = Instance.new("Frame")
local Title = Instance.new("TextLabel")
local Toggle = Instance.new("TextButton")
local StatusPF = Instance.new("TextLabel")
local Status = Instance.new("TextLabel")
local Credit = Instance.new("TextLabel")
local Plr = Players.LocalPlayer
local Clipon = false
 
Noclip.Name = "Noclip"
Noclip.Parent = game.CoreGui
 
BG.Name = "BG"
BG.Parent = Noclip
BG.BackgroundColor3 = Color3.new(0.0980392, 0.0980392, 0.0980392)
BG.BorderColor3 = Color3.new(0.0588235, 0.0588235, 0.0588235)
BG.BorderSizePixel = 2
BG.Position = UDim2.new(0.149479166, 0, 0.82087779, 0)
BG.Size = UDim2.new(0, 210, 0, 127)
BG.Active = true
BG.Draggable = true
 
Title.Name = "Title"
Title.Parent = BG
Title.BackgroundColor3 = Color3.new(0.266667, 0.00392157, 0.627451)
Title.BorderColor3 = Color3.new(0.180392, 0, 0.431373)
Title.BorderSizePixel = 2
Title.Size = UDim2.new(0, 210, 0, 33)
Title.Font = Enum.Font.Highway
Title.Text = "Noclip"
Title.TextColor3 = Color3.new(1, 1, 1)
Title.FontSize = Enum.FontSize.Size32
Title.TextSize = 30
Title.TextStrokeColor3 = Color3.new(0.180392, 0, 0.431373)
Title.TextStrokeTransparency = 0
 
Toggle.Parent = BG
Toggle.BackgroundColor3 = Color3.new(0.266667, 0.00392157, 0.627451)
Toggle.BorderColor3 = Color3.new(0.180392, 0, 0.431373)
Toggle.BorderSizePixel = 2
Toggle.Position = UDim2.new(0.152380958, 0, 0.374192119, 0)
Toggle.Size = UDim2.new(0, 146, 0, 36)
Toggle.Font = Enum.Font.Highway
Toggle.FontSize = Enum.FontSize.Size28
Toggle.Text = "Toggle"
Toggle.TextColor3 = Color3.new(1, 1, 1)
Toggle.TextSize = 25
Toggle.TextStrokeColor3 = Color3.new(0.180392, 0, 0.431373)
Toggle.TextStrokeTransparency = 0
 
StatusPF.Name = "StatusPF"
StatusPF.Parent = BG
StatusPF.BackgroundColor3 = Color3.new(1, 1, 1)
StatusPF.BackgroundTransparency = 1
StatusPF.Position = UDim2.new(0.314285725, 0, 0.708661377, 0)
StatusPF.Size = UDim2.new(0, 56, 0, 20)
StatusPF.Font = Enum.Font.Highway
StatusPF.FontSize = Enum.FontSize.Size24
StatusPF.Text = "Status:"
StatusPF.TextColor3 = Color3.new(1, 1, 1)
StatusPF.TextSize = 20
StatusPF.TextStrokeColor3 = Color3.new(0.333333, 0.333333, 0.333333)
StatusPF.TextStrokeTransparency = 0
StatusPF.TextWrapped = true
 
Status.Name = "Status"
Status.Parent = BG
Status.BackgroundColor3 = Color3.new(1, 1, 1)
Status.BackgroundTransparency = 1
Status.Position = UDim2.new(0.580952346, 0, 0.708661377, 0)
Status.Size = UDim2.new(0, 56, 0, 20)
Status.Font = Enum.Font.Highway
Status.FontSize = Enum.FontSize.Size14
Status.Text = "off"
Status.TextColor3 = Color3.new(0.666667, 0, 0)
Status.TextScaled = true
Status.TextSize = 14
Status.TextStrokeColor3 = Color3.new(0.180392, 0, 0.431373)
Status.TextWrapped = true
Status.TextXAlignment = Enum.TextXAlignment.Left
 
Credit.Name = "Credit"
Credit.Parent = BG
Credit.BackgroundColor3 = Color3.new(1, 1, 1)
Credit.BackgroundTransparency = 1
Credit.Position = UDim2.new(0.195238099, 0, 0.866141737, 0)
Credit.Size = UDim2.new(0, 128, 0, 17)
Credit.Font = Enum.Font.SourceSans
Credit.FontSize = Enum.FontSize.Size18
Credit.Text = "Created by KingLuna"
Credit.TextColor3 = Color3.new(1, 1, 1)
Credit.TextSize = 16
Credit.TextStrokeColor3 = Color3.new(0.196078, 0.196078, 0.196078)
Credit.TextStrokeTransparency = 0
Credit.TextWrapped = true
 
Toggle.MouseButton1Click:connect(function()
    if Status.Text == "off" then
        Clipon = true
        Status.Text = "on"
        Status.TextColor3 = Color3.new(0,185,0)
        Stepped = game:GetService("RunService").Stepped:Connect(function()
            if not Clipon == false then
                for a, b in pairs(Workspace:GetChildren()) do
                if b.Name == Plr.Name then
                for i, v in pairs(Workspace[Plr.Name]:GetChildren()) do
                if v:IsA("BasePart") then
                v.CanCollide = false
                end end end end
            else
                Stepped:Disconnect()
            end
        end)
    elseif Status.Text == "on" then
        Clipon = false
        Status.Text = "off"
        Status.TextColor3 = Color3.new(170,0,0)
    end
end)
end)


Section:NewButton("Noclip Tool", "Gives You Noclip Tool", function()
    mouse = game.Players.LocalPlayer:GetMouse()
tool = Instance.new("Tool")
tool.RequiresHandle = false
tool.Name = ("Equip To Noclip")
tool.Activated:Connect(function()
game.Players.LocalPlayer.Character.Humanoid.MaxHealth = math.huge
game.Players.LocalPlayer.Character.Humanoid.Health = math.huge
while true do
		game:GetService("RunService").Stepped:wait()
		game.Players.LocalPlayer.Character.Head.CanCollide = false
		game.Players.LocalPlayer.Character.Torso.CanCollide = false
end
end)
tool.Parent = game.Players.LocalPlayer.Backpack
end)



local Tab = Window:NewTab("Misc")
local Section = Tab:NewSection("Menus")


Section:NewButton("Reviz Admin", "admin window", function()
    loadstring(game:HttpGet("https://scriptblox.com/raw/Reviz-Admin-FE_156", true))()
end)


Section:NewButton("Infinite Yield", "Infinite Yield", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)


Section:NewButton("Teleport", "enter a nickname in the menu and then you can teleport to the players", function()
    loadstring(game:HttpGet(("https://pastebin.com/raw/YNVbeqPy")))()
end)


local Tab = Window:NewTab("Fling Things And People")
local Section = Tab:NewSection("Super Power")


Section:NewButton("Super Power", "you throw things away", function()
    local userinputs = game:GetService("UserInputService")
local action = game:GetService("ContextActionService")
local w = game:GetService("Workspace")
local r = game:GetService("RunService")
local d = game:GetService("Debris")
local strength = 850
 
w.ChildAdded:Connect(function(model)
    if model.Name == "GrabParts" then
        local part_to_impulse = model["GrabPart"]["WeldConstraint"].Part1
 
        if part_to_impulse then
            print("Part found!")
 
            local inputObj
            local velocityObj = Instance.new("BodyVelocity", part_to_impulse)
            local c1, c2, c3
 
            velocityObj.MaxForce = Vector3.new(0,0,0)
 
            while inputObj == nil and model.Parent do
                for _, button in pairs(game.Players.LocalPlayer.PlayerGui["ContextActionGui"]:GetDescendants()) do
                    if button:IsA("ImageLabel") then
                        if button.Image == "http://www.roblox.com/asset/?id=9603678090" then
                            inputObj = button.Parent
                            print(inputObj)
                        end
                    end
                end

				r.Heartbeat:Wait()
            end
            
			if inputObj then
				c1 = inputObj.MouseButton1Up:Connect(function()
					print("Launched!")
					velocityObj.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
					velocityObj.Velocity = workspace.CurrentCamera.CFrame.lookVector * strength
            	end)
 
            	c2 = inputObj.MouseButton1Down:Connect(function()
              	  print("Launched!")
              	  velocityObj.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
              	  velocityObj.Velocity = workspace.CurrentCamera.CFrame.lookVector * strength
            	end)
			end
            
            
            c3 = model:GetPropertyChangedSignal("Parent"):Connect(function()
                if not model.Parent then
					c3:Disconnect()
                    d:AddItem(velocityObj, 1)

                    if c1 then
                        c1:Disconnect()
                        if c2 then
                            c2:Disconnect()
                        end
                    end
                end
            end)
        end
    end
end)
end)


local Section = Tab:NewSection("Super Speed")


Section:NewButton("Super Speed", "you are very fast", function()
    --[[ Variables ]]
local PS = game:GetService("Players")
local LocalPlayer = PS.LocalPlayer
local GameMt = getrawmetatable(game)
setreadonly(GameMt, false)
local OldIndex = GameMt.__index

GameMt.__index = function(Self, Key)
if not checkcaller() and Self then
       if Key == "WalkSpeed" then
   return 16
       elseif Key == "JumpPower" then
           return 24
       end
end

return OldIndex(Self, Key)
end

LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid").WalkSpeed = 28

function Int()
   for i,v in pairs(debug.getregistry()) do

       if type(v) == "function" and not is_synapse_function(v) then
           local Values = debug.getupvalues(v)
           for a,b in pairs(Values) do
               if type(b) == "number" and b == 20 then
                   debug.setupvalue(v, a, 30)
               end
           end

           local Constants = debug.getconstants(v)
           for Number,Value in pairs(Constants) do
               if type(Value) == "number" then
                   if Value == 100 then
                       debug.setconstant(v, Number, 1000)
                       print("Set new Magnitude limit!")
                   end
                   if Value == 750 then
                       debug.setconstant(v, Number, 1350)
                       print("Set new throw limit!")
                   end
               end
           end
       end

   end

   spawn(function()
       while wait() do
           if LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid") then
               LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid").JumpPower = 24
           LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid").WalkSpeed = 28
           elseif not LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid") then
               break
           end
       end
   end)

end

Int()

LocalPlayer.CharacterAdded:Connect(function()
   repeat wait() until LocalPlayer.Character
   repeat wait() until LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid")
   repeat wait() until LocalPlayer.Character:FindFirstChild("GrabbingScript")
   Int()
end)

print("Better reach and faster speed loaded!")
end)
    


local Tab = Window:NewTab("Doors")
local Section = Tab:NewSection("Menu")


Section:NewButton("King Hub", "King Hub Script", function()
    loadstring(game:HttpGet(('https://pastebin.com/raw/R8QMbhzv')))()
end)


Section:NewButton("PoopDoors", "PoopDoors Menu", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/zoophiliaphobic/POOPDOORS/main/script.lua'))()
end)


Section:NewButton("PoopDoors", "PoopDoors Edited Menu", function()
    loadstring(game:HttpGet(("https://raw.githubusercontent.com/mstudio45/poopdoors_edited/main/poopdoors_edited.lua"),true))()
end)

Section:NewButton("Doors Gui", "Doors Menu", function()
    loadstring(game:HttpGet(('https://pastebin.com/raw/9QPGnLx6'),true))()
end)


Section:NewButton("Chiba Doors", "Chiba Gui", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/KindIhave/ChibaHubcomeback/main/Chiba-Doors.txt'))()
end)


local Tab = Window:NewTab("Lumber Tycoon")
local Section = Tab:NewSection("Lumber Gui")


Section:NewButton("Lumber Gui", "Menu", function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/Butterisgood/butter-hub/main/Butterhub.txt'))()
end)



Section:NewButton("Max Land LT2 Gui", "LT2 Gui", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/EWMnNhV8'))()
end)


Section:NewButton("NOOBARMY LT2", "NOOBARMY Gui", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/NOOBARMYSCRIPTER/NOOBARMYSCRIPTER/main/AXE%20LOOP%20SCRIPT", true))();
end)


Section:NewButton("LT2 Dupe Gui", "Dupe Gui", function()
    loadstring(game:HttpGet'https://raw.githubusercontent.com/0x37Dev/Cool-Solo-Dupe-Thing/main/script.lua')()
end)



local Tab = Window:NewTab("Adopt Me")
local Section = Tab:NewSection("Adopt Menu")


Section:NewButton("Adopt Me", "Adopt Gui", function()
    loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/ahmadsgamer2/Script--Game/main/Script%20Game"))()
end)



local Tab = Window:NewTab("JailBreak")
local Section = Tab:NewSection("Menus")


Section:NewButton("JailBreak", "JailBroken Menu", function()
    loadstring(game:GetObjects("rbxassetid://3762448307")[1].Source)()
end)


local Tab = Window:NewTab("Time")
local Section = Tab:NewSection("Stop")


Section:NewButton("Time Stop", "Stops time", function()
    loadstring(game:HttpGet('https://pastebin.com/raw/djAd7g2W'))()
end)
