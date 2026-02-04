# Lucid - An Interactive Hex-Rays Microcode Explorer

Original repository: <https://github.com/gaasedelen/lucid>

Some changes:
* 1. Added a "Copy microcode" item to the right-click menu in the "Microcode Explorer" window (dependency: pyperclip)
* 1. Added a "Set commment" item to the right-click menu in the "Microcode Explorer" window, it works the same as in the disassembly view.
* 3. The original Lucid generated microcode for all maturities in one pass, which is too slow for large functions. It has been changed to use caching and generate microcode on demand.
* 4. Added a "View microcode" item to the right-click menu in the "Disassembly" window.
* 5. When an address range is selected in the "Disassembly" window, the plugin can retrieve microcode for that code range instead of the entire function.

改进点:
* 1. "Microcode Explorer"窗口右键菜单增加"Copy microcode"项(依赖pyperclip)
* 2. "Microcode Explorer"窗口右键菜单增加"Set commment"项, 注释功能同反汇编窗口
* 3. 原版Lucid是一次性生成所有maturity的microcode, 此种方式对于大函数效率太低, 已修改为使用缓存且按需生成 
* 4. "Disassembly"窗口的右键菜单增加"View microcode"项 
* 5. 在"Disassembly"窗口选择了地址范围的情况下, 可以获取这段代码的Microcode而不是整个函数的microcode

