# Debug

## Get Registry
```lua
table debug.getregistry(<none>)
```
Returns the registry table.

## Set Metatable
```lua
void debug.setmetatable(Variant object, table mt)
```
Sets the metatable for the given object to the given table. (mt can be nil)

## Getfenv
```lua
table debug.getfenv(Variant object)
```

## Setfenv
```lua
Variant debug.setfenv(Variant object, table env)
```
Sets the environment of the given object, returns object.

## Get Metatable
```lua
table debug.getmetatable(Variant object)
```
Returns the metatable of given object. (functions exactly like getrawmetatable)

## Get Local
```lua
variant debug.getlocal(int stackIndex, string localName)
```
Returns the value of a local from the selected stack based on the name.

## Get Locals
```lua
table<variant> debug.getlocals(int stackLevel)
```
Returns a table of all locals from the selected stack.

## Set Local
```lua
variant debug.setlocal(int stackIndex, string localName, Variant value)
```
Sets the value of a local from the selected stack based on the name. Returns boolean "true" on success.

## Getupvalue
```lua
variant debug.getupvalue(Variant<int, function> container, string upvalName)
```
Returns the value of a upvalue from the selected container based on the name.

## Get Upvalues
```lua
table<variant> debug.getupvalues(Variant<int, function> container)
```
Returns a table of all upvalues from the selected container.

## Set Upvalue
```lua
variant debug.setupvalue(Variant<int, function> container, string upvalName, Variant value)
```
Sets the value of the upvalue from the selected container based on the name. Returns boolean based on whether the upvalue was set successfully or not.

## Get Constants
```lua
table<variant> debug.getconstants(Variant<int, function> f)
```
Return's the constants of the given function. Function must be a lua function.

## Set Constant
```lua
void debug.setconstant(function f, int index, variant val)
```
Set's the constant at the given index for the given function. Index's are 1-based. Function must be a lua function.

## Upvalue ID
```lua
userdata debug.upvalueid(function f, int n)
```
Returns an unique identifier (as a light userdata) for the upvalue numbered n from the given function. These unique identifiers allow a program to check whether different closures share upvalues. Lua closures that share an upvalue (that is, that access a same external local variable) will return identical ids for those upvalue indices.

## Upvalue Join
```lua
void debug.upvaluejoin(function f1, int n1, function f2, int n2)
```
Make the n1-th upvalue of the Lua closure f1 refer to the n2-th upvalue of the Lua closure f2.

## Upvalue Name
```lua
string debug.upvaluename(function f, int n)
```
Returns the name for the upvalue numbered n from the given function. Will return an empty string on C closures.