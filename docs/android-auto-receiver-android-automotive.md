# Android Auto Receiver 可让您在 Android Automotive 主机上运行 Android Auto

> 原文：<https://www.xda-developers.com/android-auto-receiver-android-automotive/>

谷歌车载信息娱乐(IVI)系统的最新版本 Android Automotive 13 已经发布。它为相机子系统、汽车框架、连接性、隐私等带来了多项幕后改进。最近，作为连接性改进的一部分，谷歌[在](https://www.xda-developers.com/android-13-gabeldorsche-bluetooth-stack/) [Android 13](https://www.xda-developers.com/android-13/) 中默认启用了 Gabeldorsche 蓝牙栈。现在，changelog 中的另一个连接改进带来了一个方便的应用程序，名为 Android Auto Receiver。

Android Auto Receiver 是一款适用于 Android Automotive head units 的应用程序，可以让您在 Android Automotive IVI 系统上通过手机运行 Android Auto(通过 Mishaal Rahman)。如果你想知道谷歌为什么提供这样一个应用程序，它的 Play Store 列表表明，它可以在你希望在不设置汽车内置信息娱乐系统的情况下访问你的数据，或者无法访问 Android 汽车主机上的某些应用程序/更新的情况下派上用场。

例如，如果你开着一辆租来的汽车，想要在它的 Android Auto 主机上访问你的数据，你可以从 Play Store 下载 Android Auto Receiver，然后把你手机上的 Android Auto 投影到 IVI 系统上。这是一个非常小众的用例，因为 Android 汽车主机仍然不是主流。但是随着越来越多的汽车制造商采用 Android Automotive ，这款应用可能很快就会流行起来。

至于 Android Automotive 13 changelog 中与 Android Auto Receiver 相关的连接性改进，该版本添加了一个*“API(和一个 CTS 测试)，以将 VendorElements 作为生成的 hostapd AP 配置的一部分。”*正如 Rahman 所解释的，这些变化通过启用几个必需的权限简化了 Android 汽车主机上的 Android Auto projection，包括*“创建虚拟显示设备、保持虚拟显示器始终解锁、与麦克风接口、位置、联系人、通话记录等权限。”*

如果你已经拥有一辆装有 Android 汽车主机的汽车，并想试用 Android Auto Receiver 应用程序，那么有一些坏消息。拉赫曼透露，该应用程序只能安装在*“declare com . goog . android . car . feature . aareceiver”的构建上。*目前这只适用于官方的 Android 汽车操作系统仿真器和带有雷诺 openR link 系统的 IVIs。

* * *

**Via:**斯珀