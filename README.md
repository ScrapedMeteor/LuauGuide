# Luau guide
- Thanks to stav and qwertyui-is-back for inspriation from their fork of mine 

# Printing 

```lua
-- there are three types of prints
error("hookfunction not found")
warn("may not contain meta tables")
print("100% useable")
-- Error is used when an error in the executor is found such as not getfenv or any other function such as hookfunction
```

# Comments
```lua
-- This is a one lined comment
--[[
    This is a
    multi layer comment 
]]
```

# Math

Opperators

- \+ addition
- \- minus
- \* multiply
- / divide
- ^ power
- % modulus
- math.huge

```lua
-- example
local age = 30
newage = 30*2
```

# Math comparsion

Opperators

- == equality
- < less than
- \> greater than
- <= less than or equal to
- \>= greater than or equal to
- ~= inequality

```lua
-- example
local DrinkingAge = 21
local OtherAge = math.huge
if DrinkingAge ~= OtherAge then
    print ("no drunk :(")

```

# Functions

```lua
local function rizz_up_girl()
    print("hey cutie")
end
rizz_up_girl
```

# Tables
```lua
local girls_hooked_up_with = {
    "Natalie"
    "Mary"
    "Jane"
}
```

# Variables 
```lua
local hookupbuddy = john
local rizz = infinte
```

# Boolean 
``lua
local hawktuah = true
local talktuah = false
```

# Services
```lua
local lplr = playersService.LocalPlayer
local playersService = game:GetService('Players')
```

# MetaTable
```lua 
local metaTable = {
    __index = function()
        print("sigma")
    end,

    __newindex = function()
        print("new sigma")
    end
}
```
