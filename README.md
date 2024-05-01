print("Fortune Strike| Legends Of Speed")
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
Window = OrionLib:MakeWindow({Name = "Fortune Strike| Legends Of Speed", HidePremium = false, SaveConfig = true, ConfigFolder = "GolpedaFortuna", IntroText = "Sub to Tubaro Scripts" })

local Tab = Window:MakeTab({
	Name = "Farm City",
	Icon = "NoId",
	PremiumOnly = false
})

OrionLib:MakeNotification({
	Name = "Executed",
	Content = "Sub to Tubaro Script",
	Image = "rbxassetid://4483345998",
	Time = 5
})

local Section = Tab:AddSection({
	Name = "Orbs"
})

Tab:AddButton({
	Name = "Farm Orb Red",
	Callback = function()            OrionLib:MakeNotification({
	Name = "Red Orbs",
	Content = "Farming Orbs On City",
	Image = "rbxassetid://4483345998",
	Time = 5
})
      		print("button pressed")            while true do
  wait(0.00001)
local args = {
    [1] = "collectOrb",
    [2] = "Red Orb",
    [3] = "City"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("orbEvent"):FireServer(unpack(args))

local args = {
    [1] = "collectOrb",
    [2] = "Yellow Orb",
    [3] = "City"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("orbEvent"):FireServer(unpack(args))

local args = {
    [1] = "collectOrb",
    [2] = "Orange Orb",
    [3] = "City"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("orbEvent"):FireServer(unpack(args))


local args = {
    [1] = "collectOrb",
    [2] = "Blue Orb",
    [3] = "City"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("orbEvent"):FireServer(unpack(args))

     end
  	end    
})

Tab:AddButton({
	Name = "Get 1 Orb Red",
	Callback = function()            OrionLib:MakeNotification({
	Name = "Red Orbs",
	Content = "Geting 1 Orb On City",
	Image = "rbxassetid://4483345998",
	Time = 5
})
      		print("button pressed")
local args = {
    [1] = "collectOrb",
    [2] = "Red Orb",
    [3] = "City"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("orbEvent"):FireServer(unpack(args))
  	end    
})

local Section = Tab:AddSection({
	Name = "Gems"
})

Tab:AddButton({
	Name = "Farm Gems",
	Callback = function()            OrionLib:MakeNotification({
	Name = "Gems",
	Content = "Farming Gems",
	Image = "rbxassetid://4483345998",
	Time = 5
})
      		print("button pressed")     while true do
  wait(0.00001)
  local args = {
    [1] = "collectOrb",
    [2] = "Gem",
    [3] = "City"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("orbEvent"):FireServer(unpack(args))
  end
  	end    
})

Tab:AddButton({
	Name = "Get 1 Gems",
	Callback = function()      OrionLib:MakeNotification({
	Name = "Gems",
	Content = "Get 1 Gems Sucessfull",
	Image = "rbxassetid://4483345998",
	Time = 5
})
      		print("button pressed")       local args = {
    [1] = "collectOrb",
    [2] = "Gem",
    [3] = "City"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("orbEvent"):FireServer(unpack(args))

  	end    
})

local Section = Tab:AddSection({
	Name = "Rebirt"
})

Tab:AddButton({
	Name = "Auto Rebirt",
	Callback = function()
      		print("button pressed")          while true do
   wait(0.00001)
local args = {
    [1] = "rebirthRequest"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("rebirthEvent"):FireServer(unpack(args))
  end
  	end    
})



local Tab = Window:MakeTab({
	Name = "Pets",
	Icon = "",
	PremiumOnly = false
})
Tab:AddButton({
	Name = "Omega Pet",
	Callback = function()
      		print("button pressed")           local args = {
    [1] = "openCrystal",
    [2] = "Electro Legends Crystal"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("openCrystalRemote"):InvokeServer(unpack(args))
  	end    
})


Tab:AddButton({
	Name = "Blue Crystal",
	Callback = function()
      		print("button pressed")          local args = {
    [1] = "openCrystal",
    [2] = "Blue Crystal"
}

game:GetService("ReplicatedStorage"):WaitForChild("rEvents"):WaitForChild("openCrystalRemote"):InvokeServer(unpack(args))


  	end    
})

