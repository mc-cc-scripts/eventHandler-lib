# eventHandler-lib

This eventHandler simulates EventHandlers similar to those of C#

## Example

```lua
--- Require
---@class eventHandler
local eventHandler = require("eventHandler")

--- Init Event, do not forget that
local testEvent = eventHandler('Test')

--- Add as many callbacks for the Event as required
local callbackObj = testEvent:AddCallback(function(parameter)
    print(parameter)
end)

--- Invoke Event
testEvent:invoke('Started Callback with Id: ' .. callbackObj.callbackID)
```

![Executed](Images/Executed.png)
