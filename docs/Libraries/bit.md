# Bit

## To Bit
```lua
int bit.tobit(int num)
```
Returns the input as a bit number? (in my testing it just returns the number without a decimal)

## Binary NOT
```lua
int bit.bnot(int num)
```
Performs a bitwise NOT operation on the input.

## Binary AND
```lua
int bit.band(int n1, int n2)
```
Performs a bitwise AND operation on the given inputs.

## Binary OR
```lua
int bit.bor(int n1, int n2)
```
Performs a wise OR operation on the given inputs.

## Binary xor
```lua
int bit.bxor(int n1, int n2)
```
Performs a bitwise XOR operation on the given inputs.

## Binary Left Shift
```lua
int bit.lshift(int num, int ShiftAmount)
```
Shifts the input left by the given amount.

## Binary Right Shift
```lua
int bit.rshift(int num, int ShiftAmount)
```
Shifts the input right by the given amount.

## Arithmetic Right Shift
```lua
int bit.arshift(int num, int ShiftAmount)
```
Performs a arithmetic right shift on the given input by the given amount.

## Binary Rotate Left
```lua
int bit.rol(int num, int ShiftAmount)
```
Circular shifts the input left by the given amount.

## Binary Rotate Right
```lua
int bit.ror(int num, int ShiftAmount)
```
Circular shifts the input right by the given amount.

## Binary Swap
```lua
int bit.bswap(int num)
```
Performs a byte swap on the given input. (basically reverses the bits).

## To Hex
```lua
string bit.tohex(int num)
```
Returns the input as a hexadecimal string.