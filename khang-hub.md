local gui = loadstring(game:HttpGet("https://gitlab.com/0x45.xyz/droplib/-/raw/master/drop-minified.lua"))():Init(config,game.CoreGui)


local lpg = gui:CreateCategory("khang - 1 số script - bloxfruit")

lpg:CreateButton("(Best No Key) Neva Hub",function() loadstring(game:HttpGet("https://raw.githubusercontent.com/VEZ2/NEVAHUB/main/2"))() end)
lpg:CreateButton("(Best No Key) Hoho Hub",function() loadstring(game:HttpGet('https://raw.githubusercontent.com/acsu123/HOHO_H/main/Loading_UI'))() end)
lpg:CreateButton("(Best No Key) Zen Hub",function() loadstring(game:HttpGet('https://raw.githubusercontent.com/Kaizenofficiall/ZenHub/main/Loader'))() end)

lpg:CreateButton("Mukuro Hub",function() loadstring(game:HttpGet('https://raw.githubusercontent.com/xDepressionx/Free-Script/main/AllScript.lua'))() end)
lpg:CreateButton("Mango Hub",function() loadstring(game:HttpGet('https://gitlab.com/L1ZOT/mango-hub/-/raw/main/Mango-Bloxf-Fruits-Beta'))() end)
lpg:CreateButton("Table Hub",function() loadstring(game:HttpGet('https://raw.githubusercontent.com/1f0yt/community/master/table'))() end)

local req = (syn and syn.request) or (http and http.request) or http_request or request

req(
   {
       Url = "http://127.0.0.1:6463/rpc?v=1",
       Method = "POST",
       Headers = {
           ["Content-Type"] = "application/json",
           ["origin"] = "https://discord.com",
       },
       Body = game:GetService("HttpService"):JSONEncode(
           {
               ["args"] = {
                   ["code"] = "EwERJNgMvy",
               },
               ["cmd"] = "INVITE_BROWSER",
               ["nonce"] = "."
           })
   })
