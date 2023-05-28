local kavoUi = loadstring(game:HttpGet("https://pastebin.com/raw/vff1bQ9F"))()

local window = kavoUi.CreateLib("+1 money for every click","BloodTheme")

 

---Tabs

 

local Tab1 = window:NewTab("Main")

local Tab1Section = Tab1:NewSection("Free Roblox Scripts")

local Tab2 = window:NewTab("Sup")

local Tab2Section = Tab2:NewSection("Sup is word")

local Tab1Section = Tab1:NewSection("Made By Skoter Scripts")

local Tab1Section = Tab1:NewSection("freerobloxscript.com")

 

---Buttons

Tab1Section:NewToggle("AutoClick", "Click automatic", function(state)

    if state then

_G.autoclick = true

   while _G.autoclick == true do

game:GetService("ReplicatedStorage"):FindFirstChild("events-shared/network@GlobalEvents").placeBlock:FireServer()

wait(0)

end

    else

_G.autoclick = false

end

end)

Tab1Section:NewToggle("Equip Best", "Equip Best Pet", function(state)

    if state then

_G.equipbest = true

   while _G.equipbest == true do

local args = {

    [1] = 17

}

game:GetService("ReplicatedStorage"):FindFirstChild("functions-shared/network@GlobalFunctions"):FindFirstChild("s:equipBestPets"):FireServer(unpack(args))

wait(5)

end

    else

_G.equipbest = false

end

end)

Tab1Section:NewToggle("AutoClaim", "Claim rewards automatic", function(state)

    if state then

_G.autoclaim = true

   while _G.autoclaim == true do

local args = {

    [1] = 0,

    [2] = 60

}

game:GetService("ReplicatedStorage"):FindFirstChild("functions-shared/network@GlobalFunctions"):FindFirstChild("s:claimTimeGift"):FireServer(unpack(args))

local args = {

    [1] = 4,

    [2] = 180

}

game:GetService("ReplicatedStorage"):FindFirstChild("functions-shared/network@GlobalFunctions"):FindFirstChild("s:claimTimeGift"):FireServer(unpack(args))

local args = {

    [1] = 2,

    [2] = 300

}

game:GetService("ReplicatedStorage"):FindFirstChild("functions-shared/network@GlobalFunctions"):FindFirstChild("s:claimTimeGift"):FireServer(unpack(args))

local args = {

    [1] = 3,

    [2] = 420

}

game:GetService("ReplicatedStorage"):FindFirstChild("functions-shared/network@GlobalFunctions"):FindFirstChild("s:claimTimeGift"):FireServer(unpack(args))

local args = {

    [1] = 5,

    [2] = 420

}

game:GetService("ReplicatedStorage"):FindFirstChild("functions-shared/network@GlobalFunctions"):FindFirstChild("s:claimTimeGift"):FireServer(unpack(args))

local args = {

    [1] = 6,

    [2] = 600

}

game:GetService("ReplicatedStorage"):FindFirstChild("functions-shared/network@GlobalFunctions"):FindFirstChild("s:claimTimeGift"):FireServer(unpack(args))

local args = {

    [1] = 7,

    [2] = 900

}

game:GetService("ReplicatedStorage"):FindFirstChild("functions-shared/network@GlobalFunctions"):FindFirstChild("s:claimTimeGift"):FireServer(unpack(args))

wait(10)

end

    else

_G.autoclaim = false

end

end)

Tab1Section:NewToggle("Auto Rebirth", "Rebirth automatic", function(state)

    if state then

_G.autorebirth = true

     while _G.autorebirth == true do

local args = {

    [1] = 8

}

game:GetService("ReplicatedStorage"):FindFirstChild("functions-shared/network@GlobalFunctions"):FindFirstChild("s:rebirth"):FireServer(unpack(args))

wait(10)

end

     else

_G.autorebirth = false

end

end)

Tab2Section:NewButton("Keyboard","Pc Like Keyboard",function()

loadstring(game:HttpGet(('https://raw.githubusercontent.com/manimcool21/Keyboard-FE/main/Protected%20(3).lua'),true))()

end)
