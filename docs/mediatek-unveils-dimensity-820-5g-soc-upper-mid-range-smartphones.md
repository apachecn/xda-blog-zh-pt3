# 联发科天玑 820 推出中端 5G 智能手机

> 原文：<https://www.xda-developers.com/mediatek-unveils-dimensity-820-5g-soc-upper-mid-range-smartphones/>

今天，台湾芯片组制造商联发科推出了联发科天玑 820，扩大了中端 SoC 阵容。Dimensity 820 继承了该公司今年早些时候在 CES 2020 上推出的 [Dimensity 800](https://www.xda-developers.com/mediatek-dimensity-800-5g-chip-mid-range-phones/) (然而它还没有出现在商业手机上)，并且介于旗舰 [Dimensity 1000 系列](https://www.xda-developers.com/mediatek-dimensity-1000-7nm-soc-integrated-5g/)和[专注于游戏的 Helio G90 系列](https://www.xda-developers.com/mediatek-helio-g90-series-hyperengine-game-technology-launched/)之间。新的芯片组带来了更快的 CPU 和 GPU 性能，支持 120Hz 面板和改进的 ISP。

Dimensity 820 基于台积电的 7 纳米 FinFET‌工艺构建，使用与之前的 SoC 相同的 CPU 微体系结构，在一个大的。LITTLE‌安排。联发科在 Dimensity 800 上设置性能核心的时钟速度方面相当保守——特别是考虑到 7 纳米工艺节点的能效。该公司这次的目标是更高的频率，所有四个 [ARM Cortex-A76](https://www.xda-developers.com/arm-cortex-a76-cpu-mali-g76-gpu-mali-v76-vpu-announcement/) 性能核心的时钟频率为 2.6GHz，高于 Dimensity 800 的 2.0GHz 时钟速度。联发科没有详细说明这种提升是否是以效率为代价的，但这种跳跃确实使芯片组在原始 CPU 能力方面比骁龙 765G 有优势。没有改变的是四个 [ARM‌ Cortex-A55 效率核心](https://www.xda-developers.com/arm-unveils-cortex-a75-a55-processors-and-mali-g72-gpu/)，它们运行在相同的 2.0GHz 频率。

| 

社会学

 | 

尺寸 800

 | 

尺寸 820

 | 

骁龙 765 克

 |
| --- | --- | --- | --- |
| 中央处理器 | 4x ARM Cortex-A76 @ 2.0 GHz 4x ARM Cortex-A55 @ 2.0 GHz | 4x ARM Cortex-A76 @ 2.6 GHz 4x ARM Cortex-A55 @ 2.0 GHz | 1 个 Kryo 475(基于 ARM Cortex-A76)主内核@ 2.4GHz1x Kryo 475(基于 ARM Cortex-A76)性能内核@ 2.2GHz6x ARM Cortex-A55 @ 1.8GHz |
| 国家政治保卫局。参见 OGPU | ARM Mali G57(4 个内核) | ARM Mali G57(5 个内核) | 肾上腺素 620 |
| 记忆 | LPDDR4X | LPDDR4X | LPDDR4X |
| NPU/APU | 

*   联发科 APU 3.0
*   高达 2.4 倍的人工智能性能

 | 

*   联发科 APU 3.0
*   高达 2.4 倍的人工智能性能

 | 

*   六角形 696
*   张量加速器
*   六边形向量扩展
*   高达 5.5 TOPS 的 AI 性能(组合 CPU+ GPU+Tensor+HVX)

 |
| 网络服务提供商 | 

*   Imagiq ISP
*   1 个 64MP 或 32MP+16MP

 | 

*   Imagiq 5.0 ISP
*   1 个 80MP
*   四台并行摄像机

 | 

*   Spectra 355 ISP
*   1 个 192 兆像素或 2 个 22 兆像素，带 ZSL

 |
| 编码/解码 | 

H.264，H.265 (HEVC)，VP-9

 | H.264，H.265 (HEVC)，副总裁-9 | H.264，H.265 (HEVC)，VP9 |
| 调制解调器 | 

*   集成 5G 调制解调器
*   5G 低于 6GHz

 |  |  |
| 制作工艺 | TSMC 7 纳米 | TSMC 7 纳米 | 三星 7 纳米 |

在 GPU‌方面，Dimensity 820 采用了 5 核版本的 [ARM Mali-G57 GPU](https://www.xda-developers.com/arm-mali-g57-gpu-launch-valhall-architecture/) ，比 Dimensity 800 的 4 核版本略有改进。为了改善游戏体验，联发科的 [HyerEngine 2.0](https://www.mediatek.com/innovations/hyperengine-game-technology) 也在板上，它提供了一系列基于软件的增强功能，以实现更好的图形性能，包括智能分配 CPU、GPU 和内存、网络延迟优化、呼叫和数据并发、增强的 HDR‌视觉效果等。

新芯片组带来显著升级的另一个领域是支持高刷新率面板。虽然 Dimensity 800 支持高刷新面板，但它只能以 90Hz 的刷新率处理 FHD+显示器。另一方面，Dimensity 820 支持以高达 120Hz 的刷新率驱动 FHD+显示器。此外，SoC 还支持 [MiraVision 显示](https://www.mediatek.com/features/miravision-display/miravision-for-smartphones)增强技术，该技术为原始设备制造商提供各种基于软件的功能，以改善观看体验。这些增强功能包括将低分辨率内容升级到全高清的能力、HDR‌10 重新映射、蓝光过滤器和亮度调光器，以获得更好的夜间阅读体验，以及 ClearMotion 功能，该功能可在支持的显示器上将标准的 24/30fps 内容自动转换为 60 或 120fps。

联发科称之为 Imagiq 5.0 的图像信号处理器(ISP)也有所升级，芯片组现在支持高达 8000 万像素的摄像头传感器，高于 Dimensity 800 上的 6400 万像素摄像头支持，以及四个并发摄像头。Imagiq 5.0 还承诺动作相机级电子图像稳定(EIS)、多帧 4K HDR‌视频录制、实时视频散景和改进的降噪功能。

就像 Dimensity 产品组合中的其他 SOC 一样，联发科天玑 820 也具有集成的 5G 调制解调器，支持独立(SA)和非独立(NSA)6 GHz 以下网络。该调制解调器支持 5G 载波聚合、双 SIM 待机、动态频谱共享(DSS)和两种 SIM 上的新无线电语音(VoNR)。

在发布会上，小米[站在舞台上](https://twitter.com/bryanbma/status/1262274469042647041?s=19)，宣布 [Redmi 10X](https://www.xda-developers.com/upcoming-redmi-5g-phone-oled-display-triple-cameras-tenaa/) 将是首批搭载联发科天玑 820 SoC 的手机之一。