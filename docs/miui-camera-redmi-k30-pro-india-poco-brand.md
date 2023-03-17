# MIUI 相机代码提示 Redmi K30 Pro 可能会在印度推出 POCO

> 原文：<https://www.xda-developers.com/miui-camera-redmi-k30-pro-india-poco-brand/>

小米最初将 [Redmi 剥离为独立品牌](https://www.xda-developers.com/xiaomi-spins-redmi-sub-brand/)，专注于预算领域。然而，由于最近推出了 Redmi K30 Pro(代号“lmi”)和 Redmi K30 Pro Zoom Edition(代号“lmipro”)，他们已经在旗舰细分市场中争夺份额。在中国[正式发布会](https://www.xda-developers.com/xiaomi-redmi-k30-pro-notchless-pop-up-camera-design-snapdragon-865-china-launch/)之前，我们甚至[偶然发现了](https://www.xda-developers.com/xiaomi-redmi-k30-pro-zoom-edition-note-9-10x-4g-names-confirmed-miui-11/)这两部手机的名字。我们现在发现的证据表明，Redmi K30 Pro 将在印度发布，可能以 [POCO 品牌](https://www.xda-developers.com/xiaomi-india-spins-off-poco-independent-brand/)发布。我们仍然不知道它是否一定会被称为 POCO F2，但由于 Redmi K30 Pro 是一款搭载[高通骁龙 865](https://www.xda-developers.com/qualcomm-snapdragon-865-processor-specifications-features/) 的旗舰智能手机，这是一种可能。

*感谢 XDA 初级会员 [kacskrz](https://forum.xda-developers.com/member.php?u=8240900) 在 MIUI 11 代码中首次发现这些提示。他与我们分享了他的发现，我们证实了他发现的所有代码和文件确实存在于最新的 MIUI 相机应用程序中。请注意，MIUI 相机应用程序相当混乱，因此我们将在下面提到的方法名称很可能不是方法的真实名称。*

这一切都是从在最新的 MIUI 11 测试版中反编译最新版本的 MIUI 相机应用开始的。我们发现了一个叫做 *Bi* 的新方法，如果 *b.kb* 和*构建成功，它将返回 true。IS_INTERNATIONAL_BUILD* 返回 true。

深入研究一下 *b.kb* ，我们发现如果模型名匹配“lmi”或“lmin”，它将返回 true

如前所述,“lmi”是 Redmi K30 Pro 的代号。据推测，“lmiin”将是印度版 Redmi K30 Pro 的代号，因为小米设备代号[末尾的“in”往往表示这个](https://www.xda-developers.com/redmi-k20-pro-xiaomi-mi-9t-pro-india-china/)。

方法 *Bi* 在另一个名为*getCustomWatermarkDefault*的方法中被调用，其中由十六进制值 *0x7F1000FF* 标识的字符串也被调用。

*0x7F1000FF* 对应一个名为*device _ poco _ watermark _ default _ text*的常量，其中包含字符串“在 POCO 手机上拍摄”。

因此，这款代号为“lmiin”的设备，我们预计是印度版的 Redmi K30 Pro，预计会显示“在 POCO 手机上拍摄”的水印。这告诉我们，Redmi K30 Pro 在印度销售时可能会有 POCO 品牌。这并不奇怪，因为 Redmi K30 4G 在印度被更名为 POCO X2。我们希望传奇的 POCO F1 ( [评论](https://www.xda-developers.com/xiaomi-poco-f1-design-display-gaming-performance-review/))的真正继任者将采用来自高通的旗舰 SoC，看起来这即将发生。

以下是中国 Redmi K30 Pro 的规格，以防你想知道 POCO F2 的性能:

### Redmi K30 Pro 规格

| 

规格

 | 

Redmi K30 Pro

 |
| --- | --- |
| **尺寸和重量** |  |
| **显示** |  |
| **SoC** | [高通骁龙 865](https://www.xda-developers.com/qualcomm-snapdragon-865-processor-specifications-features/) :

*   1 个 Kryo 585(基于 ARM Cortex-A77)Prime core @ 2.84 GHz
*   3 个 Kryo 585(基于 ARM Cortex-A77)性能内核@ 2.4GHz
*   4 个 Kryo 385(基于 ARM Cortex A55)高效内核@ 1.8GHz

肾上腺素 650 |
| **RAM 和存储器** |  |
| **电池&充电** |  |
| **后置摄像头** | 照片:

*   **主要:** 64MP 索尼 IMX686 传感器，1/1.7 英寸传感器，0.8μm 像素，EIS，OIS
*   **次要:** 5MP，宏
    *   变焦版:8MP，长焦，3 倍光学变焦，30 倍数码变焦，支持 50mm 微距，OIS，EIS，四轴防抖
*   **第三:** 13MP，广角摄像头，123
*   **四元:** 2MP，深度传感器

视频:

*   8K 视频录制(分辨率为 7680 × 4320)

 |
| **前置摄像头** | 2000 万 |
| **其他特征** |  |
| **安卓版本** | 基于 Android 10 的 MIUI 11 |

* * *

*感谢 PNF 软件为我们提供了使用 [JEB Decompiler](https://www.pnfsoftware.com/?aid=xdadev) 的许可，这是一款针对 Android 应用的专业级逆向工程工具。*