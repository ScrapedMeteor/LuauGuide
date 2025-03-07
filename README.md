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
local leaked = sigma -- nil because sigma isn't defined
local IsAlive = lol -- nil because lol isn't defined
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
print(NewAge) -- 23
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
rizz_up_girl()

local function rizz_up_boy(argument)
    print("hey "..argument)
end
rizz_up_boy("bud")
```
