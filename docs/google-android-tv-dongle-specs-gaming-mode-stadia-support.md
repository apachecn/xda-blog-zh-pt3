# 谷歌的安卓电视加密狗可能有一个 Stadia 的游戏模式

> 原文：<https://www.xda-developers.com/google-android-tv-dongle-specs-gaming-mode-stadia-support/>

本月早些时候，我们公布了从我们获得的谷歌即将推出的代号为“Sabrina”的安卓电视加密狗营销视频中获得的渲染图。我们从预发布固件版本中获得了营销视频。然而，我们最初没有意识到的是，固件也包含了即将到来的硬件特性的证据。

如果你想回顾一下我们目前所知的谷歌安卓电视加密狗的设计和软件体验，那么我推荐你阅读我最初的报道或者观看 XDA TK Bay 的 YouTube 视频。

XDA 认可的开发人员 [deadman96385](https://forum.xda-developers.com/member.php?u=4222965) ，他与我们分享了“Sabrina”的预发布固件版本，通过检查引导映像中包含的“设备树源”(DTS)文件，他发现了一些 Android 电视加密狗的硬件规格。这些文件指定了启动时要启用 SoC 平台的哪些硬件功能。

由于主 DTS 文件非常长(~4，200 行)，如果没有 Android 的 Linux 内核开发知识，很难解析，所以我不会在本文中发布完整的文件。不过，在文件的最顶部，我们可以看到“Sabrina”Android 电视加密狗设备的两个关键细节:它有 2GB 的内存(sml_sabrina_ **2g** ，由 Amlogic S905X2 片上系统供电(下面对 g12a 的引用和下面未显示的对代号“介子”的多次引用证实了这一点)。

Amlogic S905X2 采用 12 纳米制造工艺制造，具有四核 CPU，四个 ARM Cortex-A53 CPU 内核，主频高达 1.8GHz。该 CPU 由 ARM Mali-G31 MP2 GPU 连接。该 SoC 支持 4Kp75 10 位 H.265 内容的视频解码，通过 HDMI 2.1 以高达 4Kp60 的速度输出视频，通过 HDR10、HLG 和杜比视界播放 HDR 视频，等等。

S905X2 是一款非常受安卓电视设备欢迎的 SoC，因此我们看到它支持谷歌的安卓电视加密狗并不奇怪。感谢我们的朋友@ [AndroidTV_Rumor](https://twitter.com/androidtv_rumor) ，这里列出了部分通过 SoC 平台认证的 Android 电视设备:

### 采用 Amlogic S905X2 SoC 的其他 Android 电视设备

| **付费电视提供商/品牌** | **型号** | **年份** | **T21 国家** | **厂家** | **代号** | **SoC** |
| 放大 | Amplia TV | 2020 | 特立尼达&多巴哥 | 阿斯基 | STI6160d327 | Amlogic S905X2 |
| 安泰尔 | 维拉电视台 | 2020 | 乌拉圭 | SDMC | DV8547 | Amlogic S905X2 |
| 运河+波尔斯卡 | 安卓电视解码器 | 2020 年 | 波兰 | 创维 | HY4001 / HY40A | Amlogic S905X2 |
| Digiturk | 无线电视 IP 盒 | 2019 | 土耳其 | SDMC | DV8535 | Amlogic S905X2 |
| 碟形电视 | SmartVU + | 2020 年 | 新西兰 | SDMC | A7070 | Amlogic S905X2 |
| 埃姆卡利 | T49 | 2020 | 哥伦比亚 | 同洲电子 | N9119M | Amlogic S905X2 |
| Mecool | KM3 | 2019 | 中国 | Videostrong | KM3 | Amlogic S905X2 |
| Mecool | KM9 Pro | 2019 | 中国 | Videostrong | KM9PRO | Amlogic S905X2 |
| 米德科 | eSTREAM 4K | 2020 年 | 美国 | SEI 机器人 | T99 | Amlogic S905X2 |
| MINIX | NEO T5 | 2019 | T109 | SDMC | DV8553 | Amlogic S905X2 |
| 跨国公司玩 | 播放框 | 2020 年 | 印度尼西亚 | 创维 | HP40A / CYBORG001 | Amlogic S905X2 |
| Oi | 串流盒 | 2019 | 巴西 | SEI 机器人 | ETRI02 (SEI531O) | Amlogic S905X2 |
| 洛克泰克 | G1 | 2020 年 | 台湾 | 饿了么 | RT-G1 | Amlogic S905X2 |
| SK 宽带 | B 电视智能 3 | 2019 | 韩国 | 富士康 | BFX-AT100 (BFX-UH200) | Amlogic S905X2 |
| TADAAM (Telenet) | TADAAM 盒 | 2020 年 | 比利时 | 阿斯基 | STI6160 | Amlogic S905X2 |
| 变矩器离合器 | T189 | 2020 年 | 乌拉圭 | T195 | T197 | Amlogic S905X2 |
| 阿根廷电信 | 流箱-F1 | 2020 年 | 阿根廷 | 创维 | HP40A2 | Amlogic S905X2 |
| 马来西亚电信 | unifi TV Plus 盒子 | 2020 年 | 马来西亚 | 创维 | HP40A3 | Amlogic S905X2 |
| 印度尼西亚电信公司 | IndiHome | 2020 年 | 印度尼西亚 | 中兴 | B860HV5_Telkom | Amlogic S905X2 |
| 穿越 | Xstream 框 | 2020 年 | 印度尼西亚 | SEI 机器人 | SEI500TR | Amlogic S905X2 |
| 联合集团 | EON 智能盒子(OTT) | 2019 | 塞尔维亚、斯洛文尼亚、黑山、波斯尼亚 | SDMC | SDOTT0202 / DV8519 | Amlogic S905X2 |
| 威达 | 4K 盒子 | 2020 年 | 波兰 | SDMC | DV8519-Vectra | Amlogic S905X2 |
| 威瑞森 | 流媒体电视 | 2019 | 美国 | WNC | JS8V | Amlogic S905X2 |
| 是 | 是+ | 2020 年 | 以色列 | SEI 机器人 | SEI500Y | Amlogic S905X2 |
| 尤凡 | 安卓电视 | 2020 | 荷兰 | SDMC | DV8519 / Amigo7xYUF | Amlogic S905X2 |

DTS 文件中暗示的谷歌 Android 电视加密狗的其他硬件功能包括 Broadcom 的[BCM 43569](https://www.cypress.com/file/310246/download)Wi-Fi/蓝牙组合芯片和 [Cadence 的 Tensilica HiFi 4 DSP](https://www.prnewswire.com/news-releases/cadence-announces-fourth-generation-tensilica-hifi-dsp-architecture-300016314.html) 。

XDA 公认的开发者 deadman96385 还在一个名为“SabrinaService”的预装系统应用中发现了谷歌 Android TV 加密狗的一些其他有趣功能在本申请中提到了“ALLM”，它代表“自动低延迟模式”这是 [HDMI 2.1 规范](https://www.hdmi.org/spec21Sub/AutoLowLatencyMode)的一项功能，允许设备向连接的电视发送信号，使其禁用任何可能增加视频显示延迟的后处理功能。许多电视将这一功能作为“游戏模式”进行营销，因为它对减少游戏时的延迟最有用。明确地说，用户的电视需要有一个低延迟的“游戏模式”才能工作，但 ALLM 的支持意味着谷歌的 Android 电视加密狗将能够自动切换这种模式。

如果这项功能是为了支持谷歌的云游戏流媒体服务 Stadia 而添加的，我不会感到惊讶。我们首先报道了谷歌[计划在 2020 年为 Android TV](https://www.xda-developers.com/stadia-android-tv-android-11-r/) 带来 Stadia 支持，因此谷歌自己的 Android TV 加密狗成为第一个支持该公司自己的云游戏流媒体服务的设备是有意义的。Stadia [的最新更新启用了实验性的 Android 电视支持](https://www.xda-developers.com/google-stadia-mobile-touch-controls-per-device-resolution-support-any-android-device/)，但目前设置过程有点棘手。据我们的朋友@AndroidTV_Rumor 称，现有的 Android 电视机顶盒或加密狗中很少支持自动低延迟模式。不过，索尼 2018 年和飞利浦 2020 年的内置安卓电视支持低延迟游戏模式。

SabrinaService 中另一个有趣的名为“GlobalKeyReceiver”的类暗示遥控器有一个网飞按钮、YouTube 按钮和一个麦克风。

有代码建议在其中一个键上支持长按动作，这可能是为了我们之前发布的遥控器渲染中出现的带星形符号的神秘按钮。

 <picture>![Google Android TV dongle remote](img/f8463139484ce20466eb76ddd801e85d.png)</picture> 

Possible remote

SabrinaService 中的另一个类揭示了专用遥控器可能通过蓝牙连接到设备，这并不奇怪。(下面截图中的 DFU 指的是“设备固件更新”)

我们仍然不知道谷歌的 Android 电视加密狗将于何时推出，也不知道它的定价，但我们肯定对它的上市感到兴奋。消费者安卓电视领域早就应该有更多的竞争，目前由小米和英伟达支撑。

* * *

*感谢 PNF 软件公司为我们提供使用许可 [JEB Decompiler](https://www.pnfsoftware.com/?aid=xdadev) ，这是一款针对 Android 应用的专业级逆向工程工具。*