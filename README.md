# revised-uis
Roblox service "UserInputService", interpreted and modified to hold needs of some players

Here's some basic code, explaining UserInputService is better with code:
```lua
local ruis = require(game.ReplicatedStorage.RevisedUserInput)

game:GetService("RunService"):RenderStepped:Connect(function(dt)
  if ruis:KeyHolding(ruis.Key.LeftShift) then
    -- the player is holding left shift
  end
end)

ruis.Input:Connect(function(key, gameControlled)
  if key == ruis.Key.B then
    -- this code will run when "B" is pressed
  end
end)
```
