# 什么是 EdXposed，您可以在 Android 设备上用它做什么？

> 原文：<https://www.xda-developers.com/edxposed/>

[Magisk 模块](https://www.xda-developers.com/best-magisk-modules/)是一种将系统级 mod 应用到设备的简单方法，无需手动更改系统文件。你所要做的就是下载该模块，通过 [Magisk 应用](https://www.xda-developers.com/how-to-install-magisk/)激活它，然后重启你的设备以使更改生效。大多数模块专注于在你的设备上增加一个特性或者改变一件事情，但是有一些模块安装了另一个框架来扩展模块潜力。例如， [Riru](https://www.xda-developers.com/riru/) 是一个 Magisk 模块，它可以挂钩到 [Android Zygote 进程](https://developer.android.com/topic/performance/memory-overview)，并允许开发人员在其上下文中运行代码。

由于 Riru 本质上复制了 Xposed 框架的工作原理，一个高级的 Riru 模块可以在概念上充当通用的 [Android 运行时](https://source.android.com/devices/tech/dalvik) (ART)挂钩平台。**EDX exposed**就是这样一个 Riru 模块。这听起来像是一个过度抽象的例子，但是这实际上是一个通过 Magisk 实现整个 Xposed 框架的新颖想法。简而言之，Riru 本身负责设置 Xposed 风格的环境的所有先决条件，而 EdXposed 为 Xposed 模块的工作提供了一个兼容的 API。

## 什么是 EdXposed？

由 XDA 公认开发者 [mlgmxyysd](https://forum.xda-developers.com/m/mlgmxyysd.8430637/) 和 XDA 成员 [solohsu](https://forum.xda-developers.com/m/5571846/) 共同打造的 EdXposed(简称“老驱动 Xposed”)是 Xposed 框架以 Riru 模块形式的进化。在引擎盖下，它利用了 [SandHook](https://github.com/asLody/SandHook) 和 [YAHFA(又一个艺术用的 Hook 框架)](https://github.com/PAGalaxyLab/YAHFA)项目。该模块自带名为*EDX 曝光管理器*的配套应用，用户可以通过它检查核心的状态，并下载不同的 x 曝光模块。

## EdXposed 有什么特点？

*   完全开源和免费。
*   对各种篡改检测应用的低检测率。
*   如果是软砖，可以轻松关闭。
*   与原始的 Xposed API 兼容。
*   兼容安卓奥利奥 8.0 到安卓 11。

## 如何下载 EdXposed？

你可以从 GitHub repo 下载 EdXposed 的 flash 版本。EdXposed Manager，即配套应用程序托管在下面链接的独立 GitHub repo 上。

**[下载 EDX 曝光](https://github.com/ElderDrivers/EdXposed/releases/latest)|**|**[下载 EDX 曝光管理器](https://github.com/ElderDrivers/EdXposedManager/releases/latest)**

## 如何安装 EdXposed？

在安装 EdXposed 之前，请确保在目标设备上安装了最新版本的 Magisk。请注意，Riru 的最新版本(v26.x)与 EdXposed 不兼容，因此您必须预先安装 Riru v25.x。

1.  从前面提到的 URL 下载 EdXposed ZIP 包。如果您已经在 PC 或 Mac 上下载了它，那么将您的 Android 设备连接到它，并将下载的 ZIP 文件复制到目标设备的内存中。
2.  打开 Magisk 应用程序，使用底部导航菜单切换到*模块*选项卡。
3.  点击名为*从存储器安装*的按钮。接下来，浏览并选择您之前下载的 ZIP 文件。
    *   您也可以从自定义恢复(如 TWRP)中刷新 ZIP 文件。

4.  成功安装后，重新启动您的设备。
    *   如果使用 Magisk 应用程序刷新，该应用程序会自动提示您重新启动。
    *   如果使用 TWRP 刷新，您需要手动导航到 TWRP 电源菜单并选择重新引导至系统选项。

5.  如果你看不到配套的应用程序，或者应用程序提示你安装完整版，那么[侧载](https://www.xda-developers.com/how-to-sideload-install-android-app-apk/)EDX 曝光的管理器 APK(下载链接参见上一节)。
6.  你完了！

## EdXposed 和原始 Xposed 框架之间的比较

遗留 Xposed 框架支持的最后一个 Android 版本是 Android Oreo。此外，最初的 Xposed 安装程序从未被设计为在“无系统”模式下运行。而 EdXposed 则兼容 Android Oreo 到 Android 11。由于对 Riru 的依赖，它可以与 Magisk 协同工作，而无需触及底层系统。

**[曝光 XDA 讨论线索](https://forum.xda-developers.com/t/4070199/)**

不过截至目前，EdXposed 已经不在积极开发中。自 2021 年 2 月以来，无论是管理器应用程序还是实际的代码库都没有提交。当然，你不应该通过提交的频率来判断一个项目的新颖性，但是缺乏开发对于售后改装社区来说肯定是一个红色信号，尤其是在考虑到不断变化的 Android 环境之后。

## 结论

既然你对如何安装和配置 EdXposed 有了更清晰的想法，你的下一步就是[下载一些 Xposed 模块](https://www.xda-developers.com/best-xposed-modules/)并开始摆弄你的 Android 智能手机。当你在设置的时候，也可以看看[最适合 Android 设备的应用](https://www.xda-developers.com/best-android-root-apps/)。