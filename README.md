local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "Vn7 Hub",
   Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
   LoadingTitle = "Carregando Vn7 Hub",
   LoadingSubtitle = "by Vn7_Oficial",
   ShowText = "Rayfield", -- for mobile users to unhide rayfield, change if you'd like
   Theme = "Light", -- Check https://docs.sirius.menu/rayfield/configuration/themes

   ToggleUIKeybind = "K", -- The keybind to toggle the UI visibility (string like "K" or Enum.KeyCode)

   DisableRayfieldPrompts = false,
   DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface

   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Vn7 Hub"
   },

   Discord = {
      Enabled = true, -- Prompt the user to join your Discord server if their executor supports it
      Invite = "m7zMnpez", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },

   KeySystem = false, -- Set this to true to use our key system
   KeySettings = {
      Title = "Untitled",
      Subtitle = "Key System",
      Note = "No method of obtaining the key is provided", -- Use this to tell the user how to get a key
      FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"Hello"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})



local giros da sorte = Window:CreateTab("Tab Example", 4483362458) -- Title, Image


local Main = Window:CreateTab("Tab Example", 4483362458) -- Title, Image
      Enabled = true, -- Prompt the user to join your Discord server if their executor supports it
      Invite = "m7zMnpez", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },

   KeySystem = false, -- Set this to true to use our key system
   KeySettings = {
      Title = "Untitled",
      Subtitle = "Key System",
      Note = "No method of obtaining the key is provided", -- Use this to tell the user how to get a key
      FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"Hello"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","
   end,
})




local giros da sorte = Window:CreateTab("Tab Example", 4483362458) -- Title, Image


local Main = Window:CreateTab("Tab Example", 4483362458) -- Title, Image



local ButtonHabilidadeSorte = giros da sorte:CreateButton({
   Name = "Ganhar Habilidade da Sorte",
   Callback = function()
      local remote = game:GetService("ReplicatedStorage"):FindFirstChild("SpinSkill")
      if remote and remote:IsA("RemoteEvent") then
         remote:FireServer()
         Rayfield:Notify({
            Title = "Sucesso!",
            Content = "Você ganhou uma habilidade da sorte!",
            Duration = 3
         })
      else
         Rayfield:Notify({
            Title = "Erro",
            Content = "RemoteEvent 'SpinSkill' colocado.",
            Duration = 3
         })
      end
   end,
})



local SliderHitbox = Main:CreateSlider({
   Name = "Tamanho da Hitbox Verde",
   Range = {0, 40},
   Increment = 1,
   Suffix = "",
   CurrentValue = 0,
   Flag = "SliderHitbox",
   Callback = function(Value)
      hitboxValue = Value
   end,
})



local ButtonEstiloSorte = giros da sorte:CreateButton({
   Name = "Ganhar Estilo da Sorte",
   Callback = function()
      local remote = game:GetService("ReplicatedStorage"):FindFirstChild("SpinStyle")
      if remote and remote:IsA("RemoteEvent") then
         remote:FireServer()
         Rayfield:Notify({
            Title = "Sucesso!",
            Content = "Você ganhou um estilo da sorte!",
            Duration = 3
         })
      else
         Rayfield:Notify({
            Title = "Erro",
            Content = "RemoteEvent 'SpinStyle' colocado.",
            Duration = 3
         })
      end
   end,
})
