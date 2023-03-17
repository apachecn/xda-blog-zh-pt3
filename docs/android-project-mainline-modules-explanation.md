# 关于 Android 项目主线你需要知道的一切

> 原文：<https://www.xda-developers.com/android-project-mainline-modules-explanation/>

相对于其重要性而言，Android 近年来最大的变化之一是在 Android 10 中引入了[项目主线](https://www.xda-developers.com/android-q-project-mainline-security/)。谷歌强制要求在 Android 版本中包含特定的主线模块，其中[的 Android 11](https://www.xda-developers.com/android-11-stable-google-pixel-oneplus-xiaomi-realme-oppo/) 与[的总共 25 个主线模块](https://www.xda-developers.com/android-11-stable-google-pixel-oneplus-xiaomi-realme-oppo/)一起推出。这里有一个关于什么是项目主线和它的目标是解决什么的解释，以及一个 Android 的所有项目主线模块的列表。

## 什么是项目主线？

为了正确理解项目主线，我们必须倒回一点。如果你回到几年前，很多关于 Android 更新的讨论都集中在碎片化问题上。在冰淇淋三明治-棒棒糖时代，碎片化是谷歌在 Android 上要解决的最大挑战之一。尽管 Android 作为一个平台，在很大程度上可以预测的模式下定期收到更新，但这些更新通常需要很长时间才能到达最终消费者手中，如果有的话。因此，虽然谷歌在平台层面修复了关键的漏洞和安全问题，但这些变化的实际推出仍有许多不足之处。有许多中间商(SoC 供应商、原始设备制造商、运营商等)。)和许多移动部件参与了向您的手机提供更新，碎片问题似乎不会在不需要一些强硬干预的情况下自行解决。

解决这个问题的主要努力之一是以 Android 8.0 Oreo 旁边的 Treble 项目的形式出现的，该项目涉及 Android 的重大重组，将 Android OS 框架组件与供应商 HALs 和 Linux 内核分离。从本质上来说，Project Treble 通过将操作系统框架从特定于设备的底层软件中分离出来，将 Android 模块化。通过这种方式，设备制造商(OEM)无需等待芯片制造商(SoC 供应商)更新他们的供应商实现代码，OEM 可以独立更新 Android OS 框架。最终结果是 OEM 厂商更快地采用更新的 Android 版本，因为他们不再需要等待中间人(SoC 供应商)先完成工作，然后才能开始做他们的工作。

虽然 Android 更新情况并没有随着 Project Treble 的推出而得到显著改善，但它在很大程度上促进了更广泛的 OEM 参与 Android 10 和 Android 11 测试版，并使 OEM 更容易在更短的时间内更新更多的设备。此外，GSI(通用系统映像)的整个概念对我们论坛上的售后市场发展产生了重大影响。

**[开发者用项目三冠王 GSI](https://www.xda-developers.com/developer-boots-android-11-22-older-devices-project-treble-gsi/)** 在 22 台老设备上启动 Android 11

项目主线延伸了项目三倍的努力。虽然 Treble 降低了原始设备制造商对 SoC 供应商进行每一次操作系统更新的依赖程度，但 Mainline 降低了谷歌对原始设备制造商提供关键操作系统组件安全更新的依赖程度。Project Mainline 将三重理念扩展到 Android 框架的更关键部分，将 OEM 从这个等式中移除。Project Mainline 的目的是让 Google 从原始设备制造商手中夺取对安全性和维护开发一致性至关重要的框架组件和系统应用程序的控制权。Project Mainline 被恰当地称为自 Project Treble 以来对 Android 的[最大改变。](https://www.xda-developers.com/android-q-apex-biggest-thing-since-project-treble/)

对于项目主线，Google 使用通过 Google Play 服务框架和谷歌 Play 商店交付的主线模块。每个主线模块以 APK 文件、APEX 文件或 APK-in-APEX 的形式交付。当主线模块正在更新时，用户会在他们的设备上看到“Google Play 系统更新”(GPSU)通知。实际上，为了向关键组件提供更新，谷歌已经绕过了等待 OEM 厂商推出更新的需要，选择自己完成这项任务。

正如谷歌在安卓网站上所说的:

*模块化系统组件使谷歌和 Android 合作伙伴能够以非侵入式方式向最终用户设备广泛、快速、无缝地分发更新。例如，媒体编解码器碎片和关键错误的结合会显著降低应用的采用率和用户参与度。对媒体相关模块的频繁更新可以减少编解码器碎片，使媒体应用程序在不同 Android 设备上的行为更加一致，并修复关键错误以建立用户信任。*

*Android 10 或更高版本将选定的系统组件转换为模块，其中一些使用 APEX 容器格式(在 Android 10 中引入)，另一些使用 APK 格式。模块化架构使系统组件能够根据需要更新关键的错误修复和其他改进，而不会影响较低级别的供应商实施或较高级别的应用和服务。*

正如 [*Ars Technica* 提到的](https://arstechnica.com/gadgets/2020/09/android-11-the-ars-technica-review/5/):

*项目主线，又名“Google Play 系统更新”，是在 Android 10 中引入的，作为一项重大努力，使 Android 的核心系统组件更加模块化和可更新。Mainline 专门为系统组件引入了一种新的“APEX”文件类型，其目标是通过 Play Store 发布核心 Android 代码，就像发布应用程序更新一样简单。此前，Android 唯一可发布的代码块是 APK，这是一种最初为第三方应用设计的文件类型。这带来了各种各样的安全限制，并且只能在启动过程的后期启动，因此 APEX 是在考虑更强大的系统组件的情况下创建的。apex 只能由 Google 或您的设备制造商创建，因此它们的功能明显更强大，并且包含关键的启动组件，如应用程序运行时。*

Mainline 不仅仅是一个技术解决方案，它还涉及到让谷歌集中发布 Android 的更多部分，这涉及到与设备制造商谈判，并让他们都同意发布相同的代码块。主线模块最终成为强制发货，因此主线实际上是与设备制造商的一次大合作，以确保单个生态系统范围的模块满足每个人的需求。并不是每个主线模块都是超级强大的 APEX 模块——有些只是 apk，现在是 Google 分发的 Android 代码。

## 项目主线—模块

在 Android 10 中，谷歌强制要求包含 13 个特定的主线模块。对于 Android 11，强制模块总数为 25。以下是完整列表，以及一些关键细节:

| 

模块名

 | 

包名

 | 

类型

 | 

设备升级到或使用 Android 11 启动

 | 

设备由机器人 10 启动

 | 

设备升级到 droid 10

 |
| --- | --- | --- | --- | --- | --- |
| [adbd](https://source.android.com/devices/architecture/modular-system/adbd) | com.google.android.adbd | 顶点 | 必须 | 无支持的 | 无支持的 |
| [安卓神经网络 API 运行时](https://source.android.com/devices/architecture/modular-system/nnapi) | com。谷歌。安卓。神经网络 | 顶点 | 必须 | 无支持的 | 无支持的 |
| [强制网络门户登录](https://source.android.com/devices/architecture/modular-system/networking) | com。谷歌。安卓。captivepotallogin | APK | 必须 | 强烈推荐 | 可选择的 |
| [小区广播](https://source.android.com/devices/architecture/modular-system/cellbroadcast) | com。谷歌。安卓。小区广播 | 顶点 | 必须 | 无支持的 | 无支持的 |
| [共密](https://source.android.com/devices/architecture/modular-system/conscrypt) | com。谷歌。安卓。密码 | 顶点 | 必须 | 强烈推荐 | 可选择的 |
| [DNS 解析器](https://source.android.com/devices/architecture/modular-system/dns-resolver) | com.google.android.resolv | 顶点 | 必须 | 强烈推荐 | 可选择的 |
| [文档 UI](https://source.android.com/devices/architecture/modular-system/documentsui) | com.google.android.documentsui | APK | 必须 | 必须 | 可选择的 |
| 延伸服务 - APK | com。谷歌。安卓。延伸文件系统服务 | APK | 必须 | 必须 | 必须 |
| [外部服务](https://source.android.com/devices/architecture/modular-system/extservices) - APEX | com.google.android.extservices | 顶点 | 必须 | 无支持的 | 无支持的 |
| [IPsec/IKEv2 库](https://source.android.com/devices/architecture/modular-system/ipsec) | com.google.android.ipsec | 顶点 | 必须 | 无支持的 | 无支持的 |
| [媒体编解码器](https://source.android.com/devices/architecture/modular-system/media) | com。谷歌。安卓。媒体。软件编解码器 | 顶点 | 必须 | 必须 | 可选择的 |
| [媒体框架组件](https://source.android.com/devices/architecture/modular-system/media) | com.google.android.media | 顶点 | 必须 | 必须 | 可选择的 |
| [媒体提供商](https://source.android.com/devices/architecture/modular-system/media) | com。谷歌。安卓。媒体提供商 | 顶点 | 必须 | 无支持的 | 无支持的 |
| [模块元数据](https://source.android.com/devices/architecture/modular-system/metadata) | com。谷歌。安卓。module 元数据 | APK | 必须 | 必须 | 必须 |
| [网络堆栈组件](https://source.android.com/devices/architecture/modular-system/networking) | com。谷歌。安卓。网络堆栈 | APK | 必须 | 强烈推荐 | 可选择的 |
| [网络栈权限配置](https://source.android.com/devices/architecture/modular-system/networking) | com。谷歌。安卓。网络堆栈。权限配置 | APK | 必须 | 强烈推荐 | 可选择的 |
| [权限控制人](https://source.android.com/devices/architecture/modular-system/permissioncontroller) - APK | com。谷歌。安卓。许可控制器 | APK | 必须 | 必须 | 必须 |
| [权限控制员](https://source.android.com/devices/architecture/modular-system/permissioncontroller) - APEX | com。谷歌。安卓。许可证 | 顶点 | 必须 | 无支持的 | 无支持的 |
| [SDK 扩展](https://source.android.com/devices/architecture/modular-system/sdk-extension) | com.google.android.sdkext | 顶点 | 必须 | 无支持的 | 无支持的 |
| [Statsd](https://source.android.com/devices/architecture/modular-system/statsd) | com.google.android.os.statsd | 顶点 | 必须 | 无支持的 | 无支持的 |
| [遥测列车版本包](https://source.android.com/devices/architecture/modular-system/telemetry) | com.google.mainline .遥测技术 | APK | 必须 | 无支持的 | 无支持的 |
| [系绳](https://source.android.com/devices/architecture/modular-system/tethering) | com.google.android .网络共享 | 顶点 | 必须 | 无支持的 | 无支持的 |
| [时区数据](https://source.android.com/devices/architecture/modular-system/timezone) | com.google.android.tzdata | 顶点 | 不得 | 必须 | 可选择的 |
| 时区数据 2 | com.google.android.tzdata2 | 顶点 | 必须 | 无支持的 | 无支持的 |
| [无线网络](https://source.android.com/devices/architecture/modular-system/wifi) | com.google.android.wifi | 顶点 | 必须 | 无支持的 | 无支持的 |

为了给上面的专栏提供一些背景，标题为“升级到 Android 11 或使用 Android 11 启动的设备”的专栏包括关于该模块是否必须存在于所有已经升级到 Android 11 或开箱即用 Android 11 启动的设备上的详细信息(或在时区数据的情况下，因为包含其替代品而必须不存在)。类似地，使用 Android 10 启动的设备需要包含一些模块，强烈建议包含一些其他模块，其余的都不支持。对于升级到 Android 10 的设备(相对于用 Android 推出的)，所需模块的列表更短。

## 每个主线模块做什么？

以下是对每个主线模块的简要说明:

### Adbd

adbd 模块管理命令行 adb 和 IDE 调试会话。模块化 adbd 允许 Google 更快地提供性能改进和错误修复。这一点至关重要，因为过去的一些错误与电池耗尽有关，可能会导致设备继续使用 100%的 CPU，直到手机死机。因此，解决这些问题对谷歌来说至关重要，因为 adb 被应用开发者和原始设备制造商广泛用于测试。

### Android 神经网络 API 运行时

这是一个位于应用程序和后端驱动程序之间的库。该 API 又是 Android C API，用于在移动设备上运行计算密集型机器学习操作，并实现硬件加速的推理操作。

### 手机广播

小区广播是指紧急和非紧急警报(如黄色警报)。该模块关注与这些警报相关的任务，以及其他辅助功能，如 SMS 解码和无线紧急警报的地理围栏。

### Conscrypt

Conscrypt 模块处理 Android 的 TLS 实现和其他加密功能，如密钥生成器、cipers 和消息摘要。将它作为一个模块发布可以让谷歌加速安全改进，而不需要依赖 OTA 更新。

### DNS 解析器

顾名思义，DNS 解析器解析 DNS，即它将人类可读的 URL 转换为 IP 地址。该模块包含实现 DNS 存根解析器的代码，将其作为一个模块发布可以让 Google 为用户提供更好的保护，防止 DNS 拦截和配置更新攻击。

### 文档用户界面

文档 UI 是负责控制处理文档权限的组件对特定文件的访问的模块。正如 Google 所说，将存储访问和权限放入一个模块中可以增加最终用户的隐私和安全性，而运行时资源覆盖(RRO)功能允许 OEM 在需要时对体验进行主题化(指文件应用程序)。作为一个模块，所有 Google-Android 设备都将提供相同的文档用户界面体验。

### ExtServices

此模块包括核心操作系统功能的框架组件，如通知排名、自动填充文本匹配策略、存储缓存、包监视器和其他服务。

### IPsec/IKEv2 库

这个库模块关注与互通无线局域网(IWLAN)和 VPN 相关的新的和现有的特性，例如协商密钥、算法和隧道配置等安全参数。将这些功能模块化的想法是为了促进生态系统的一致性，并提供一种方法来快速修复安全性和互操作性问题。

这是三个分支模块，但是它们的功能相互依赖。这些媒体模块处理媒体类型和代码，与外部播放器交互，向框架展示传输控制和回放信息，优化索引元数据等。还记得改变 Android 并带来平台每月安全更新概念的漏洞吗？该漏洞利用了媒体播放库中的漏洞。因此，媒体组件的模块化允许谷歌在这个经常被攻击的组件中发现安全漏洞的情况下做出快速和广泛的反应。

这个模块的功能从它的名字就可以清楚地看出，尽管它的用途并不清楚。模块元数据模块包含....关于设备上模块列表的元数据。大概就是这样。

### 网络堆栈组件，网络堆栈权限配置，强制网络门户登录

网络堆栈组件模块提供通用 IP 服务、网络连接监控和强制登录门户检测。权限配置模块定义了允许其他模块执行网络相关任务的权限。强制网络门户登录模块处理强制网络门户，即连接到特定公共 Wi-Fi 网络时显示的网页，用户需要输入详细信息才能访问互联网。

### 许可控制器

该模块提供了可更新的隐私策略和关于授予和管理权限的 UI 元素。如果这听起来很熟悉软件包安装程序所做的事情，那是因为它确实如此。在 Android 9 之前，运行时权限授予、管理和使用跟踪等功能都是软件包安装程序的一部分。在 Android 10 中，包安装程序应用程序被分成几个部分，以便更新权限逻辑。权限控制器模块以 APK 文件的形式提供，在 Android 11 中，该模块可以自动撤销长期未使用的应用程序的运行时权限。

### SDK 扩展

这个模块有点难以理解和解释。每个 Android 版本都被分配了一个 SDK 级别(通常是其前身的+1)。当一个应用以特定的 SDK 为目标时，假设开发者已经考虑了 Android 版本带来的平台行为和 API 变化。

SDK 扩展模块决定设备的“扩展 SDK”级别，并为应用程序公开 API 以查询扩展 SDK 级别。这就是官方文件提到的全部内容。[*ArsTechnica 提到*](https://arstechnica.com/gadgets/2020/09/android-11-the-ars-technica-review/5/)*这可能是将通过 Play Store 发布的二级 API 层。*

 *### Statsd，遥测列车版本包

Statsd 负责收集设备指标。另一方面，遥测列车版本包不包含活动代码或其自身的任何功能。它只包含“遥测列车”的版本号，谷歌称这是一组度量相关的模块。根据版本号，Google Play 向最终用户显示安全补丁版本，并判断是否有度量相关模块的更新。

### 系绳

网络共享模块通过 Wi-Fi、USB、蓝牙或以太网与其他连接的客户端设备共享设备的互联网连接。该模块包括网络共享组件及其依赖项。通过使用这一网络共享模块，原始设备制造商可以依赖单一的标准参考实施，并在各种设备之间带来一致的体验。

### 时区数据

时区数据模块更新 Android 设备上的夏令时(DST)和时区，标准化数据(由于宗教、政治和地缘政治原因，数据可能会经常变化)和整个生态系统的更新机制。Android 8.1 和 Android 9 使用了基于 APK 的时区数据更新机制，Android 10 用基于 APEX 的模块更新机制取代了它。谷歌表示，AOSP 继续包括 APK 更新所需的平台代码，因此升级到 Android 10 的设备仍然可以通过 APK 接收合作伙伴提供的时区数据更新。然而，谷歌警告说，基于 APK 的更新取代了基于 APEX 的更新。

### 无线保真

这是 Wi-Fi 功能模块。最终用户现在可以在 Android 设备上获得一致的 Wi-Fi 体验，并通过模块更新修复互操作性问题，应用程序开发人员可以减少平台碎片，原始设备制造商可以满足运营商的要求，同时降低个性化定制的成本。

* * *

希望这篇文章强调了项目主线对谷歌 Android 生态系统的重要性。*