local targetGameId = 118677256126351

if not game:IsLoaded() then
    game.Loaded:Wait()
end

if game.PlaceId == targetGameId or game.GameId == targetGameId then
    print("[Solix Loader] Game detected! Loading Bomb Fishing script...")
    
    local success, err = pcall(function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/YOUR_GITHUB_NAME/YOUR_REPO_NAME/main/BombFishing_Obfuscated.lua"))()
    end)

    if not success then
        warn("[Solix Loader] Failed to load script: " .. tostring(err))
    end
else
    local LocalPlayer = game.Players.LocalPlayer
    if LocalPlayer then
        LocalPlayer:Kick("\n[Solix Loader]\nThis script is only supported for Bomb Fishing!\nPlease join the correct game.")
    else
        warn("[Solix Loader] Wrong game detected! Expected ID: " .. tostring(targetGameId))
    end
end
