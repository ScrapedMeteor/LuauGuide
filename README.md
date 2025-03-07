# Luau guide

# Printing and comments

```lua
-- this is a comment 
print("hi")
--[[
    This is a multi layer comment
]]
```

# Variables
```lua
local leaked = sigma
local IsAlive = lol
```

# Math

operators
- \+ addition
- \- minus
- \* multiply
- / divide
- ^ power
- % modulus

```lua
-- example

local Age = 18
local NewAge = Age + 5
print(NewAge)
```

# Boolean

local rizz = false
local aura = true

# Math Comparsion

- == equality
- < less than
- \> greater than
- <= less than or equal to
- \>= greater than or equal to
- ~= inequality

```lua
--example 
local MarriageAge = 23
if MarriageAge < 23 then
    print("no marriage :(")
end
```

# Functions
```lua
local function rizz_up_girl()
    print("hey cutie")
end
rizz_up_girl
```

# Services
- cloneref (Copys userdata from one to another) (Help avoid detections)

```lua
-- /w cloneref
local Players: Players = game:GetService('Players')
-- w/ cloneref
local HttpService = cloneref(game:GetService('HttpService'))
```
