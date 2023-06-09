# 联想智能显示器现在可以解锁引导程序，运行 Android 应用程序

> 原文：<https://www.xda-developers.com/lenovo-smart-display-bootloader-unlock-android-apps/>

谷歌试图让 Android Things——一个面向物联网(IoT)设备的高度精简的、基于 Android 的操作系统——起飞的努力一直不太成功。也就是说，有一件事它非常擅长:启动谷歌助手支持的智能扬声器和显示器。然而，从改装的角度来看，这些设备远不如普通的 Android 智能手机和平板电脑。但这是 XDA，我们尽量不歧视。

如果你碰巧有一个旧的联想智能显示器，那么有一个好消息要告诉你。多亏了肖恩·霍伊特的工作，又名 XDA 公认的开发者 [deadman96385](https://forum.xda-developers.com/m/deadman96385.4222965/) ，你不仅可以解锁这款设备的引导加载程序，还可以在上面运行常规的 Android 应用程序！

到目前为止，支持以下联想智能显示器变体:

*   7 英寸版本(型号 **CD-17302F** ，代号“Ivy”)
*   8 英寸版本(型号 **SD-8501F** ，代号“琥珀”)
*   10 英寸版本(型号 **SD-X701B** 和 **SD-X501F** ，代号“蓝莓”)

在联想智能显示屏的第三方开发道路上有几个障碍。首先，设备上的 USB-C 端口隐藏在电源插头周围的硅胶盖下面(对于 7 英寸机型)/右下角(对于 8 英寸和 10 英寸机型)。在暴露 USB-C 端口并将设备连接到 PC 后，您可以使用标准的`fastboot flashing unlock`命令解锁引导加载程序，但绕过 Android 验证的引导保护并不是一项简单的任务。该方法使用一种特殊的解锁工具，要求您将设备引导至引导加载程序模式并执行 CLI 脚本。

如前所述，在联想智能显示器上运行常规 Android 应用程序的工作也在进行中。这是一个有点不规则的过程，因为首先你需要刷新特定于设备的调试固件。此外，由于内部限制，它涉及使用 ADB 安装应用程序和终端命令来运行它们。撇开古怪不谈，这款设备的售后市场发展有一个相当不错的开端。

如果你想玩几个小时，你可以看看下面链接的完整安装指南。我们建议在尝试该程序之前，通读说明书和第一篇文章。

**Bootloader 解锁并在联想智能显示器上运行 Android 应用: [7 英寸机型](https://forum.xda-developers.com/t/cd-17302f-lenovo-smart-display-7-ivy-avb-bootloader-unlock-firmware.4472041/) || [8 英寸和 10 英寸机型](https://forum.xda-developers.com/t/lenovo-smart-display-8-10-amber-blueberry-avb-bootloader-unlock-firmware.4472049/)**

许多人会争论，即使是最狂热的自制者，在这样的外形上运行常规的 Android 应用程序会有多大用处。嗯，这只是以更智能的方式扩展设备生产力的开始。传统智能显示器可能会获得新的生命，而不是被扔进垃圾填埋场，或许在不久的将来，它会被成熟版本的 Android 所补充。

* * *

**来源:** [肖恩·霍伊特在推特上](https://twitter.com/Deadman_Android/status/1550976308536135682)