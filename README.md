> [!IMPORTANT]
> This guide may not have every function, take caution

# luaU for idiots/skids
Explains luaU for exploits in a user-friendly way!

## Printing/Comments
There are 3 types of print, (error, warn and print). Error has a second argument called (level), however its not required.
```lua
print('test')
warn('yo')
error('real') -- A comment
```

## Functions
Functions help in situations (e.g api) and clean code!
```lua
local function an4rch()
    print('an4rchist for life!!')
end
an4rch()
```

## Variables, Booleans, Services
Booleans are (true or false). Variables require two arguments. (name, (string or function or service or boolean))
```lua
local Skibidi = 'string' -- This is a string ''.
local Hawk = an4rch() -- Function inside a variable
local skibid = false -- Returns false
local Players: Players = game:GetService('Players') -- gets the players service
```

## Tables
Tables in luaU are powerful data structures that can be used as arrays, dictionaries, objects, functions and more.
```lua
an4rch = function() return 'asteria' end
local table = {
    test = 'yuh', -- Value of the key 'test'
    funcs = { -- Table in a table
        an4rch = an4rch()
    },
    'first', -- [1]
    123 -- [2]
}

-- Accessing, inserting, removing and sorting a table
print(table.test) -- outputs 'yuh'
print(table['test']) -- outputs 'yuh' but in a fancier way
print(table[1]) -- outputs 'first', in index[1] of the table
table.insert(table, 'new') -- adds 'new' to the end of the table
table.remove(table, 1) -- removes the first element of the table
table.concat({"a", "b", "c"}, "-") -- joins array elements (output: abc)

-- Loops (loop around the table)
for i,v in pairs(table) do
    print(v)
end
```

# Operators
- `+` Addition (adds two values together)

  ```lua
  local sum = 5 + 3 -- Returns 8
  ```
- `-` Subtraction (subtracts second value from first)

  ```lua
  local difference = 10 - 4 -- Returns 6
  ```
- `*` Multiplication (multiplies two values)

  ```lua
  local product = 6 * 2 -- Returns 12
  ```
- `/` Division (divides first value by second)

  ```lua
  local quotient = 15 / 3 -- Returns 5
  ```
- `^` Exponentiation (raises first value to power of second)

  ```lua
  local power = 2 ^ 3 -- Returns 8
  ```
- `%` Modulus (returns remainder after division)

  ```lua
  local remainder = 10 % 3 -- Returns 1
  ```

## Operator Comparison
- `==` Equal to

  ```lua
  print(5 == 5) -- Returns true
  print(5 == 6) -- Returns false
  ```
- `<` Less than

  ```lua
  print(3 < 5) -- Returns true
  print(5 < 3) -- Returns false
  ```
- `>` Greater than

  ```lua
  print(5 > 3) -- Returns true
  print(3 > 5) -- Returns false
  ```
- `<=` Less than or equal to

  ```lua
  print(3 <= 3) -- Returns true
  print(4 <= 3) -- Returns false
  ```
- `>=` Greater than or equal to

  ```lua
  print(3 >= 3) -- Returns true
  print(2 >= 3) -- Returns false
  ```
- `~=` Not equal to

  ```lua
  print(5 ~= 6) -- Returns true
  print(5 ~= 5) -- Returns false
  ```
## String Functions
```lua
-- string.split() divides a string by separator
local text = "apple,banana,orange"
local fruits = string.split(text, ",")  -- Returns {"apple", "banana", "orange"}

-- string.pack() and string.unpack() for binary data
local packed = string.pack("ii", 123, 456)    -- Packs numbers into binary
local num1, num2 = string.unpack("ii", packed) -- Unpacks back to numbers

-- tostring() turns the result into a string
local math = math.random(1,999)
print(tostring(math))

-- string.find() searches for a pattern in a string and returns its position, string:gsub() replaces pattern matches in a string
local e = 'balls-eeee'
if string.find(e, 'balls') then -- finds the string balls
    e = string.gsub(platform, 'balls-', '') -- replaces balls- with '' (nil)
end
print(e)
```

## Metatables
Metatables allow you to change the behavior of a table by defining special functions that are called when certain operations are performed on the table.
```lua
local table = {}
local metatable = {
    --__index is called when accessing a key that doesn't exist in the table
    __index = function(tbl, key)
        print('yap')
        return 'yap'
    end,
    --__newindex is called when setting a value for a key that doesn't exist
    __newindex = function(tbl, key, value)
        print('yap')
        rawset(tbl, key, value)
    end
}

setmetatable(table, metatable)
print(table.metatable)
```

> [!IMPORTANT]
> For every exploit function: [here](https://github.com/sentinel-lua/exploit-functions/blob/main/main)