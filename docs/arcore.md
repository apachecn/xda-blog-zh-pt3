# Google ARCore:关于增强现实平台你需要知道的一切

> 原文：<https://www.xda-developers.com/arcore/>

谷歌已经几次试图进入增强现实世界。增强现实，通常被称为 AR，如果使用得当，可能会成为改变生活的技术，但还没有一家科技公司能够掌握它。苹果已经采取了使用专用硬件的方法，如 iPads 和 iPhones 中包含的激光雷达扫描仪，而谷歌等其他公司则仅通过软件实现一切。然而，我们肯定越来越接近完美的 AR，谷歌是领先的公司之一，他们拥有增强现实 SDK 和技术，被称为“ARCore”。

但是 ARCore 是什么呢？支持哪些手机？最重要的是，你应该关心 ARCore 吗？

* * *

## ARCore 是什么？

ARCore 也称为“用于 AR 的 Google Play 服务”，是一个谷歌软件开发工具包，允许开发人员创建增强现实应用程序。它于 2018 年首次推出，自那以来，它已经成为几家制造商的许多智能手机的一部分。它可以在大多数高端和中档 Android 设备上工作，并被改编成一些非常酷的用例，其中一些是合理有用的，而一些可以被认为是更“噱头”。

ARCore 肯定不是谷歌第一次涉足 AR 领域。有些人可能还记得谷歌第一次涉足增强现实技术的项目 Tango。ARCore 和 Project Tango 有很多共同之处，但也有不同之处。特别是，项目 Tango 需要专用硬件，配备多台摄像机和特殊传感器。当 Project Tango 还是一个东西的时候，拥有一个以上的后置传感器几乎是闻所未闻的，更不用说集成 Tango 所需的相机技术了，包括像鱼眼相机这样的功能。

另一方面，ARCore 要有趣得多，因为它不需要任何特殊的硬件。它用你的手机的摄像头和内部传感器做一切事情，不需要更多或更少的东西。这意味着任何普通的智能手机都可以很好地享受 ARCore 增强现实体验。Project Tango 最终被终止，并被 ARCore 取代，因为它是一个更具可扩展性的解决方案，几乎可以与任何手机兼容。

* * *

## ARCore 是如何工作的？

当然，与 Project Tango 不同，ARCore 完全不需要特殊的传感器，因为它意味着可以在带有传统相机设置的消费设备上工作。这意味着它只依赖于你的相机，你手机的运动传感器，如陀螺仪和加速度计，以及谷歌的一些软件技巧来完成它的工作。ARCore 遵循一系列基本概念，以便成功地看到和解释摄像机看到的内容，并基于这些信息提供增强现实体验。

ARCore 使用[同步定位和地图](https://en.wikipedia.org/wiki/Simultaneous_localization_and_mapping)，或 SLAM，来了解手机相对于周围世界的确切位置。它设法通过检测捕获的相机图像中的视觉上不同的特征来计算位置的变化，然后使用该特征点来知道它是否改变了位置以及该位置的特征。它使用这些特征点来检测平面或水平/垂直表面，并将其用于附加的上下文。

为了推断相机随着时间推移相对于环境的姿态(位置和方向)，该视觉信息还与设备 IMU 的惯性测量值配对。使用这些信息和上下文，开发人员可以通过摄像头渲染事物，使其看起来像是真实世界的一部分。它还可以推断平面中有多少光，并使用该上下文，根据 ARCore 认为有多少光照射到它，使渲染的图像看起来更亮或更暗。

这些基本概念是一本很好的读物，如果你有兴趣了解 ARCore 如何变魔术的来龙去脉，你应该去看看。虽然这个故事比页面上说的要多得多，但它确实让您很好地了解了它到底是如何做的。

* * *

## 有哪些手机可以运行 ARCore？

谷歌并没有对 ARCore 支持的设备提出精确的系统要求。在这方面，我们只知道这些受支持的设备至少需要运行 Android 7.0 牛轧糖，Android 8.0 奥利奥是最佳选择。然而，对于某些设备，可能需要更新的 Android 版本。但是谷歌并没有公布该平台的系统需求，因为一个特殊的原因——ARCore 支持实际上需要谷歌手动切换。

之所以会这样，有几个原因。ARCore 支持的所有手机都经过谷歌的手动测试和认证，以确保手机与增强现实服务最佳配合，包括摄像头和运动传感器的质量，以及 CPU 处理屏幕背后一切的能力。虽然现在大多数智能手机都足够强大，可以毫不费力地支持 ARCore，但手机仍然需要手动认证，以确保完全兼容，并确保设备能够提供最佳的 ARCore 体验。

截至本文撰写之时，已有数百个 ARCore 设备得到支持。其中一些来自最受欢迎的品牌，包括:

### 谷歌

### 支持谷歌 ARCore 的谷歌设备列表。单击以展开。

*   谷歌 Nexus 5X
*   谷歌 Nexus 6P
*   谷歌像素
*   谷歌像素 XL
*   谷歌像素 2
*   谷歌像素 2 XL
*   谷歌像素 3
*   谷歌 Pixel 3 XL
*   谷歌像素 3a
*   谷歌 Pixel 3a XL
*   谷歌像素 4
*   谷歌 Pixel 4 XL
*   谷歌像素 4a
*   谷歌像素 4a 5G
*   谷歌像素 5
*   谷歌 Pixel 5a 5G
*   谷歌像素 6
*   谷歌 Pixel 6 Pro
*   谷歌像素 6a
*   谷歌像素 7
*   谷歌 Pixel 7 Pro

### 华硕

### 支持谷歌 ARCore 的华硕设备列表。单击以展开。

*   华硕 ROG 手机
*   华硕 ROG 手机 II
*   华硕 ROG 手机三
*   华硕 ROG 手机 5
*   华硕 Zenfone 6
*   华硕 Zenfone 7/7 Pro
*   华硕 Zenfone 8
*   华硕 Zenfone 9
*   华硕 Zenfone AR
*   华硕 Zenfone ARES

### HMD 移动

### 支持谷歌 ARCore 的 HMD 移动设备列表。单击以展开。

*   HMD 诺基亚 3.4
*   HMD 诺基亚 5.4
*   HMD 诺基亚 6 (2018)
*   HMD 诺基亚 6.1 Plus
*   HMD 诺基亚 6.2
*   HMD 诺基亚 7 Plus
*   HMD 诺基亚 7.1
*   HMD 诺基亚 7.2
*   HMD 诺基亚 8
*   HMD 诺基亚 8 热风
*   HMD 诺基亚 8.1
*   HMD 诺基亚 8.3 克

### 常简称为 HTC 或宏达电

### 支持谷歌 ARCore 的 HTC 设备列表。单击以展开。

### 华为

### 支持谷歌 ARCore 的华为设备列表。单击以展开。

*   华为荣耀 8X
*   华为荣誉 10
*   华为 Honor View 10 Lite
*   华为荣誉 V20
*   华为 Mate 20 Lite
*   华为 Mate 20
*   华为 Mate 20 Pro
*   华为 Mate 20 X
*   华为 Nova 3
*   华为 Nova 3i
*   华为 Nova 4
*   华为 P20
*   华为 P20 Pro
*   华为 P30
*   华为 P30 Pro
*   华为保时捷设计 Mate RS
*   华为保时捷设计 Mate 20 RS
*   华为 Y9 2019

### Infinix

### 支持 Google ARCore 的 Infinix 设备列表。单击以展开。

*   无限注 6
*   Infinix Note 7
*   Infinix 零 8
*   Infinix Note 10 Pro
*   无限零 X
*   Infinix 零 X 新
*   Infinix Note 11
*   Infinix Note 11 Pro
*   Infinix Note 11S

### 京瓷公司

### 支持谷歌 ARCore 的京瓷设备列表。单击以展开。

*   京瓷扭矩 5G
*   京瓷扭矩 G04
*   京瓷 Duraforce Ultra 5G

### 联想（电脑的品牌名）

### 支持谷歌 ARCore 的联想设备列表。单击以展开。

*   联想 K13 Note
*   联想 Tab P11 Pro
*   联想标签 P11 5G
*   联想标签 P11 Plus
*   联想 Tab P12 Pro
*   联想 Yoga Tab 11

### 利特拜莱亚

### 支持谷歌 ARCore 的 LitByleia 设备列表。单击以展开。

### 水平规ˌ水准仪(Level Gauge)

### 支持谷歌 ARCore 的 LG 设备列表。单击以展开。

*   LG G6
*   LG G7 Fit
*   LG G7 One
*   LG G7 薄 q
*   LG G8 ThinQ
*   LG G8S ThinQ
*   LG G8X ThinQ
*   LG G Pad 5 10.1 FHD
*   LG K61
*   LG K71
*   LG K92
*   LG Q6
*   LG Q70
*   LG Q8
*   LG Q92
*   LG 风格 2
*   LG 风格 3
*   LG Stylo 5
*   LG Stylo 6
*   LG Stylo 7
*   LG V30
*   LG V30+
*   LG V30+ JOJO
*   LG 签名版 2017
*   LG V35 ThinQ
*   LG 签名版 2018
*   LG V40 ThinQ
*   LG V50 ThinQ
*   LG V50S ThinQ
*   LG 签名版 2019
*   LG V60 ThinQ
*   LG V60 ThinQ 5G
*   LG 天鹅绒 5G
*   LG 天鹅绒 2 pro
*   LG Wing 5G

### 摩托罗拉

### 支持谷歌 ARCore 的摩托罗拉设备列表。单击以展开。

*   摩托罗拉摩托 G5S Plus
*   摩托罗拉摩托 G6
*   摩托罗拉摩托 G6 Plus
*   摩托罗拉摩托 G7
*   摩托罗拉摩托 G7 Play
*   摩托罗拉摩托 G7 Plus
*   摩托罗拉摩托 G7 动力
*   摩托罗拉摩托 G7 Play
*   摩托罗拉摩托 G8
*   摩托罗拉摩托 G8 Play
*   摩托罗拉摩托 G8 Plus
*   摩托罗拉摩托 G8 动力
*   摩托罗拉 Moto G8 Power lite
*   摩托罗拉摩托 G9 Play
*   摩托罗拉摩托 G9 Plus
*   摩托罗拉摩托 G9 动力
*   摩托罗拉摩托 G 5G
*   摩托罗拉摩托 G 动力 2021
*   摩托罗拉摩托 G 动力
*   摩托罗拉摩托 G Pro
*   摩托罗拉摩托 G 手写笔
*   摩托罗拉 Moto G 手写笔(2020)
*   摩托罗拉摩托 G(100)
*   摩托罗拉摩托 G(50)
*   摩托罗拉摩托 G(30)
*   摩托罗拉摩托 G(10)
*   摩托罗拉 Moto G 手写笔 5G
*   摩托罗拉摩托 G(40) fusion
*   摩托罗拉摩托 G(50) 5G
*   摩托罗拉摩托 G(60)
*   摩托罗拉摩托 G(60)s
*   摩托罗拉·莫托·拉兹尔(2020)
*   摩托罗拉边缘
*   摩托罗拉边缘 S
*   摩托罗拉边缘+
*   摩托罗拉边缘 20
*   摩托罗拉 Edge 20 Lite
*   摩托罗拉 Edge 20 专业版
*   摩托罗拉一号
*   摩托罗拉 One 5G
*   摩托罗拉一招
*   摩托罗拉一号核聚变
*   摩托罗拉 One Fusion+
*   摩托罗拉一超
*   摩托罗拉一宏
*   摩托罗拉一号电力公司
*   摩托罗拉 One Zision
*   摩托罗拉一变焦
*   摩托罗拉摩托 X4
*   摩托罗拉摩托 Z2 部队
*   摩托罗拉摩托 Z3
*   摩托罗拉摩托 Z3 play
*   摩托罗拉摩托 Z4

### 一加

### 支持谷歌 ARCore 的一加设备列表。单击以展开。

*   OnePlus 3T
*   一加 5
*   一加 5T
*   一加 6
*   一加 6T
*   一加 7
*   一加 7 专业版
*   一加 7 Pro 5G
*   一加 7T
*   一加 7T 专业版
*   一加 8
*   一加 8 专业版
*   一加 8T
*   一加 9
*   一加 9 专业版
*   一加 9R
*   一加 10 专业版
*   一加 11
*   北一加
*   一加北部 N10 5G
*   一加北部
*   一加诺德 N200 5G
*   一加诺德 2 5G

### 同僚

### 支持谷歌 ARCore 的 Oppo 设备列表。单击以展开。

*   Oppo A52
*   Oppo A72
*   Oppo A72 5G
*   Oppo A92
*   Oppo A92s
*   Oppo A93 5G
*   Oppo A94
*   Oppo F11 Pro
*   Oppo F15
*   Oppo F17 Pro
*   Oppo F19 Pro+
*   Oppo 找 X2
*   Oppo Find X2 Pro
*   Oppo Find X3 Pro
*   Oppo Find X5 Pro
*   Oppo K3
*   Oppo K5
*   Oppo R17 Pro
*   Oppo Reno
*   Oppo 雷诺 2
*   Oppo 雷诺 2 F
*   Oppo 雷诺 2 Z
*   Oppo 雷诺 3
*   Oppo Reno 3 5G
*   Oppo 雷诺 3 A
*   Oppo 雷诺 3 Pro
*   Oppo Reno 3 Pro 5G
*   Oppo Reno 4 4G
*   Oppo Reno 4 SE 5G
*   Oppo 雷诺 5 A
*   Oppo Reno 5 5G
*   Oppo 雷诺 5 Pro 4G
*   Oppo Reno 5 Pro 5G
*   Oppo Reno 5 Pro+ 5G
*   Oppo 雷诺 6 Pro+ 5G
*   Oppo Reno 10x 倍变焦
*   Oppo 雷诺 A
*   Oppo 雷诺 Z

### 真我

### 支持谷歌 ARCore 的 Realme 设备列表。单击以展开。

*   现实 5
*   Realme 5 Pro
*   现实 6
*   Realme 6 Pro
*   现实 7
*   Realme 7i
*   Realme 7 Pro
*   Realme 8 Pro
*   Realme Narzo 20 Pro
*   真实 Q
*   Realme X
*   Realme X Lite
*   Realme XT
*   真实的 X2
*   皇家 X2 专业版
*   Realme X3 超级变焦
*   Realme X7 5G
*   Realme X7 Pro 5G
*   Realme X50 Pro
*   Realme X50t 5G
*   Realme V5 5G
*   Realme V15 5G
*   Realme GT 5G
*   现实 GT Neo
*   Realme 8 5G

### 三星电子

### 锋利的

### 支持谷歌 ARCore 的夏普设备列表。单击以展开。

*   夏普 AQUOS R3
*   夏普 AQUOS R5G
*   夏普 AQUOS sense3
*   夏普 AQUOS sense3 基础版
*   夏普 AQUOS sense3 plus
*   夏普 AQUOS sense4
*   夏普 AQUOS sense4 基础版
*   夏普 AQUOS sense4 lite
*   夏普 AQUOS sense4 plus
*   夏普 AQUOS sense5G
*   夏普 AQUOS sense6
*   夏普 AQUOS zero2
*   夏普 AQUOS zero5G 基本款
*   夏普 AQUOS zero5G 基础 DX
*   夏普 AQUOS zero6
*   夏普 S7
*   夏普莱茨手机 1

### 索尼

### 支持谷歌 ARCore 的索尼设备列表。单击以展开。

*   索尼 Xperia XZ Premium
*   索尼 Xperia XZ1
*   索尼 Xperia XZ1 紧凑型
*   索尼 Xperia XZ2
*   索尼 Xperia XZ2 紧凑型
*   索尼 Xperia XZ2 高级版
*   索尼 Xperia XZ3
*   索尼 Xperia 1
*   索尼 Xperia 1 专业版
*   索尼 Xperia 1 II
*   索尼 Xperia 5
*   索尼 Xperia 5 II
*   索尼 Xperia 5 III
*   索尼 Xperia 10 III
*   索尼 Xperia PRO

### TCL 集团股份有限公司（TCL Corporation 的缩写）

### 支持谷歌 ARCore 的 TCL 设备列表。单击以展开。

### 泰克诺

### 支持谷歌 ARCore 的 Tecno 设备列表。单击以展开。

*   Tecno Camon 12 Pro
*   Tecno Camon 16 Premier
*   Tecno Camon 16 Pro
*   Tecno Camon 17 Pro
*   Tecno Camon 18P
*   Tecno Camon 18 Premier
*   泰克诺幻影 9
*   Tecno Phantom X Pro
*   Tecno 幻影 V 形折叠
*   Tecno Pova 2

### UMX(超移动体验)

### 支持 Google ARCore 的 UMX(超移动体验)设备列表。单击以展开。

### Vinsmart

### 支持谷歌 ARCore 的 Vinsmart 设备列表。单击以展开。

*   Vinsmart 直播 4
*   Vinsmart Aris Pro

### 活泼的

### 支持谷歌 ARCore 的 Vivo 设备列表。单击以展开。

*   Vivo Nex 3
*   Vivo Nex 3 5G
*   Vivo NEX S
*   Vivo NEX 双显版
*   Vivo iQOO 3 4G
*   Vivo iQOO 3 5G
*   Vivo V17
*   Vivo V20
*   Vivo V20 Pro
*   Vivo X23
*   Vivo X50
*   Vivo X50 Pro
*   Vivo X50e 5G
*   Vivo X60 Pro
*   Vivo X70 Pro
*   Vivo I2011
*   Vivo V2041
*   Vivo V2045
*   Vivo V2046
*   Vivo V2050

### Wiko

### 支持谷歌 ARCore 的 Wiko 设备列表。单击以展开。

### 小米

### 支持谷歌 ARCore 的小米设备列表。单击以展开。

*   小米 Mi 8
*   小米 Mi 8 SE
*   小米 Mi 9
*   小米 Mi 9 Lite
*   小米 Mi 9 SE
*   小米 Mi 10
*   小米 Mi 10i
*   小米 Mi 10 Lite
*   小米 Mi 10 Lite 5G
*   小米 Mi 10 Lite 变焦
*   小米 Mi 10 Pro
*   小米米 10T Pro
*   小米米 11
*   小米 11T
*   小米 Mi 11 Pro
*   小米 Mi 11 Lite 5G
*   小米 Mi 11 Ultra
*   小米 Mi A3
*   小米 Mi Mix 2S
*   小米 Mi Mix 3
*   小米 Mi Note 10
*   小米米 Note 10 Lite
*   小米 Pocophone F1
*   小米 POCO X2
*   小米 POCO X3
*   小米 POCO X3 NFC
*   小米 Poco X3 Pro
*   小米 POCO M2 Pro
*   小米 Redmi K20
*   小米 Redmi K20 Pro
*   小米 Redmi K30
*   小米 Redmi K30 Pro
*   小米 Redmi K40
*   小米 Redmi K40 Pro/Pro+
*   小米 Redmi Note 7
*   小米红米 Note 7 Pro
*   小米 Redmi Note 8
*   小米 Redmi Note 8 Pro
*   小米 Redmi Note 8T
*   小米 Redmi Note 9
*   小米 Redmi Note 9 Pro
*   小米红米 Note 9 Pro Max
*   小米 Redmi Note 9S
*   小米红米 Note 9 (5G)
*   小米 Redmi Note 10
*   小米 Redmi Note 10S
*   小米红米 Note 10 5G
*   小米红米 Note 10 Pro
*   小米红米 Note 10 Pro Max
*   小米 Redmi 10X 4G
*   小米 Pad 5

### 斑马

### 支持谷歌 ARCore 的 Zebra 设备列表。单击以展开。

*   斑马 ET51s 8 英寸企业平板电脑
*   斑马 ET56s 8 英寸企业平板电脑
*   斑马 ET56 10 英寸企业平板电脑
*   斑马 TC21 无线局域网触摸电脑
*   斑马 TC26 无线触摸电脑
*   斑马 EC50 无线局域网企业计算机
*   斑马 EC55 WWAN 企业计算机
*   斑马 TC52 无线局域网触摸电脑
*   斑马 TC52x 无线局域网触摸电脑
*   斑马 TC57 无线触摸电脑
*   斑马 TC57x 无线触摸电脑
*   斑马 TC72 无线局域网触摸电脑
*   斑马 TC77 无线触摸电脑
*   斑马 ET51L 10 英寸企业平板电脑
*   斑马 ET56L 10 英寸企业平板电脑

### 中兴通讯股份有限公司（Zhongxing Telecommunication Equipment Corporation 的缩写）

### 支持谷歌 ARCore 的中兴设备列表。单击以展开。

*   中兴 Libero 5G
*   中兴 Libero 5G II

此外，ARCore 还支持少数只在中国销售的手机，其中一些不在此列。要在这些中国智能手机上使用 ARCore，没有 Google Play 或 Google Play 服务可供下载，但谷歌确实在中国的其他应用商店(如华为的 AppGallery、小米的 App Store、Oppo 的 App Market 等)上单独提供了“用于 AR 的 Google Play 服务”组件。

* * *

## 你应该关心 ARCore 支持吗？

ARCore 为你的日常生活带来了一些非常酷的技术和用例，谷歌完全投入到这项技术中，每天都在让它变得更好。最好的例子就是 Measure 应用。这个应用程序实际上是从 Project Tango 借来的，虽然远不是绝对精确的东西，但它允许你通过使用手机的摄像头来精确测量现实生活中的事情。我用它来测量从人、狗甚至树的各种东西，最多也就差几厘米。虽然谷歌已经扼杀了这款应用，但增强现实的底层技术在这个用例之外继续蓬勃发展。

如果你喜欢纹身，还有一个名为 [InkHunter](https://play.google.com/store/apps/details?id=tattoo.inkhunter) 的应用程序，它使用 ARCore 让你在实际预约纹身师之前尝试纹身，看看你是否喜欢它穿在你身上的样子。如果你对多种设计或者纹身本身的位置犹豫不决，这是非常有用的。

Snapchat 和抖音等其他应用程序也在 Android 智能手机上利用 ARCore 的技术来增强自己的应用内增强现实体验，包括面部检测等方面的改进。

像这样的用例有很多。易贝有一个功能，在 AR 中显示一个盒子，以确定什么是运输东西的最佳盒子。Wayfair 允许您在家中摆放虚拟家具，这样您就可以看到它在家中的美观程度。 [ColorSnap Visualizer](https://play.google.com/store/apps/details?id=com.colorsnap) 可以用 AR 给你的墙壁上色，所以你可以在真正给你的墙壁上色之前预览颜色。你甚至可以用它来学习，利用像 [GeoGebra](https://play.google.com/store/apps/details?id=org.geogebra.android.g3d) 学习数学/代数和[人体解剖图谱](https://play.google.com/store/apps/details?id=com.visiblebody.atlas)学习解剖学。

当然，也许迄今为止它最广泛的用途是在游戏中。一些游戏利用这项技术在游戏过程中提供更丰富、更精确和更有趣的 AR 体验。Pokémon GO 开创了 AR 游戏的潮流，并在 2016 年问世时风靡一时，成为一个非常有趣的夏天。现在 Pokémon GO 用的是 ARCore，像《弗雷迪的五夜 AR:快递》、《侏罗纪世界活着》、《行尸走肉:我们的世界》等游戏也是。

* * *

## 底线

ARCore 作为一个概念，是很神奇的。它可能远远不是显示 ar 内容的最佳解决方案之一，但它是精简的，可以在大多数现代 Android 手机上工作，并且不需要任何专门的硬件。它在可伸缩性和整体平台采用方面都有很大的优势，Google 一直在改进它，以提高效率和精确度。它经常被直接与苹果自己的 AR 解决方案 ARKit 相比较，后者也不需要任何特殊的硬件(尽管它最近开始利用一些苹果设备中包含的激光雷达传感器)。但 ARCore 有很大的优势，比如全球市场的大部分都在使用 Android，更不用说 ARCore 也可以在 iOS 上使用。

它给用户带来的惊人用途确实令人着迷。摆放家具、测量物品、尝试纹身对很多人来说肯定会派上用场。但是，在很大程度上，在 iOS 上使用 ARCore 或 ARKit 的应用数量非常有限。智能手机上的增强现实还没有被广泛使用。它可能有一天会实现，正如 2016 年的 Pokémon GO 狂潮所证明的那样，但它需要与现实世界更多地融合才能实现。

然而，到目前为止，ARCore 是一个很酷的特性。这可能是一个小众功能，只有发烧友才会以半持续的方式使用，但仍然很酷。