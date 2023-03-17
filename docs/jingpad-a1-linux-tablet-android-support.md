# JingPad A1 是一款运行 Android 应用程序的 Linux 平板电脑

> 原文：<https://www.xda-developers.com/jingpad-a1-linux-tablet-android-support/>

已经有很多人试图创造运行 Linux 的平板电脑，甚至有几款搭载 ARM 处理器，比如 [Pine64 PineTab](https://www.pine64.org/pinetab/) 。然而，另一家公司现在正在尝试，推出了一款看起来非常像苹果 iPad 的 ARM Linux 平板电脑。它被称为“JingPad”，至少从表面上看，它似乎可以成为任何对平板电脑上的 Linux 感兴趣的人的一个很好的设备。

京垫[目前可在 Indiegogo](https://www.indiegogo.com/projects/jingpad-world-s-first-consumer-level-linux-tablet) 预购，但不要让它作为众筹项目的地位吓跑了你——制造商已经向一些技术评论者和新闻媒体发出了预生产单元。早期的视频展示了这款平板电脑的广告效果，尽管还有一些软件问题仍在解决中。

| 

规格

 | 

京帕德

 |
| --- | --- |
| **尺寸&重量** | 

*   178 x 243.5 x 6.7 毫米
*   “小于 500 克”

 |
| **显示** | 

*   11 英寸 4:3 AMOLED
*   2368 x 1728，266 ppi
*   90%的屏幕与机身比例

 |
| **SoC** | 

*   优索虎 T7510
*   4x Cortex-A75 @ 2.0GHz
*   4x Cortex-A55 @ 1.8GHz

 |
| **闸板&存放** | 

*   8GB LPDDR4 RAM
*   256GB UMCP
*   MicroSD 支持

 |
| **电池&充电** | 

*   8000 毫安时电池
*   18W 有线充电

 |
| **安全** | 指纹传感器 |
| **后置摄像头** | 带闪光灯的 1600 万像素摄像头 |
| **前置摄像头** | 800 万像素摄像头 |
| **端口** | USB 类型-C |
| **音频** | 

*   底部发射扬声器
*   没有耳机插孔

 |
| **连通性** | 

*   2.4/5GHz 双频 Wi-Fi
*   2x2 MIMO
*   蓝牙 5.0
*   GPS/Glonass/伽利略/北斗

 |
| **软件** | 金戈斯 |
| **其他特性** | 

*   支持 4096 压力等级的京垫铅笔
*   支持京板键盘

 |

这款平板电脑由 Unisoc Tiger T7510 驱动，这当然不是骁龙的旗舰芯片，但显然仍然能够提供良好的性能和电池寿命。JingPad 的制造商 Jingling Tech 声称，在需要充电之前，成品平板电脑的电池电量可持续 8-10 小时。该芯片组也能够支持 LTE 和 5G(去年在[海信 F50 5G](https://www.gsmarena.com/the_hisense_f50_5g_will_use_a_new_5g_modem_developed_by_a_company_in_china_no_not_huawei-news-42676.php) 中使用了该芯片组)，但似乎 Jingling 不包括所需的调制解调器，大概是为了降低成本。

鉴于平板电脑和铅笔的预计零售价为 700 美元(尽管 Indiegogo 的定价为 549 美元)，其余的规格令人印象深刻。你得到了一个 2368x1729 AMOLED 屏幕，Type-C 连接，8GB 内存，256GB 内部存储(加上一个 microSD 卡插槽)，一个指纹传感器和一个 8,000mAh 电池，带 18W 有线充电。

叮当科技有自己的平板电脑 Linux 发行版，名为 JingOS，也可以在普通电脑上使用。据[的 GitHub 库](https://github.com/JingOS-team/JingOS)称，该操作系统基于 Ubuntu 20.04 和 KDE 桌面，上面有几个定制应用。精灵已经创建了自己的[窗口管理器](https://github.com/JingOS-team/jing-kwin)、[应用启动器、](https://github.com/JingOS-team/jing-plasma-phone-components)、[视频播放器](https://github.com/JingOS-team/jing-haruna)、[录音机](https://github.com/JingOS-team/jing-krecorder)、[时钟](https://github.com/JingOS-team/jing-kclock)等应用。还有一个专门针对 JingOS 的应用商店正在开发中，但你也可以从 Ubuntu 的 ARM 软件仓库安装软件。

这里的主要问题是 JingOS 不使用主线 Linux 内核 SoC 需要专有的驱动程序。这也意味着，如果不做修改，其他 ARM Linux 发行版将无法在平板电脑上运行。

也许最有趣的软件功能是 Android 应用支持，我们被告知目前由旧版本的 [WayDroid](https://www.xda-developers.com/waydroid-android-apps-on-linux/) 支持。Android 应用程序还不能访问互联网，通知也不能到达，但这仍在努力中。上面的视频展示了 WPS Office、水果忍者和其他在 Android 环境下运行的应用程序。

对于主要对 Linux 感兴趣的人来说，JingPad 最终可能成为一款出色的平板电脑，但只有时间才能证明最终产品的表现如何。Jingling 计划下个月开始大规模生产，Indiegogo 支持者的预计发货日期目前定在 10 月。