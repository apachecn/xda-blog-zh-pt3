# Wine 8.0 发布了更好的控制器兼容性、实验性 WoW64 支持等等

> 原文：<https://www.xda-developers.com/wine-80-released/>

如果你想在 Linux 上运行 Windows 应用程序，那么你可能听说过 Wine。Wine 作为一个层，将 Windows API 调用转换为 POSIX(可移植操作系统接口)调用，同时重新创建 Windows 目录结构，并提供系统服务的替代实现。它也不使用任何仿真或虚拟化来执行 Windows 二进制文件。现在，Wine 版本刚刚发布，进行了大量的改进和更改。

最显著的变化之一是完成了可移植可执行文件(PE)转换，即 Windows 二进制格式。这很重要，因为这意味着检查系统模块的磁盘和内存内容是否相同的各种复制保护方案现在将信任它们运行的系统。Wine 开发者表示，这将允许“64 位主机上的 32 位应用程序、Windows 调试器、ARM 上的 x86 应用程序”等等。

此外，wow 64(**W**windows 32 位**o**n**W**windows**64**位)支持已经为“几乎所有”Unix 库实现。这允许在 64 位环境中执行 32 位应用程序，而不需要适当的 32 位库。Wind 开发人员还不建议将其用于一般用途，但可以通过使用'- enable-archs '选项来启用它。

其他改进包括:

*   默认配置下启用新灯光主题
*   许多 Direct3D 优化和改进
*   控制器热插拔支持得到改进
*   驱动轮检测
*   使用 hidraw 后端时，支持索尼 DualShock 和 DualSense 控制器
*   Windows 运行时(WinRT)模块。游戏。输入已经被引入，一个访问游戏手柄、操纵杆和驱动轮的编程接口
*   Wine Gecko 获得可访问性支持

请务必查看葡萄酒 8.0 官方公告，了解更多信息。虽然二进制文件还不能下载，但是您可以自己构建或者等待这些二进制文件发布。一旦完成，你就可以在 Ubuntu、Debian、Fedora 和 macOS 上安装它了。葡萄酒构成了[蒸汽甲板](https://www.xda-developers.com/steam-deck-review)的[质子](https://www.xda-developers.com/how-proton-on-the-steam-deck-works/)的一部分，因此其中一些改进可能会在未来使蒸汽甲板上的游戏变得更好。

* * *

**来源:** [酒](https://www.winehq.org/announce/8.0)