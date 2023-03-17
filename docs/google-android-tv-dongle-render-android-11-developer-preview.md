# 这是从 Android 11 DP 上看到的谷歌 Android 电视加密狗

> 原文：<https://www.xda-developers.com/google-android-tv-dongle-render-android-11-developer-preview/>

今天，谷歌[发布了针对](https://www.xda-developers.com/android-11-developer-preview-adt-3-android-tv) [ADT-3](https://www.xda-developers.com/google-android-10-android-tv-adt-3-developer/) 的安卓 11 开发者预览版，这是一款面向运行谷歌安卓电视操作系统的开发者的机顶盒。开发者预览版不包含任何面向用户的变化——毕竟，ADT-3 只面向开发者——但我们仍然通过更新看了一下，看看是否有任何谷歌没有记录的即将推出的 Android TV 特定功能。当我们挖掘固件时，我们发现了与谷歌即将推出的 Android TV 加密狗相关的另一项资产。

本月早些时候，我们收到了代号为“sabrina”的谷歌设备的预发布固件。在该固件中，[我们发现了](https://www.xda-developers.com/google-android-tv-dongle-remote-ui/)一段视频，展示了谷歌 Android TV 加密狗的设计，这是该设备的专用遥控器，以及可能会在该设备上首次亮相的新 Android TV UI。该视频创建于 2019 年 10 月 10 日，比 Pixel 4 上市日期早 5 天。鉴于产品发布的生命周期，自视频制作以来，加密狗的最终设计和规格不太可能有太大变化。然而，由于我们仍然不知道加密狗何时会真正推出，所以谷歌总有可能在过去几个月的任何时间点返回，对设计或内部组件进行调整。

然而，在谷歌 ADT-3 开发者盒子的 Android 11 开发者预览版中，我们在 SetupWraithPrebuiltGtvs 中发现了一个名为“reboot_sabrina”的视频，该系统应用程序处理 Android TV 的设置向导。该视频向用户展示了如何通过从其电源连接器(似乎是 USB 线，尽管我们不知道它是 micro-USB 还是 Type-C)中拔出 3 秒钟来重新启动“Sabrina”Android 电视加密狗。视频显示了该设备的草图，其整体形状为长方形，中间有“G”标志，与我们在预发布固件中看到的加密狗的设计相匹配。

这个视频本身并没有真正告诉我们太多关于谷歌的加密狗，我们还不知道，但它确实证实了我们本月早些时候发表的渲染设计。另外，这是我们第一次在公开来源中看到*任何*与《莎宾娜》相关的东西，尤其是一个*非常*近的东西。但愿，这意味着我们看到《莎宾娜》上映的日子不会太久了。[我们中的一些人迫不及待地想要得到它。需要注意的一点是，这一资产在 Android 11 开发者预览版中的出现并不能保证“sabrina”将与 Android 11 一起开箱即用——我猜测它将与基于 Android 10 的 Android TV 一起推出，但一旦基于 Android 11 的 Android TV 上市，它将是首批体验 Android 11 的 Android TV 的产品之一(这通常发生在新的手机操作系统公开后的几个月)。)](https://www.xda-developers.com/google-android-tv-dongle-long-overdue/)

以下是我们目前所知的谷歌安卓电视加密狗规格的总结。我们根据对预发布固件的分析编辑了这个规格列表，所以不能保证这些规格是准确的。

| 

种类

 | 

规格

 |
| --- | --- |
| **CPU + GPU** | Amlogic S905X2

*   4 个 ARM Cortex-A53 @ 1.8GHz
*   马里-G31 MP2

 |
| **闸板** | 2GB |
| **显示** | HLG、HDR10、杜比视界、自动低延迟模式(ALLM) |
| **连通性** | Broadcom BCM 43569(Wi-Fi 802.11 AC+蓝牙 4.1) |
| **音频** | Cadence 的 Tensilica HiFi 4 DSP |
| **远程** | 是的，谷歌助手的麦克风 |

这里有一个发布在我们 YouTube 频道上的视频，展示了谷歌 Android TV 加密狗的设计及其远程和新的 Android TV UI。

* * *

*感谢 PNF 软件为我们提供了使用 [JEB Decompiler](https://www.pnfsoftware.com/?aid=xdadev) 的许可，这是一款针对 Android 应用的专业级逆向工程工具。*