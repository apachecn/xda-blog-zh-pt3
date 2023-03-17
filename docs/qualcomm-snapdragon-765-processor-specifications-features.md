# 高通宣布推出支持 5G 的骁龙 765 和 765G SoCs

> 原文：<https://www.xda-developers.com/qualcomm-snapdragon-765-processor-specifications-features/>

面对来自联发科、华为和三星在价格和规格方面日益激烈的竞争，如印度和中国，高通去年开发了新的骁龙 700 系列中端芯片组。700 系列拥有高通顶级 800 系列的最佳性能，但价格更低。最新版本的骁龙 730 甚至引入了一种游戏变体，以满足移动游戏行业不断增长的需求。现在，高通再一次为 700 系列引入了一个新成员:高通骁龙 765。新的 SoC 为中端价格层带来了对 5G 连接、高刷新率显示和高质量成像的支持。

在印度、中国和亚洲其他地区，小米、Realme、OPPO、华为/Honor、Vivo、联想/摩托罗拉和三星等手机制造商正在竞争，看谁能以最好的价格提供最好的规格。当然，SoC 的成本会影响品牌智能手机的定价，这就是为什么我们会看到许多中端智能手机采用高通最新的 600 系列 SoC 或联发科的 Helio P 系列 SoC。

在这个范围和高端旗舰层之间的是中端设备，如小米 9T、Realme X2、红米 Note 8 Pro、小米 Note 10、Honor 9X 和三星 Galaxy A80。这些设备具有以前只属于旗舰级的功能，例如 3+摄像头、[超高分辨率主摄像头](https://www.xda-developers.com/samsung-isocell-bright-hmx-108mp-camera-sensor-xiaomi/)、6+GB 内存和非常快速的有线充电。凭借高通骁龙 765，明年的中端设备可能具有 120Hz 显示屏、5G 网络支持、12GB 内存、超慢动作视频等功能。以下是骁龙 765 如何做到这一点。

*免责声明:高通赞助我去夏威夷毛伊岛参加骁龙科技峰会。公司支付了我的机票和酒店费用。然而，他们没有对该文章的内容提出任何意见。*

首先，我做了一个表格，比较了[骁龙 730](https://www.xda-developers.com/qualcomm-snapdragon-665-snapdragon-730g/) 和新的高通骁龙 765。如果你还不熟悉大多数术语，这个表格可能很难理解。在表格下方，我提供了所有同比改进和新功能的说明。

|  | 

高通骁龙 730 (sm7150-AA)

 | 

高通骁龙 765 (sm7250-AA)

 |
| --- | --- | --- |
| **CPU** | 2 个 Kryo 470(基于 ARM Cortex-A76)性能内核@ 2.2GHz6x 个 Kryo 470(基于 ARM Cortex-A55)效率内核@ 1.8GHz | 1 个 Kryo 475(基于 ARM Cortex-A76)主内核@ 2.3 GHz(765g 上为 2.4 GHz)1 个 Kryo 475(基于 ARM Cortex-A76)性能内核@ 2.2GHz6x(基于 ARM Cortex-A55)效率内核@ 1.8GHz |
| **GPU** | adre no 618 @ 500 MHz vulkan 1.1 视频播放:H.264 (AVC)、H.265 (HEVC)、VP8、VP9、4K HDR10 PQ、HLG | adre no 620(765G 上 15%速度的 GPU)Vulkan 1.1 视频播放:H.264 (AVC)、H.265 (HEVC)、VP8、VP9、4K HDR10、HLG、HDR10+、杜比 VisionSelect 骁龙精英游戏功能(仅限 765g)性能和效率提高 20% |
| **显示** | 最大设备上显示支持:FHD+@ 120hz 最大外部显示支持:UHD @ 60HzHDR 支持 USB Type-C 上的显示端口支持 | 最大设备上显示支持:FHD+ @ 120Hz，QHD+@ 60hz 最大外部显示支持:UHD @ 60HzHDR 支持 USB Type-C 上的显示端口支持 |
| 【艾】艾 | 具有六边形矢量扩展和六边形张量加速器的六边形 688 第四代人工智能引擎 | Hexagon 696，带 Hexagon 矢量扩展和新 Hexagon 张量加速器第五代人工智能引擎高通传感中心 5.5 TOPS (765G) |
| **记忆** | 类型:2 个 16 位，lpddr 4 速度:最高 1866MHz，8GB RAM | 类型:2 个 16 位，lpddr 4 速度:高达 2133MHz，12GB RAM1MB 系统高速缓存 |
| **ISP** | 双 14 位 Spectra 350 单摄像头:最高 36MP，带 ZSL；最高 192MPDual 摄像头:最高 22MP 带 ZSLVideo 抓拍:4K·HDR @ 30 fps 视频；慢动作高达 720p @ 240 fpsHDR10，HLG | 双 14 位 Spectra 355 单摄像头:最高 36MP，带 ZSL；最高 192MPDual 摄像头:最高 22MP 带 ZSLVideo 抓拍:4K·HDR @ 30 fps 视频；慢动作高达 720p @ 480 fpsHDR10、HDR10+、HLG |
| **调制解调器** | 骁龙 X15 LTE 模式下行链路:800Mbps (4G LTE)上行链路:150Mbps (4G LTE) | 骁龙 X52 4G LTE 和 5G 多模模式下行链路:3.7Gbps (5G)，1.2Gbps (4G LTE)上行链路:1.6Gbps (5G)，210Mbps (4G LTE)模式:NSA，SA，TDD，FDDmmWave: 400MHz 带宽，8 个载波，2x2 MIMOsub-6 GHz: 100MHz 带宽，4x4 MIMO |
| **充电** | 高通快充 4+ | 高通快充 4+高通快充 AI |
| **连通性** | 位置:北斗，伽利略，GLONASS，GPS，QZSS，SBA swi-Fi:Wi-Fi 6；2.4/5GHz 频段；20/40/80 MHz 频道；DBS、TWT、WPA3、8x8 MU-mimobluteooth:版本 5.0、aptX TWS 和自适应 | 位置:北斗，伽利略，GLONASS，GPS，QZSS，SBAS，双频支持 Wi-Fi:高通 FastConnect 6200Wi-Fi 6 就绪；2.4/5GHz 频段；20/40/80 MHz 频道；DBS、TWT、WPA3、8x8 MU-mimobluteooth:版本 5.0、aptX TWS 和自适应 |
| **制造过程** | 三星 8 纳米 LPP | 三星 7 纳米 EUV |

**CPU**

与骁龙 730 相比，骁龙 765 的 CPU 性能略有提高。这是因为 CPU 内核没有任何重大的架构变化。相反，高通增加了一个新的“Prime”CPU 核心集群，由一个主频高达 2.3GHz 的独立核心组成。还有一个主频高达 2.2GHz 的独立“性能”核心。高通表示，这两个核心基于其定制的 Kryo 475 架构，该架构源自 [ARM Cortex-A76 设计](https://www.xda-developers.com/arm-cortex-a76-cpu-mali-g76-gpu-mali-v76-vpu-announcement/)。最后，有 6 个基于 ARM Cortex-A55 的高效 CPU 核心，时钟频率高达 1.8GHz。因此，骁龙 765 的核心集群配置是 1+1+6，而骁龙 730 是 2+6。

从 8 纳米制造工艺过渡到 7 纳米制造工艺可能会在 CPU 能效方面产生一些改进，从而提高平均性能。

**图形处理器**

高通在骁龙 765 中的新 Adreno 620 GPU 据称比骁龙 730 中的 Adreno 618 GPU 提供了 20%的更好的性能和效率。我们不知道 GPU 的最高时钟速度或任何其他可能解释性能和效率提高的细节，但同样，从 8 纳米到 7 纳米制造工艺的过渡很可能在这些方面产生了一些好处。

高通在 Adreno 620 中增加了对 HDR10+和杜比视觉视频播放的支持。相比之下，Adreno 618 仅支持 4K HDR10 PQ。

**显示**

根据高通的说法，新骁龙 765 的最佳功能之一是它支持高达 FHD+分辨率和 120Hz 刷新率的设备显示。GPU 主要负责将像素推送到显示器，随着分辨率和刷新率的提高，有更多的像素要推。

到目前为止，高刷新率面板只出现在高端旗舰智能手机中。然而，Snapdragon 835 驱动的 [Razer 手机](https://forum.xda-developers.com/razer-phone)早在 2017 年就有 120Hz 的显示屏，仅今年我们就看到了近十几款具有高刷新率显示屏的智能手机。第一款中端设备与 one 一起推出只是时间问题[，届时，它很可能由高通骁龙 765 提供动力。有趣的是，高通向我们证实，骁龙 730 中的 GPU 已经能够支持 FHD+ @ 120Hz，但我们不知道骁龙 765 在维持 120fps 方面比骁龙 730 多多少。](https://www.xda-developers.com/redmi-k30-120hz-display-side-mounted-fingerprint-sony-imx686/)

**艾**

高通在设备人工智能方面的进步每年都在新的 Snapdragon 800 系列中得到最好的体现，但该公司也将其中一些进步带到了骁龙 700 系列。高通[通过引入他们的第四代人工智能引擎，在 GPU 中添加更多 alu，改善 CPU 中的点积指令性能，并添加他们的六边形张量加速器(HTA)，将骁龙 730](https://www.xda-developers.com/qualcomm-snapdragon-665-snapdragon-730g/) 的人工智能性能翻了一番。

高通正在继续改善骁龙 700 系列的人工智能性能，推出了第五代人工智能引擎和骁龙 765 中更新的六边形张量加速器。总体而言，骁龙 765G SoC 能够达到 5.5 TOPS(万亿次运算)的性能，接近[骁龙 855 的 7 TOPS](https://www.xda-developers.com/qualcomm-snapdragon-855-performance-gaming-ai-improvements-explained/) 性能。

一个名为“高通传感中心”的独立组件也已经发布。传感中枢旨在对音频进行不间断检测，支持多个热门词汇，如“嘿/好的谷歌”和“Alexa”利用<1 mW of power, the chip’s power drain is basically negligible. As the sensor’s framework is scalable, developers can use Qualcomm’s Hexagon SDKs to create their own audio-activated features.

**ISP**

虽然 Snapdragon 800 系列中的 Spectra ISP 在性能和功能上与这一代产品相比有了巨大的提升，但骁龙 700 系列的改进则较为有限。据我们所知，高通没有透露摄影方面的任何显著改进。高通吹嘘骁龙 765 的 Spectra 355 ISP 能够处理 192MP 照片，但如果没有那个分辨率的 ZSL，就不要指望智能手机制造商会允许你拍摄完整的 192MP 照片。不过，高通确实表示，相机厂商正在研发超高像素的图像传感器。

我们所知道的是，在这一代发生变化的是视频捕捉。与 Spectra 350 的 720p@240fps 支持相比，Spectra 355 能够以 480fps 处理慢动作 720p 视频。此外，Spectra 355 增加了对 HDR10+中视频拍摄的支持。

**连通性**

***Modem***

高通正在积极地将自己定位于 5G 技术的前沿，他们指望骁龙 765 将 5G 智能手机带给大众。骁龙 765 是高通第一款集成 5G 的 SoC，这意味着 5G 调制解调器就在芯片上。这导致了更低的功耗，因为智能手机不必为分立调制解调器供电。然而，这并不意味着骁龙 765 在 5G 连接方面优于骁龙 865。

与[骁龙 X55](https://www.xda-developers.com/qualcomm-snapdragon-x55-5g-modem-2019-android-smartphones/) 一样，骁龙 X52 是一款多模式调制解调器，这意味着它能够支持 2G、3G、4G LTE 和 5G(6 GHz 以下和毫米波)连接。然而，当比较这两种调制解调器的规格时，你会发现，与搭配骁龙 865 的骁龙 X55 调制解调器相比，骁龙 X52 提供了最大理论 5G 下载速度的一半(3.7Gbps 对 7.5Gbps)，最大理论 5G 上传速度的一半(1.6Gbps 对 3.0Gbps)，毫米波带宽的一半(400MHz 对 800MHz)，以及 6GHz 以下带宽的一半(100MHz 对 200MHz)。4G LTE 速度也是如此。

然而，毫米波 5G 网络的部署仍在进行中，因此大多数用户不会看到接近理论最大值的 5G 速度。更重要的是，骁龙 X52 支持全球频段，并拥有高通开发的所有技术，以提高吞吐量、可靠性和可用性。诸如动态频谱共享、全球 5G 漫游、多 SIM 卡 5G、5G 节能和高通宽带包络跟踪等技术都在骁龙 X52 调制解调器中实现，仅举几例。

***地点***

像最新的 800 系列芯片组一样，骁龙 765 支持[双频 GNSS](https://www.xda-developers.com/dual-frequency-gnss-important-location-feature-your-phone-probably-missing/) ，如果智能手机有一个能够支持多个频率(L1+L5 或 E1+E5a)的芯片，它可以实现更精确的位置跟踪。这是首款支持此功能的骁龙 700 系列芯片组。

**内存**

正如我们在最近的一些旗舰设备中看到的那样，4GB 的 RAM 可能不足以处理复杂的相机处理，同时在后台运行高端移动游戏和其他应用程序，而不杀死其中一个或多个进程。骁龙 730 已经支持高达 8GB 的内存芯片，但现在骁龙 765 支持高达 12GB 的内存容量！更好的是，765 支持高达 2133MHz 的内存速度，比 730 提高了 267MHz。内存速度的提高可能不太重要，但额外的 4GB 内存可以发挥很大作用。与此同时，高级骁龙 865 现在支持 LPDDR5 内存，从而提高了骁龙 700 系列必须满足的标准。也许明年吧。

**充电**

高通最新的快速充电技术[仍在研发中](https://www.xda-developers.com/qualcomms-next-quick-charge-32w-fast-charging/)，看起来，27W [快速充电 4+](https://www.xda-developers.com/qualcomm-introduces-quick-charge-4-nubia-z17-to-bring-it-first/) 仍是骁龙 765 的首选快速充电技术。然而，高通增加了一项新的“快速充电人工智能”技术，据称可以延长智能手机电池的寿命。与骁龙 730 相比，配备骁龙 765 的设备的电池寿命最多可延长 200 个周期。高通没有分享关于快速充电人工智能如何工作的许多细节，但它可能使用像 USB-PD PPS (USB-Power Delivery 可编程电源)这样的动态电压调整。)

但是等等，还有更多！认识一下高通骁龙 765G

为了迎合手机游戏玩家，高通再次设计了其最新的骁龙 700 系列芯片的变体，具有更强的功能和一些以游戏为中心的功能。骁龙 765G 与骁龙 765 基本相同，但具有以下优势:

*   单核 CPU 性能稍高(主内核时钟速度从 2.3 GHz 提高到 2.4 GHz)
*   GPU 性能稍快(速度提升 15%)
*   选择骁龙精英游戏功能(游戏平滑器、游戏快速加载器、游戏网络延迟管理器、邱建减速器 2.0、预测游戏自动调谐器)

### 高通骁龙 765 完整的功能列表。单击以展开。

**高通 AI 引擎**

*   adre no 620 GPU(765g 上的 15%速度分级 GPU)
*   高通 Kryo 475 CPU
*   Hexagon 696 处理器
*   六边形向量扩展
*   六边形张量加速器
*   高通传感中心
    *   用于音频、语音和传感器的超低功耗集线器
    *   低功耗支持人工智能算法
    *   支持融合上下文数据流，包括传感器、音频和语音
    *   支持多个语音助手
    *   始终在线的多话筒远场检测和回声消除

**5G 调制解调器-射频系统**

*   骁龙 X52 5G 调制解调器-射频系统–面向 5G 多模式的调制解调器至天线集成系统
*   5G 毫米波和 6 GHz 以下，独立(SA)和非独立(NSA)模式，FDD、TDD
*   动态频谱共享
*   毫米波:400 MHz 带宽，2x2 MIMO
*   低于 6 GHz: 100 MHz 带宽，4x4 MIMO
*   高通 5G 节能
*   高通智能传输技术
*   高通宽带包络跟踪
*   高通信号增强自适应天线调谐
*   全球 5G 多 SIM 卡
*   下行:最高 3.7 Gbps (5G)，1.2 Gbps (LTE)
*   上行链路:最高 1.6 Gbps (5G)，210 Mbps (LTE)
*   多模支持:5G NR、LTE，包括 CBRS、WCDMA、HSPA、TD-SCDMA、CDMA 1x、EV-DO、GSM/EDGE

**Wi-Fi &蓝牙**

*   高通快速连接 6200 子系统
    *   Wi-Fi 标准:802.11ax 就绪、802.11ac 第二波、802.11a/b/g、802.11n
    *   Wi-Fi 频段:2.4 GHz、5 GHz
    *   信道利用率:20/40/80 MHz
    *   MIMO 配置:采用 MU-MIMO 的 2x2 (2 流)
    *   8 流探测(用于 8×8 MU-MIMO)
    *   双频同步(DBS)
    *   Wi-Fi 安全性:WPA3-企业级、WPA3-增强型开放式、wpa 3 轻松连接、wpa 3-个人级
    *   目标唤醒时间(TWT)
*   集成蓝牙
    *   蓝牙版本:5.0
    *   蓝牙速度:2 Mbps
    *   蓝牙音频:高通 TrueWireless 技术，高通 aptX Adaptive

**摄像机**

*   高通 Spectra 355 图像信号处理器
*   双通道 14 位 ISP
*   计算机视觉硬件加速器(CV-ISP)
*   高达 192 MP 捕获
*   高达 22 MP 的双摄像头，零快门延迟
*   高达 3600 万像素的单摄像头，零快门延迟
*   建议。2020 色域视频捕捉
*   高达 10 位色彩深度视频捕捉
*   720p、480fps 的慢动作视频拍摄
*   HEIF: HEIC 照片捕捉，HEVC 视频捕捉
*   视频采集格式:HDR10+，HDR10，HLG
*   4K·HDR 用肖像模式拍摄视频(散景)
*   多帧降噪(MFNR)
*   实时对象分类、分割和替换

**音频**

*   用于硬件加速语音信号处理的六边形语音辅助加速器
*   高通 Aqstic 音频编解码器(最高支持 WCD9385)
    *   总谐波失真+噪声(THD+N)，回放:-108dB
    *   原生 DSD 支持，PCM 最高 384 kHz/32 位
    *   可定制的“金耳朵”过滤器
*   高通 Aqstic 智能扬声器放大器(高达 WSA8815)

**显示**

*   设备上显示支持:
    *   60 赫兹的 QHD+
    *   FHD+120 赫兹
*   最大外部显示器支持:60Hz UHD
*   10 位颜色深度。2020 色域
*   HDR10 和 HDR10+

**CPU**

*   Kryo 475，八核 CPU
*   高达 2.3 GHz (765)
*   最高 2.4 GHz(765 克)
*   64 位架构

**视觉子系统**

*   Adreno 620 GPU
*   Vulkan 1.1 API 支持
*   4K HDR10 PQ 和 HLG 视频播放(10 位色深，记录。2020 色域)
*   H.264 (AVC)、H.265 (HEVC) VP8 和 VP9 播放
*   基于物理的渲染
*   API 支持:OpenGL ES 3.2、OpenCL 2.0 FP、Vulkan 1.1、DirectX 12

**安全**

*   生物认证:指纹、虹膜、声音、面部
*   设备上:高通移动安全、密钥供应安全、高通处理器安全、高通内容保护、高通可信执行环境、摄像头安全、加密引擎、恶意软件防护、安全引导、安全令牌

**充电**

*   高通快充 4+技术
*   高通快充 AI

**地点**

*   GPS、Glonass、北斗、伽利略、QZSS 和 SBAS
*   双频支持
*   低功耗地理围栏和跟踪、传感器辅助导航

**通用规格**

*   精选的骁龙精英游戏功能包括:游戏平滑器、游戏快速加载器和游戏网络延迟管理器(765G)
*   内存速度:高达 2133 MHz，12 GB 内存
*   内存类型:2 个 16 位，LPDDR4x
*   近场通信(NFC)支持
*   USB Type-C 支持上的显示端口
*   7 纳米。加工工艺学
*   零件号:SM7250-AA (765)
*   零件号:SM7250-AB (765G)

由骁龙 765 系列驱动的移动设备将于今年晚些时候和 2020 年发布。[小米的 Redmi K30 和 OPPO 的 Reno3 Pro](https://www.xda-developers.com/xiaomi-redmi-k30-oppo-reno3-pro-snapdragon-765/) 已被证实将采用骁龙 765G，而 HMD Global 和摩托罗拉也证实他们正在开发基于 765 或 765G 移动平台的智能手机。采用这种 SoC 的设备将主要在印度和中国等市场销售，在这些市场，移动游戏是一个巨大的市场，智能手机竞争非常激烈，但我们可以预计至少会有一些采用这些芯片组的设备登陆欧洲。