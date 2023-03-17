# 你需要知道的关于高通骁龙 8 代 1 的一切

> 原文：<https://www.xda-developers.com/qualcomm-snapdragon-8-gen-1/>

高通的骁龙芯片组遍布安卓世界的各个领域，为数百万设备提供动力。今年标志着公司命名策略的改变，不仅骁龙品牌从“高通”中分离出来，而且芯片组本身的命名方式也发生了变化。今年，该公司推出了一款智能手机芯片组，它既不叫骁龙 895，也不叫骁龙 898。这是骁龙 8 Gen 1，将在 2022 年的几款热门旗舰中看到的芯片。

每年，高通都喜欢吹嘘其在效率和性能方面的改进，今年也不例外。随着高通和联发科之间的竞争开始升温(谷歌和三星也有点)，高通似乎感受到了压力。今年的芯片组比去年有了大量的改进，高通承诺在人工智能和图形渲染方面取得巨大进展。高通表示，骁龙 8 Gen 1 显示的变化“远远超过”该公司此前显示的同比变化。

**[对标高通骁龙 8 Gen 1:为 2022 年的旗舰车型设定性能预期](https://www.xda-developers.com/qualcomm-snapdragon-8-gen-1-benchmarks/)**

### 高通骁龙 8 代 1 全规格

## 高通骁龙 8 代 1:完整规格

|  | 

高通骁龙 8 代 1 (sm8450)

 |
| --- | --- |
| **CPU** | 

*   1x Kryo(基于 ARM Cortex-X2)Prime core @ 2.995 GHz，1MB L2 高速缓存
*   3 个 Kryo(基于 ARM Cortex A710)性能内核@ 2.5GHz
*   4 个 Kryo(基于 ARM Cortex A510)高效内核@ 1.79GHz
*   手臂皮层 v9
*   6MB 三级高速缓存
*   **性能提升 20%**
*   **能效提高 30%**

 |
| **GPU** | 

*   新肾上腺素
*   Vulkan 1.1 ( **比 Vulkan** 快 60%)
*   骁龙精英博彩
*   肾上腺素框架运动引擎
*   视频播放:H.264 (AVC)，H.265 (HEVC)，VP8，VP9，4K HDR10，HLG，HDR10+，杜比视界
*   **图形渲染速度提高 30%**
*   **能效提高 25%**

 |
| **显示** | 

*   最大设备显示支持:4K @ 60Hz/QHD+ @ 144Hz
*   最大外部显示器支持:4K @ 60Hz
*   HDR 支持
*   USB Type-C 支持上的显示端口

 |
| **艾** | 

*   具有六边形矢量扩展、六边形张量加速器和六边形标量加速器的六边形 DSP
*   第七代人工智能引擎
*   第三代高通传感中心
*   拥抱脸自然语言处理
*   徕卡的莱茨外观模式
*   **AI 性能提升 400%**
*   **张量加速器性能快 100%**
*   **能效提高 70%**

 |
| **记忆** | LPDDR5 @ 3200MHz，16GB |
| **ISP** | 

*   三路 18 位 Spectra 680 ISP
*   单摄像头:最高 108MP，ZSL @ 30 FPS；高达 200 兆像素
*   双摄像头:高达 64+36MP，ZSL @ 30 FPS
*   三摄像头:最高 3600 万像素，ZSL 每秒 30 帧
*   视频拍摄:8K HDR @ 30 fps；慢动作高达 720p @ 960 fpsHDR10、HDR10+、HLG、杜比视界

 |
| **调制解调器** | 

*   骁龙 X65 5G 调制解调器
*   下行链路:10Gbps
*   模式:NSA、SA、TDD、FDD
*   毫米波:1000MHz 带宽，8 个载波，2x2 MIMO
*   低于 6 GHz: 300MHz 带宽，4x4 MIMO

 |
| **充电** | 高通快速充电 5 |
| **连通性** | 位置:北斗、伽利略、GLONASS、GPS、QZSS、[双频 GNSS 支持](https://www.xda-developers.com/dual-frequency-gnss-important-location-feature-your-phone-probably-missing/) Wi-Fi:高通 FastConnect 6900Wi-Fi 6E，Wi-Fi 6；2.4/5GHz/6GHz 频段；20/40/80/160 兆赫频道；DBS (2x2 + 2x2)、TWT、WPA3、8×8 MU-MIMOBluetooth:版本 5.2、aptX 语音、aptX 无损、aptX 自适应和 LE 音频 |
| **制造工艺** | 4 纳米 |

* * *

## 骁龙 8 代 1 CPU:新 Kryo

ARM 于今年 3 月推出了 ARMv9 架构，该公司表示，预计未来十年将有超过 3000 亿颗芯片使用该架构。ARM ISA 的最后一次重大修订是 v8，于 2011 年 10 月推出，采用 64 位 AArch64 指令集。然而，ARM 多年来一直在扩展 ARMv8，在 ARMv8.5 中添加了内存标记等新功能。对于 ARMv9，该公司继续使用 AArch64 作为基准指令集，但扩展了旨在提高安全性和性能的新功能。据 ARM 称，ARMv9-A 架构的主要新特性如下:

*   **SVE2** :将可扩展向量的优势扩展到更多的用例
*   **领域管理扩展(RME):** 将 Arm 平台上的机密计算扩展到所有开发人员。
*   **BRBE** :提供剖析信息，如汽车 FDO
*   **嵌入式跟踪扩展(ETE)** 和**跟踪缓冲扩展(TRBE)**:arm v9 的增强跟踪功能
*   TME:Arm 架构的硬件事务内存支持

骁龙的新 Kryo 内核基于 ARMv9 架构。使用新技术的第一批 CPU 设计是 Cortex-X2、Cortex-A710 和 Cortex-A510，这些正是构成高通 Kryo 芯片基础的 CPU 设计。其单个 Cortex-X2 内核、三个 Cortex-A710 内核和四个 Cortex-A510 内核的配置类似于骁龙 888 的布局，后者也有类似的配置。这一次，骁龙 8 Gen 1 采用 4 纳米工艺制造(预计将是三星代工的 4 纳米工艺)。

Prime core 的主频为 2.995GHz，高通曾经达到的峰值速度是在[中期骁龙 865 加刷新](https://www.xda-developers.com/qualcomm-snapdragon-865-plus-launch/)时的 3.1GHz。搭载 Cortex-X1 的[中期骁龙 888 Plus refresh](https://www.xda-developers.com/qualcomm-snapdragon-888-plus/) 也达到了 2.995GHz。苹果 A15 性能核心主频 3.2GHz，供参考。

三个 Kryo 性能核心采用 [ARM 的 Cortex-A710 设计](https://www.xda-developers.com/armv9-cpu-designs-cortex-x2-performance-gains/)。Cortex-A710 承诺比其前身 A78 的效率提高 30%，性能提升 10%。Cortex-A710 内核的主频为 2.5GHz。至于三个 Kryo 效率内核，它们基于新的 Cortex-A510 设计。去年对骁龙 888 的效率核心的主要批评围绕着使用老化的 Cortex-A55 核心，所以现在我们应该看到今年的效率有了很大的提高。Cortex-A510 的性能比 A55 提高了 35%,效率也提高了 20%。这些内核的时钟频率为 1.79GHz。

骁龙 8 Gen 1 比骁龙 888 有一些相当大的改进，该公司宣传一些相当大的效率改进是有道理的。还有待观察的是，这些改进在现实世界中是否真的明显。高通表示，总体而言，今年的芯片组比骁龙 888 的功能强 20%，能效高 30%。

* * *

## 骁龙 8 代 1 GPU:新 Adreno

谈到 Android GPU 的性能，高通遥遥领先。谷歌 Pixel 6 的 Mali GPU 将会给高通带来一场竞争，但问题是谷歌的强大无法维持这种峰值性能很长时间。即便如此，高通似乎也感到了一点压力，因为该公司宣布了对其 Adreno 系列 GPU 的一些重大改进。首先，这款新的 Adreno 比骁龙 888 中的 Adreno 660 性能提高了 30%，能效也提高了 25%。

然而，高通也引入了许多其他的改进，不仅仅是数字处理能力。Vulkan 渲染据说获得了 60%的速度提升，并且有一大堆新的骁龙精英游戏功能。可悲的是，似乎没有 AV1 解码支持，尽管像 YouTube 和网飞这样的公司开始推动它。

### 骁龙精英博彩

高通说手机游戏玩家想在骁龙上玩。新的 Adreno GPU 标志着 Adreno Frame Motion Engine 的引入，它允许游戏在不使用更多功率的情况下以两倍的帧率运行，或者使用一半的功率并保持相同的帧率。还有其他改进，包括可变速率着色专业，允许更显着的权力和性能的节省。所有这些都有助于骁龙精英游戏的下一次迭代，根据高通的说法，该游戏在体积渲染方面具有“桌面级能力”。体积渲染包括图形，如雾和烟。

骁龙 8 Gen 1 还首次引入了 Audiokinetic 技术，带来更加身临其境的声音。高通还表示，它正在与无数游戏行业的合作伙伴合作，以便专门针对骁龙芯片优化 Android 上的游戏。

* * *

## 骁龙 8 代第 1 代连接:集成骁龙 X65 调制解调器-RF 系统和 FastConnect 6900

骁龙 8 Gen 1 有一个集成的[高通骁龙 X65 调制解调器](https://www.xda-developers.com/qualcomm-unveils-snapdragon-x65-x62-5g-modem-products/)，这是今年早些时候宣布的 X60 的继任者。这种特殊的调制解调器可以在独立和非独立的 5G 网络上实现 10 千兆位的速度，这是有史以来第一个达到这些速度的调制解调器-RF 系统，去年的 X60 最高可达 7.5Gbps。骁龙 X65 也是第一个支持 [3GPP 的 5G NR release 16](https://www.3gpp.org/release-16) 的调制解调器，这是旨在促进 5G NR 在全球范围内的扩展和部署的第二套规范。

该调制解调器采用 4 纳米工艺制造，支持所有低于 6GHz 和毫米波频段之间的同步载波聚合。骁龙 X65 还具有可升级的架构，使得通过软件更新快速推出 3GPP 第 16 版中提出的新功能成为可能。更小的制造工艺应该有望全面节省电力，尽管这显然还有待观察。

就像它在 2008 年首次亮相的高通骁龙 865 Plus 和骁龙 888 一样，骁龙 8 Gen 1 采用了用于 Wi-Fi 和蓝牙的[高通 FastConnect 6900](https://www.xda-developers.com/qualcomm-fastconnect-6900-fastconnect-6700-wifi-6e-bluetooth-5-2-high-end-android-devices/) 系统。它具有 Wi-Fi 6E、蓝牙 5.2、4K QAM、160MHz 频道和 4 流 DBS。高通说，你甚至可以第一次通过蓝牙传输无损的 CD 音频。

* * *

## 骁龙 8 代 1 ISP: Spectra 680 和骁龙瞄准器

高通近年来的一些最大进步可以说是在 Spectra ISP 方面。在过去，我们看到 [Spectra 280](https://www.xda-developers.com/qualcomm-second-gen-spectra-isp-massive-improvements-smartphone-photography/) ISP 带来了对 10 位色深 HDR 视频捕捉的支持，然后骁龙 855 中的 [Spectra 380](https://www.xda-developers.com/qualcomm-spectra-380-isp-integrated-ai/) ISP 是世界上第一个 CV-ISP。之后，我们看到 Spectra 480 ISP 拥有令人印象深刻的 2 千兆像素/秒处理速度，Spectra 580 ISP 也带来了相当多的重大飞跃，包括新的三 ISP 架构、35%的速度提升、对交错 HDR 传感器的支持等等。现在它变得更好了，因为 Spectra 680 将所有这些新功能都投入了使用。

就背景而言，三重 ISP 是一件大事。它允许最多三个相机同时处于活动状态，这对于在相机应用程序中流畅地切换相机非常有用。iPhones 没有遇到的 Android 智能手机中著名的相机延迟是由于每个相机都只是单独运行，而不是一起无缝切换。骁龙 888 改变了这种情况，高通在这方面加倍努力。它的内存带宽增加到了 3.2 千兆像素/秒，允许以每秒 30 帧的速度录制 108 兆像素的图像。或者，它可以在 8K HDR 下拍摄，同时拍摄 64MP 照片，或者以 30 FPS 的速度同时为三个 36MP 相机供电。这是一个强大的 ISP。

Spectra 680 明显快于去年的 Spectra 580。它更高的带宽也允许许多其他用途，包括在一秒钟内捕捉 240 张 12MP 照片。该公司还使用其新的超宽引擎来防止照片边缘扭曲，其中包括色差校正，也称为彩色边缘。这是物体周围颜色失真的地方，有时超宽相机会出现问题。

高通还致力于极端变焦的视频超分辨率，据说它提供了“非常好的细节”，消除了“数字变焦的坏缺点”。最后，由于第三代高通传感中心，ISP 支持一个永远在线的前置摄像头，可以更快地进行面部解锁。高通还表示，这可以用于隐私保护，包括如果别人看到你的手机就锁定它，或者如果有人越过你的肩膀偷看就隐藏通知内容。

至于骁龙瞄准镜，这只是该公司对其整个相机功能集的称呼。除此之外，似乎没有什么真正的变化。

* * *

## 骁龙 8 Gen 1:人工智能与机器学习

虽然高通在 Android 世界的单核性能和 GPU 性能方面经常领先，但在人工智能性能方面，竞争对手肯定已经迎头赶上。谷歌 Pixel 6 Pro 在人工智能方面无需介绍，华为的海思麒麟芯片组提供了出色的人工智能性能。然而，高通仍然提供了出色的人工智能性能，其永不停机系统的功耗不到 1mA。骁龙芯片组上没有专用的神经处理单元，或 NPU。相反，它的“AI 引擎”[包含 CPU、GPU 和 DSP](https://www.xda-developers.com/qualcomm-gary-brotman-ziad-asghar-ai-snapdragon-855-hexagon-690-dsp/) 。骁龙 855 引入了一个[张量加速器](https://www.xda-developers.com/qualcomm-snapdragon-855-performance-gaming-ai-improvements-explained/)，骁龙 865 带来了[实时翻译设备](https://www.xda-developers.com/qualcomm-snapdragon-865-ai-performance-machine-learning-analysis/)。骁龙 888 推出了第二代传感中枢，同时每秒运算量大幅增加。

据称，由于该公司的第七代人工智能引擎，骁龙 8 Gen 1 的人工智能性能提高了 4 倍。与前代产品相比，它的张量加速器性能快两倍，共享内存大两倍，能效高 1.7 倍。所有这些都为骁龙 888 带来了更好的人工智能体验。

### 第三代高通传感中心

第三代高通传感中枢采用了全新的低功耗人工智能系统。它拥有由[拥抱脸](https://huggingface.co/)、探测器和徕卡驱动的附加功能，同时还提供了骁龙历史上最好的张量加速器性能功耗比。徕卡·莱茨的外观模式可以在人工智能中重现徕卡的散景，而由拥抱脸驱动的自然语言处理可以帮助智能地对通知进行分组和优先排序。高通表示，它通过在本地处理你的信息来进行情感分析。最后，Sonde Health 可以通过分析你的声音来监测你的健康状况，高通说，这甚至可以通过训练来识别新冠肺炎症状。

* * *

## 最初的想法

高通表示，由骁龙 8 Gen 1 驱动的第一批设备将很快问世。Realme 已经证实，其 [Realme GT 2 Pro](https://www.xda-developers.com/realme-gt-2-pro-first-phones-launch-snapdragon-8-gen-1-chip) 将是首批发布的产品之一，[小米 12 系列](https://www.xda-developers.com/xiaomi-reveals-the-first-snapdragon-8-powered-smartphone/)也将随之发布。这将成为高通又一个改进的一年，我们将密切关注骁龙 8 Gen 1 与[联发科天玑 9000](https://www.xda-developers.com/mediatek-dimensity-9000-launch/) 和苹果 A15 Bionic 相比表现如何。

高通证实，以下公司将推出基于骁龙 8 代 1 的设备:黑鲨、Honor、iQOO、摩托罗拉、努比亚、一加、OPPO、Realme、Redmi、夏普、索尼公司、Vivo、小米和中兴，商业设备预计将于 2021 年底上市。总而言之，期待看到许多新的旗舰与这一新的旗舰芯片组。