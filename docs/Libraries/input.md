# Input

## Left Click
```lua
void Input.LeftClick(int Action)
```
!!! note "Defaults to MOUSE_CLICK if no Action is provided"
Performs a left click of the mouse when called. Use MOUSE_DOWN or MOUSE_UP as Action to do something other than a click.

## Right Click
```lua
void Input.RightClick(int Action)
```
!!! note "Defaults to MOUSE_CLICK if no Action is provided"
Performs a right click of the mouse when called. Use MOUSE_DOWN or MOUSE_UP as Action to do something other than a click. 

## Move Mouse
```lua
void Input.MoveMouse(int x, int y)
```
Moves the mouse from its current position by the given amounts.

## Scroll Mouse
```lua
void Input.ScrollMouse(int ScrollAmount)
```
!!! note "The amount is negative for up, positive for down."
Scrolls the mouse by the given amount.


!!! note "Key Codes"
    Key codes can be found [here](https://msdn.microsoft.com/en-us/library/windows/desktop/dd375731)

## Key Press
```lua
void Input.KeyPress(int VirtualKeyCode)
```
Performs a key press of the given key when called.

## Key Down
```lua
void Input.KeyDown(int VirtualKeyCode)
```
"Holds" a key down when called.

## Key Up
```lua
void Input.KeyUp(int VirtualKeyCode)
```
Releases a key when called.