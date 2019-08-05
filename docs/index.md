# Getting Started
Welcome to the ProtoSmasher Docs!

## Contributing
If you would like to contribute to the ProtoSmasher docs, simply open the github up in the top right and edit what you need to and hit us up with a pull request. Though we please ask you to follow our currently layout.

## Support
For any support, please contact us at support@protosmasher.net or message one of the staff/support in our discord, which can be found on our main website.

## LuaU
As some of you may, or may not have heard, ROBLOX has released a new feature to their custom edition of Lua 5.1 called LuaU. What is it? Well, it's their custom Lua VM, including new opcodes, and further optimization to make Lua faster, as the changes that they made to the already slow Lua VM, had made Lua even slower than it was. Thus with these changes, they are planning to further extend Lua capabilities, by adding type definitions to Lua, to optimize Lua.

Though with these changes it makes it a little bit harder for us ato execute Lua, as the instructions that our Lua parsers generate aren't the same, so we would have to modify our Lua to match theirs, which could make it a bit unstable. Along with the debug information now being stripped from all Lua code that runs inside of LuaU, meaning that some of the functions that use this debug information, like getconstants, or even the decompiler may be harder to understand.

!!! note
    This is a new additional to ROBLOX