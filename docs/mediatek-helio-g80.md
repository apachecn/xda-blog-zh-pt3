# 联发科宣布面向移动游戏的 Helio G80 经济型 SoC

> 原文：<https://www.xda-developers.com/mediatek-helio-g80/>

# 联发科发布 Helio G80 芯片，目标是低成本的手机游戏

联发科是一家无晶圆厂芯片设计公司，以其一系列廉价和中档芯片而闻名，它宣布了针对移动游戏的 Helio G80。

随着 Helio G80 的推出，台湾芯片设计公司联发科正在扩大其中端 SOC 产品线。联发科的 Helio 芯片 G 系列旨在为手机游戏提供出色的性能，同时不会大幅提高价格，超出普通消费者的承受能力。Helio G 系列的第一款芯片是 Helio G90/G90T，早在去年 7 月[宣布](https://www.xda-developers.com/mediatek-helio-g90-series-hyperengine-game-technology-launched/)，并在红米 Note 8 Pro 中发货[。上个月，联发科宣布了面向预算游戏设备的](https://www.xda-developers.com/xiaomi-redmi-note-8-pro-review-mid-range-performance-champion/) [Helio G70](https://www.xda-developers.com/mediatek-helio-g70-helio-g70t/) ，Realme 已经确认其即将推出的 [Realme C3](https://www.xda-developers.com/realme-c3-5000mah-battery-launching-india-february-6/) 将采用该芯片。新的 Helio G80 介于 G70 和 G90 之间，尽管就性能而言，它更接近于 G70 而不是 G90。我们希望看到 G80 出现在本月晚些时候在印度上市的廉价游戏智能手机中。

新的 SoC 有一个八核 CPU，由 2 个最大频率为 2.0GHz 的 ARM Cortex-A75 内核和 6 个最大频率为 1.8GHz 的 ARM Cortex-A55 内核组成。GPU 是 ARM 的 Mali-G52，频率为 950MHz，与 Helio G70 相比略有波动。该 SoC 支持高达 8GB 的 LPDDR4X RAM，时钟频率为 1800MHz。与更高端的 Helio G90 不同，Helio G80 不支持存储芯片的 UFS 技术。像 G70 一样，G80 的 ISP 支持 ZSL 的单个 2500 万像素摄像头和 ZSL 的双 1600 万像素摄像头。显示器、调制解调器和连接规格也与 G70 相同。总的来说，Helio G80 是一款 Helio G70，在 Cortex A55 核心的最大 CPU 频率和最大 GPU 频率方面略有提升。当比较联发科 Helio G80 和高通骁龙芯片时，G80 在性能方面最接近骁龙 710。

| 

规格

 | 

联发科 Helio G70

 | 

联发科 Helio G80

 | 

联发科 Helio G90/G90T

 |
| --- | --- | --- | --- |
| 中央处理器 | 2x ARM Cortex A75 @ 2.0 GHz 6x ARM Cortex A55 @ 1.7 GHz 12 纳米制造 | 2x ARM Cortex A75 @ 2.0 GHz 6x ARM Cortex A55 @ 1.8 GHz 12 纳米制造 | 2 个 ARM Cortex A76 @ 2.0 GHz(G90T 上为 2.05GHz 个 ARM Cortex A55 @ 2.0 GHz12nm 纳米制造 |
| 国家政治保卫局。参见 OGPU | ARM Mali-G52 MC2 @ 820MHz | ARM Mali-G52 MC2 @ 950MHz | ARM Mali-G76 3 eemc 4 @ 720 MHz(G90T 为 800MHz) |
| 人工智能 | 没有专用辅助动力装置 | 没有专用辅助动力装置 | 2x 联发科 APU @ 750MHz |
| 记忆 | 1 个 LPDDR3 @ 933 MHz，最高 4GB2x LPDDR4X @ 1800MHz，最高 8GBeMMC 5.1 | 1 个 LPDDR3 @ 933MHz，最高 4GB2x LPDDR4X @ 1800MHz，最高 8GBeMMC 5.1 | 2 个 LPDDR4X @ 2133MHz，最高 10GBUFS 2.1，eMMC 5.1 |
| 照相机 | 25MP @ 30fps16MP+16MP @ 30fps48MP 4 芯@ 17fps | 25MP @ 30fps16MP+16MP @ 30fps48MP 4 芯@ 17fps | 48MP @ 30 fps 24mp+16MP @ 30 fps 64mp @ 22.5 fps |
| 显示 | FHD+ @ 60Hz | FHD+ @ 60Hz | FHD+@ 60Hz(G90T 上的@90Hz) |
| 调制解调器 | 第 7 类，2xCA | 第 7 类，2xCA | Cat-12，3xCA |
| 连通性 | 1x1 802.11ac，蓝牙 5.0，GPS+GLONASS+北斗+伽利略 | 1x1 802.11ac，蓝牙 5.0，GPS+GLONASS+北斗+伽利略 | 1x1 802.11ac，蓝牙 5.0，GPS+GLONASS+北斗+伽利略 |

尽管 Helio G80 缺乏任何专用的人工智能加速器，包括 Helio G90 中的 APU，但联发科表示，该芯片的 ISP 能够实现谷歌镜头中的对象识别、智能相册、场景检测、带背景移除的场景分割、人像模式增强和面部识别等功能。联发科技还表示，该芯片支持该公司的超引擎游戏技术，该技术最初是为 Helio G90 宣布的。其他功能包括唤醒语音(VoW)支持、EIS、滚动快门补偿和惯性导航引擎。