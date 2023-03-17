# 华硕 ZenFone 8 Mini 将配备 5.9 英寸 OLED 面板和旗舰处理器

> 原文：<https://www.xda-developers.com/asus-zenfone-8-mini-flip-leak/>

本月早些时候，华硕发布了今年第一款旗舰手机:[ROG 手机 5](https://www.xda-developers.com/asus-rog-phone-5/) 。它比预期的发布时间要早，但是[仍然比去年的 ROG 手机增加了许多改进。不过，ROG Phone 5 并不是华硕在 2021 年推出的唯一一款旗舰手机。我们预计去年 ZenFone 7 的继任者将在今年亮相，我们从内核源代码和固件分析中发现的新细节为华硕 ZenFone 8 系列带来了一些希望。](https://www.xda-developers.com/asus-rog-phone-5-review/)

作为一个背景，我们预计多款手机将作为华硕 ZenFone 8 系列的一部分推出。虽然去年的 ZenFone 7 [在阵容中增加了一款“专业”型号](https://www.xda-developers.com/asus-zenfone-7-pro-review-a-flipping-fantastic-flagship-smartphone/)，但据传继任者[将增加一款“迷你”版本](https://www.xda-developers.com/asus-zenfone-mini-rumor-details/)，该版本将以更紧凑的外形规格为特色。还有神秘的“华硕 Zen fone 8 Flip”[前几天出现在谷歌的一份支持文档](https://www.xda-developers.com/google-leaks-asus-zenfone-8-flip/)中，但我们不知道传闻中的“Mini”和“Flip”实际上是不是一回事。不过，我们可以预计 ZenFone 8 系列中至少会有两款手机，内核源代码和固件文件暗示可能会有第三款。

多亏了来自 XDA 知名开发者 [Freak07](https://forum.xda-developers.com/m/freak07.3428502/) 的提示，我们查看了华硕 ROG 手机 5 的[内核源代码，发现了可能是三款华硕新旗舰手机的参考资料。这三款手机的代号分别是“清酒”、“毕加索”、“伏特加”。作为参考，ZenFone 7 系列的代号为“龙舌兰酒”，而 ROG Phone 3 和 ROG Phone 5 的代号分别为“奥比万”和“阿纳金”。我们还在内核源代码的单个文件中发现了对“SAKE_PLUS”和“VODKA_PLUS”的引用，但是我们不知道这些是否实际上是不同的模型，因为在其他地方没有出现其他引用。](https://www.xda-developers.com/asus-rog-phone-5-bootloader-unlock-tool-kernel-source/)

虽然我们不知道这三款手机中哪一款属于华硕 ZenFone 8 系列，但我们确实在华硕 PixelMaster 相机应用程序的最新版本中明确提到了华硕 ZenFone 8 和华硕 ZenFone 8 Flip。然而，这三款手机都应该基于高通的旗舰产品骁龙 888 移动平台，至少根据内核源代码是这样的。

至少，我们预计“清酒”将是传言中的 ZenFone 8“迷你”，因为它被定义为 5.92 英寸有机发光二极管显示屏，在华硕的软件中被称为“小手机”。面板的配置文件还提到它将支持 120Hz 的刷新率和全高清+ (2400x1080)分辨率。至于相机，我们只发现了两个图像传感器:64MP 的索尼 IMX686 和新的索尼 IMX663。

另一方面，“毕加索”似乎与 ZenFone 7 系列拥有相同的面板:6.67 英寸三星制造的全高清+分辨率 OLED 面板。毕加索也有与 ZenFone 7 系列非常相似的相机硬件，除了一个额外的 24MP 图像传感器，它被奇怪地定义为内核中的“前置”传感器。尽管 ZenFone 的翻盖相机设置很奇怪，但这可能并不意味着它实际上有一个传统的前置摄像头。最后，我们对传闻中的“伏特加”装置一无所知。这是三者中最难以捉摸的，在内核源代码和最新的固件中都很少提到它。

以下是我们了解到的三款手机的信息汇总:

| 

规格

 | 

华硕“清酒”

 | 

华硕“毕加索”

 | 

华硕“伏特加”

 |
| --- | --- | --- | --- |
| **型号名称** | 华硕 _ zs 590 ks/华硕 _I006D | 华硕 _ zs 672 ks/华硕 _I004D | 华硕 _ zs 675 kw/华硕 _I007D |
| **SoC** | 高通骁龙 888 | 高通骁龙 888 | 高通骁龙 888 |
| **显示** | 

*   5.92 英寸 OLED 面板(三星 AMS592YP01)
*   全高清+分辨率(2400x1080)
*   120 赫兹刷新率

 | 

*   6.67 英寸 OLED 面板(三星 AMS667UU07)
*   全高清+分辨率(2400x1080)
*   未知刷新率

 | 未知的 |
| **摄像机** | 

*   索尼 imx 686(6400 万像素图像传感器)
*   索尼 IMX663(新图像传感器？)

 | 

*   索尼 imx 686(6400 万像素图像传感器)
*   索尼 imx 363(1220 万像素图像传感器)
*   Omnivision OV24B1Q (24MP 图像传感器)
*   Omnivision OV08A(用于“远摄”的 800 万像素图像传感器)

 | 未知的 |
| **杂项** | Cirrus CS35L45 放大器 | Pixelworks i6 视觉处理器 | 未知的 |

*感谢 PNF 软件为我们提供了使用**[JEB Decompiler](https://www.pnfsoftware.com/?aid=xdadev)**的许可，这是一款针对 Android 应用的专业级逆向工程工具。*