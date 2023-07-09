# Imgui2

Create Window Here
```lua
local window = library:AddWindow("Name GUI", {
	main_color = Color3.fromRGB(41, 74, 122), -- Color
	min_size = Vector2.new(250, 346), -- Size of the gui
	can_resize = false, -- true or false
})
```
Make tab
```lua
local features = window:AddTab("Features")
features:Show()
```

```lua
