# Welcome
Welcome to the ProtoSmasher Documentation!

## Contributing
If you would like to contribute to the ProtoSmasher documentation, simply open a pull request on GitHub. We only request that you preserve our current style and layout.

## Support
For any support, please contact us at [support@protosmasher.net](mailto:support@protosmasher.net) or message one of our staff or support in our Discord, which can be found on our [website](https://protosmasher.net).

## LuaU
As some may or may not have heard, Roblox has released a new Lua virtual machine known as LuaU. This is a complete rewrite of their old VM, with new opcodes, optimizations, and changes. With these changes, Roblox plans to extend their Lua implementation's capabilities through optimization and the addition of type definitions. This update also strips debug information from scripts' bytecode, meaning ProtoSmasher functions that use this information, such as `getconstants` and the decompiler may be harder to interpret.

With these changes, script execution has been harder to achieve due to discrepancies in our Lua parser and Roblox's. Adapting to these changes may bring about some instabilities in ProtoSmasher, but stability should improve with each update that passes.