# Window-Library-Lua-RBLX
Example Code

```lua
local Library = loadstring(Game:HttpGet("https://raw.githubusercontent.com/RN455/Window-Library-Lua-RBLX/refs/heads/main/library"))()



local MainWindow= Library:NewWindow("window title")



local MiniSection == MainWindow:NewSection("section title")



MiniWindow:CreateToggle("toggle button", function(value)

if value then

-- Code to execute when the toggle button is toggled on



-- Perform any actions or execute any code here

else

-- Code to execute when the toggle button is toggled off



end

-- Perform any actions or execute any code here

end

end)


MainWindow:CreateSlider(

    "WalkSpeed", -- The name displayed on the UI
    16,          -- Minimum value (Default Roblox speed)
    200,         -- Maximum value
    16,          -- Default starting value
    function(value)
        -- This code runs every time the slider is dragged
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
        print("Current Speed: " .. value)
    end
	
)
