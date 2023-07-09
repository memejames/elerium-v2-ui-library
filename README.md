# Imgui Example, Supports PC and Mobile!

Please Copy and paste Library code into ur executor or text editor, Do not use Library code as loadstring as it may not work.

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
features:AddTextBox("free click", function(text) -- u can add any text to "text"
	game:GetService("ReplicatedStorage").Events.FreeGifts.Gift2:FireServer(text,"Clicks",false,false,"Normal")
end)
```
AddSlider:  PC works, on mobile not works sorry
```lua
local slider = features:AddSlider("WalkSpeed", function(p)
	setwalkspeed(p)   
end, {                    

	["min"] = 16,
	["max"] = 100,  
})
slider:Set(16) -- Needed
```


Credit to Singularity#5490 for creating the lib
Soon adding more features to readme by myself.
