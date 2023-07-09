# Imgui Example
```lua

local library = loadstring(game:HttpGet(("https://raw.githubusercontent.com/memejames/Imgui/main/Library"),true))()
```

Create Window Here:
```lua
local window = library:AddWindow("Name GUI", {
	main_color = Color3.fromRGB(41, 74, 122), -- Color
	min_size = Vector2.new(250, 346), -- Size of the gui
	can_resize = false, -- true or false
})
```
create tab:
```lua
local features = window:AddTab("Features") -- Name of tab
features:Show() -- shows the tab
```
create button:
```lua
features:AddButton("name",function()
	-- Code here
end)
```
create toggle:
```lua
local switch = features:AddSwitch("name", function(bool)
	 -- toggle_god_mode(bool)
end)
switch:Set(true)
```
AddTextBox:
```lua
features:AddTextBox("free click", function(text)
	game:GetService("ReplicatedStorage").Events.FreeGifts.Gift2:FireServer(text,"Click",false,false,"Normal")
end)
```
