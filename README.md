# RioUI
A gooning UI Library that is created by Proz (me).

Start with loading its Library and creating window.

```lua

-- Load the library
local RioUi = loadstring(game:HttpGet("https://gist.githubusercontent.com/prozprow87-netizen/5d843cfc1c41436c6a1ec439ac3f06ee/raw/114f28be9f6c110faceda0eb36da6c1806672cea/uilib.lua"))()

-- Create a window
local Window = RioUi:CreateWindow("rio is best")

```

And then, you create a tab:

```lua
local MainTab = Window:CreateTab("Main")
```

And then you put elements! :

Buttons (has confirmation):

```lua
Tab:AddButton(text, callback, requireConfirm, confirmMessage)
```

Toggles (has confirmation too!):

```lua
Tab:AddToggle(text, defaultState, callback, requireConfirm, confirmMessage)
```

Sliders (it even has stepper and reset):

```lua
Tab:AddSlider(text, min, max, default, callback, showStepper)
```

Dropdown:

```lua
Tab:AddDropdown(text, options, callback)
```

TextBox (it has copy button):

```lua
Tab:AddBox(placeholderText)
```

Paragraph:

```lua
Tab:AddParagraph(title, text)
```

Checklist (basically dropdown, but you can choose many things):

```lua
Tab:AddChecklist(text, options, callback)
```

Section:

```lua
Tab:AddSection(title, startCollapsed)
```

Labels:

```lua
Tab:AddLabel(text, rightText) -- rightText optional for dual labels.
```
Keybind:

```lua
Tab:AddBind(text, defaultKey, callback)
```

..

Floating Icons:
This icon can be customized, but when it isnt customized it will turn into the image of RioUI. 

It toggles UI on or off.

Notification:

```lua
Window:Notify(title, message, duration, type)
```

it has 4 types, 
info, error, warning, success

Info: Crimson color
Error: Red
Warning: Yellow
Success: Green

Console:

RioUI is having their own console. You can add your own prints, errors or warning.

Its the same as Notify, but its inside the console.

Console functions:
```lua
local Console = Window:CreateConsole(title, description)
Console:Toggle()
Console:Log(message, type) -- Types: "info", "warn", "error", "success"
```

Example Preview:

![Screenshot_2026-02-07-07-35-31-430_com roblox client-edit](https://github.com/user-attachments/assets/96622180-5d97-4d51-81ca-d538433950c4)

Thats kinda it, i can update this everyday if i was still motivated and had ideas.
Goodbye!
