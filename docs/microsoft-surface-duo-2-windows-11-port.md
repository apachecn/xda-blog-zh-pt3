# 微软 Surface Duo 2 借助天才开发者之手运行 Windows 11

> 原文：<https://www.xda-developers.com/microsoft-surface-duo-2-windows-11-port/>

高通制造笔记本电脑处理器已经有一段时间了，它是为 Arm 超便携电脑上的永不关机[窗口设计的。但我们几乎不知道，一些售后市场开发商将在 Arm 驱动的设备上获得 Windows 的好处方面领先微软一步。例如，Gustave Monce 又名 XDA 资深成员](https://www.xda-developers.com/best-windows-on-arm/)[gus 33000](https://forum.xda-developers.com/m/gus33000.7651894/),[已经说服 Windows 11 在最初的 Surface Duo](https://www.xda-developers.com/windows-11-dual-boot-on-microsoft-surface-duo/) 上运行，但现在他已经将微软的最新操作系统移植到 Surface Duo 2 上。

在一系列推文和回复中，Monce 展示了 Windows 11 启动到桌面，并在一定程度上运行于微软 Surface Duo 2。不过，值得注意的是，该设备的大多数核心组件都不起作用。虽然显示面板以部分方式运行，但截至目前，操作系统只能识别底层骁龙 888 SoC 的八个核心中的一个。

在第二代 Surface Duo 上引导替代操作系统的基础是在 8 月份奠定的，当时 Gustave 和其他 WOA 项目贡献者在开源 Windows UEFI 固件引导程序项目 SurfaceDuoPkg 中添加了对该设备的初步支持。虽然 Monce 没有分享安装阶段的任何一瞥，但对于任何关心 Android 智能手机或 Windows 或两者兼而有之的人来说，在微软制造的智能手机上运行 Windows 的完整实例的想法是非常有趣的。

**[微软 Surface Duo 2 XDA 论坛](https://forum.xda-developers.com/f/microsoft-surface-duo-2.12449/)**

如果你喜欢冒险，这个端口可以在解锁引导程序后安装在欧洲和美国版本的微软 Surface Duo 2 上。请记住，Windows 11 的内核将在启动期间尝试读取该设备上不支持的寄存器，因此最好在尝试自行安装之前等待额外的补丁，以避免不可预见的错误。不言而喻，这伴随着砖砌你的手机或更糟的风险。

看到操作系统在不适合运行的设备上运行总是很有趣。有些人可能会觉得这很有诗意，因为微软自己也在努力为 Surface Duo 家族发布 Android 12L 在这一点上，这是一项在操作系统推出七个多月后才完成的任务。

* * *

**来源:**[surface duopkg GitHub Repo](https://github.com/WOA-Project/SurfaceDuoPkg/releases/tag/2210.29)， [Gustave Monce 在推特上](https://twitter.com/gus33000/status/1579135965918302208)