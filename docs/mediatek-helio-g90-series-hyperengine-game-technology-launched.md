# 联发科 Helio G90 系列采用超引擎游戏技术

> 原文：<https://www.xda-developers.com/mediatek-helio-g90-series-hyperengine-game-technology-launched/>

Android 智能手机有各种各样的选项，但当涉及到电话 SOC 时，真正的选项相当有限。移动芯片市场在很大程度上仅限于少数几家公司，即高通、三星、海思和联发科。高通最近发布了[高通骁龙 855 Plus](https://www.xda-developers.com/qualcomm-snapdragon-855-plus/) ，这是他们旗舰 SoC 的升级版，配有超频 CPU 和 GPU，在旗舰领域提供更好的游戏性能。现在，联发科正在借机推出其新的 Helio G 系列芯片组——新的 Helio G90 和 Helio G90T，承诺在预算空间内带来更高的游戏性能；以及联发科超引擎游戏技术。

联发科的命名惯例表明，新的 Helio G90 系列是对其 Helio P90 SoC 的专注于游戏的升级。虽然联发科在新闻稿或公告中没有明确提到这一点，但 Helio G90 似乎与 P90 基于相同的 12 纳米工艺。该 SoC 由 2 个主频为 2.05Ghz 的 Cortex-A76 内核和 6 个 Cortex-A55 内核组成。这是由 [ARM Mali G76](https://developer.arm.com/ip-products/graphics-and-multimedia/mali-gpus/mali-g76-gpu) 3EEMC4 GPU 补充的，这是对 P90 上存在的 IMG PowerVR GM 9446 的明确升级。与联发科产品线中的其他 SoC 相比，这是该 SoC 的一个亮点升级，因为同样的 10 核集群 GPU 也可以在高端芯片上找到，如[麒麟 980](https://www.xda-developers.com/hisilicon-kirin-980-honor-magic-2-huawei-mate-20-pro/) ，尽管 Helio G90 系列上的 Mali G76 配备了 4 核集群。基于 Bifrost 架构的 Mali G76 是 2018 年的，ARM 最新的高级 GPU 是基于 Valhall 架构的[Mali G77](https://developer.arm.com/ip-products/graphics-and-multimedia/mali-gpus/mali-g77-gpu)；但即便如此，这也是一个非常令人兴奋的机会，因为联发科的 SOC 往往瞄准更便宜的设备。在 SoC 上包含一个功能强大的 GPU 将大大增强低成本设备上的游戏体验，使它们成为预算内游戏的更好主题。联发科的目标是直接与高通骁龙 730G 这样的产品竞争，所以我们很高兴看到它如何在中端移动市场取得成功。

G90 系列的其他功能包括高达 10GB 的 LPDDR4X RAM，时钟频率高达 2133MHz。该 SoC 还支持高达 64MP 的单摄像头或 24MP 加 16MP 的双摄像头配置，以及像素宁滨支持和 240fps slo-mo，以及人工智能面部检测。有趣的是，该芯片还集成了双唤醒词支持，允许手机内置同时收听多个触发词的支持。对于网络，该系列支持采用 3X CA 和 4X4 MIMO 技术的 Cat-12 4G LTE 调制解调器。

| 

规范

 | 

联发科 Helio G90

 | 

联发科 Helio G90T

 |
| --- | --- | --- |
| 中央处理器 |  |  |
| 国家政治保卫局。参见 OGPU | ARM Mali-G76 3EEMC4 最高可达 720MHz | ARM Mali-G76 3EEMC4 最高 800MHz |
| 照相机 |  |  |
| 人工智能 | 2 个联发科 APU，高达 750MHz | 2 个联发科 APU，高达 750MHz |
| 语音唤醒 | 单个唤醒字 | 双唤醒字 |
| 记忆 | LPDDR4x 高达 8GB，2133MHz(有效速率为 4，266 GT/s) | LPDDR4x 高达 10GB，2133MHz (4，266 GT/s 有效) |
| 储存；储备 | UFS 2.1；eMMC 5.1 | UFS 2.1；eMMC 5.1 |
| 显示 | 最高可达 2400 x 1080，全高清，21:9 | 最高可达 2400 x 1080，全高清，21:9 |
| 显示刷新率 | 60Hz | 高达 90Hz |
| 调制解调器 | 4G LTE Cat-12(DL)/Cat-13(UL)(FDD/TDD)，4x4 MIMO，3CA，256QAM，HUPE，IMS (VoLTE/ViLTE/WFC)，eMBMS，双 4G VoLTE (DSDS)，全球频段，TAS 2.0 | 4G LTE Cat-12(DL)/Cat-13(UL)(FDD/TDD)，4x4 MIMO，3CA，256QAM，HUPE，IMS (VoLTE/ViLTE/WFC)，eMBMS，双 4G VoLTE (DSDS)，全球频段，TAS 2.0 |

在推出 G90 系列的同时，联发科技还推出了其超引擎游戏技术，该技术采用了一系列引擎来提升移动游戏体验:

*   **联网引擎:**联网引擎具备检测到 WiFi 信号降级，然后触发 WiFi 和 LTE 并发从一个连接无缝切换到另一个连接的能力。
*   **快速反应引擎:**触摸加速，提高游戏内动作显示速度。
*   **资源管理引擎:**智能重定向设备资源，如 CPU 和 GPU，以获得最佳性能。
*   **画质引擎:**支持 HDR10 标准，10 位色深，可在支持 HDR 的智能手机显示屏上呈现生动的视觉效果。
*   **双 WiFi 连接:**允许单个智能手机天线同时连接到两个 WiFi 频段(2.4GHz/5GHz)或两个路由器。这保证了可靠的连接，减少延迟和游戏抖动。
*   **通话和数据并发:**允许数据连接在来电中保持活动状态，因此您可以推迟通话，而不会因为您的非活动连接而被赶出游戏。

* * *

联发科 G90 系列将于“不久的将来”在印度的小米智能手机上首次亮相。鉴于游戏在印度市场有着非常光明的前景，我们预计其他原始设备制造商也会购买这款设备。