# 微软将把 Android 13 带到 Android 的 Windows 子系统中

> 原文：<https://www.xda-developers.com/windows-subsystem-for-android-development-roadmap-android-13/>

在 Windows 11 上，Android 的 Windows 子系统(WSA)是一个平台，让你可以在笔记本电脑或台式机上无缝运行 Android 应用程序以及常规的 Windows 应用程序。微软在 5 月份将 WSA 的底层升级到了 Android 12L。现在 [Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2/) 的第一个功能下降已经到来，Android 子系统正式退出预览，开发团队已经开始关注 [Android 13](https://www.xda-developers.com/android-13/) 的更新。

虽然 WSA 不完全是开源软件，但微软现在已经为社区创建了一个 GitHub 存储库，用于报告问题和提交子系统的新功能请求。除了作为开发者互动的一站式场所，repo 还提供了 Android 的官方开发路线图 Windows 子系统。虽然 Android 13 的到来确实在战略之中，但该公司也计划在不久的将来推出大量新功能。

根据最初的路线图，微软正在开发一个文件传输功能，这将大大简化 Android 容器和 Windows 之间的文件传输过程。当然，你可以[使用 ADB 与当前版本的 WSA 进行交互](https://www.xda-developers.com/how-to-sideload-android-apps-on-windows-11/),但是一个将自身与 Windows 资源管理器集成的图形界面对普通用户来说更好。

本地网络接入是另一个即将实现的功能。这将有望解决 WSA 社区面临的许多与网络相关的障碍。画中画模式也在计划中，这将允许你在原生 Windows 应用之上的一个小矩形空间中运行 Android 应用。

然而，事情远不止如此。微软还列出了其他几个功能，这些功能被高度要求，但目前 Android 的 Windows 子系统还不支持。例如，直接 USB 访问目前既不被允许，也不在未来的路线图中，但该公司继续评估由于普遍需求的潜力。

下面是 Android Windows 子系统的功能可用性表和未来发展路线图:

| 

当前功能

 | 

未来路线图

 |
| :-- | :-- |
| ❌安卓 Widgets✅某些音频 Codecs✅摄像头(前置+ back)✅ ClearKey DRM 或 MPEG-DASH content✅ CTS/VTS❌直接蓝牙接入(以及 BLE)✅ Ethernet❌文件 Backup/restore❌文件 transfer✅自由形式窗口管理✅游戏手柄\00i 硬件 DRM✅位置+ GPS✅麦克风✅多显示器/辅助显示器\00i 画中画✅打印\00i 快速磁贴✅软件 DRM (Widevine L3 支持)\ | ⏩安卓 13⏩文件传输⏩快捷指令⏩画中画⏩默认情况下本地网络访问 |

目前还不清楚这些功能何时会出现在 Windows 11 上，但我们预计它们将与下一个“时刻”功能一起推出。

要在支持的国家/地区更新到最新版本的 Android Windows 子系统，您可以前往 Microsoft Store 的 Library 部分查看更新。然而，如果你已经解决了地区(或更新渠道)限制，你应该可以很好地获得更新。

* * *

**来源:** [安卓 GitHub 回购的 Windows 子系统](https://github.com/microsoft/WSA)