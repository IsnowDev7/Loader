# Loader
## Airflow lifecycle options

`AutoExecute` accepts a raw URL, Lua source string, or function. A raw URL is fetched and executed after the window is created. `AutoReconnect = true` listens for teleport failures and Roblox disconnect/shutdown messages, then attempts to rejoin the current place after a short delay.

```lua
local Airflow = loadstring(game:HttpGet(
    "https://raw.githubusercontent.com/IsnowDev7/Loader/main/Source.luau.txt"
))()

local Window = Airflow:CreateWindow({
    Name = "My Hub",
    AutoExecute = "https://example.com/your-script.lua",
    AutoReconnect = true,
})
```
