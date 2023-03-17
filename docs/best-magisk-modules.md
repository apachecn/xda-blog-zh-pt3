# 最佳 Magisk 模块

> 原文：<https://www.xda-developers.com/best-magisk-modules/>

Magisk 无疑是 Android 高级用户释放设备全部潜力的最佳工具之一。Magisk 由吴炯开发，又名 XDA 资深公认开发者 [topjohnwu](https://forum.xda-developers.com/m/topjohnwu.4470081/) ，Magisk 提供了一个独特的“无系统界面”，可以用于从[给](https://www.xda-developers.com/root/)你的设备添加独特功能的一切事情。使用它的最大好处是它允许用户修改系统设置，而不需要实际修改系统文件。通过利用 Magisk 的这种基于覆盖的机制，开发人员可以以标准化的方式创建和分发现成的 mod。这种 mod 在 Android 售后改装场景中被归类为“Magisk 模块”。

Magisk 有许多模块，提供人们可以想象的各种修改。无论是删除一些预装的 OEM 应用程序，将 [PlayStation 5](https://www.xda-developers.com/sony-playstation-5-first-impressions/) 的 DualSense 控制器与您的 [Android 手机](https://www.xda-developers.com/best-android-phones/)配对，还是从 SafetyNet 中隐藏您的设备，您都可以通过安装适当的 Magisk 模块来执行各种复杂的系统级修改。

但是 Magisk 模块里面有什么呢？如何使用 Magisk 安装模块？最重要的是，有哪些最好的 Magisk 模块？

* * *

## Magisk 模块的内部结构

与许多其他文件格式不同，没有为 Magisk 模块定义唯一的扩展名。它只不过是一个[特制的 ZIP 存档](https://topjohnwu.github.io/Magisk/guides.html#magisk-modules)，保存了与相应 mod 相关的文件和元数据，如下所示。

* * *

## 如何安装 Magisk 模块

尽管具有相同的文件扩展名，但请记住，Magisk 模块与常规的可闪存 ZIP 文件完全不同。因此，你不能像一个定制的 ROM 一样引导进入恢复模式。相反，你需要使用 Magisk 应用程序或`magisk` Android 二进制程序来完成这项工作。当然，在安装模块之前，您需要[在手机上安装 Magisk](https://www.xda-developers.com/how-to-install-magisk/)。

### 使用 Magisk 应用程序安装

*   从其官方来源下载该模块。如果你是在 PC 或 Mac 上下载，那么将你的 Android 设备连接到它，并将下载的 ZIP 文件复制到目标设备的内存中。
*   打开手机上的 Magisk 应用程序，使用底部导航菜单切换到**模块**选项卡。

*   点击名为**从存储器安装**的按钮。
*   浏览并选择您先前下载的模块 ZIP。
*   Magisk 现在将安装该模块，并提示您重新启动。

*   重启后，再次打开 Magisk 应用程序，查看**模块**选项卡。您刷新的模块应该列在*已安装*部分。

### 使用“magisk”Android 二进制文件安装

*   重启手机。重启后，检查 Magisk 应用程序的**模块**标签。您刷新的模块应该列在已安装部分下。

官方的 Magisk 应用程序曾经有一个内置的集中模块库，但是为了扩大模块发现的范围，topjohnwu 决定[逐步淘汰](https://www.xda-developers.com/magisk-development-continues-without-magiskhide/)。

* * *

## 最佳 Magisk 模块

由于策划的集中式模块 repo 正逐渐从应用程序中退出，Magisk 用户最终将需要手动下载模块 ZIP 文件并自行安装。这正是本文的切入点，因为它在一个索引中汇集了一些最流行的 Magisk 模块。请随意在本文底部的评论部分添加您的评论和建议。

**注意:**在这篇文章中，我们将只涉及一小部分 Magisk 模块，这些模块正被 Android modding 社区的大部分积极使用。这并不意味着认可这些模块，也不是说应该忽视其他人的工作。请访问 Magisk 的 [XDA 分论坛，查看是否有其他(可能更通用的)模块可用。](https://forum.xda-developers.com/f/magisk.5903/)

### 0 - 9

### 1 控制器

如果您的 Android 设备不支持几种流行的游戏控制器之一，那么 1Controller Magisk 模块可以解决这个问题。该模块介绍了几种流行的游戏控制器的键盘布局文件，包括 [PS5 的 DualSense](https://www.xda-developers.com/add-playstation-5-dualsense-controller-support-root/) 、DualShock 4、DualShock 3、Xbox 360、Xbox One|One S、Xbox Series X|S 和 Switch Pro 控制器。

**1 控制人: [GitHub 回购](https://github.com/Magisk-Modules-Repo/OneController) || [XDA 讨论线程](https://forum.xda-developers.com/t/3865889/)**

* * *

### 阿-埃

### 像素器件的有效边沿模式

错过了新一代 Pixel 设备上的 Google Pixel 2 的 Active Edge 功能？感谢 XDA 公认的开发者 [mikalovtch](https://forum.xda-developers.com/m/mikalovtch.3184278/) ，你现在可以通过名为“像素设备的活动边缘模式”的模块将它带回来

**针对像素设备的 Active Edge Mod:[GitHub Repo](https://github.com/Magisk-Modules-Repo/active_edge_system_mod)| |[XDA 讨论线程](https://forum.xda-developers.com/t/4226343/)**

### 高级充电控制器

由 XDA 资深会员 [VR25](https://forum.xda-developers.com/m/vr25.5228676/) 创建的高级充电控制器是一个旨在通过限制充电电流、温度和电压来延长设备电池寿命的模块。

**高级充电控制器:[下载](https://github.com/VR-25/acc/releases)| |[GitHub Repo](https://github.com/VR-25/acc)| |[XDA 讨论线程](https://forum.xda-developers.com/t/3668427/)**

### 应用系统化

有时你想在`/system`分区中安装一个第三方应用程序来获得更多的功能。XDA 资深会员 [veez21](https://forum.xda-developers.com/m/veez21.7296895/) 的 App Systemizer 在这种情况下可以很方便，因为该模块允许安装第三方应用作为系统应用。

**App 系统化: [GitHub Repo](https://github.com/Magisk-Modules-Repo/terminal_systemizer) || [XDA 讨论线程](https://forum.xda-developers.com/t/3585851/)**

### ARCore/游乐场修补器

由 XDA 资深会员 [MarcAnt01](https://forum.xda-developers.com/m/marcant01.9262827/) 开发的 Magisk 模块，该模块使 [ARCore](https://www.xda-developers.com/arcore/) (又名用于 AR 的 Google Play 服务)支持尚未获得官方支持的设备，并允许您通过 Play Store 安装 ARCore 支持的应用程序。

**ARCore/游乐场补丁程序: [GitHub Repo](https://github.com/Magisk-Modules-Repo/ARCore_enabler) || [XDA 讨论线程](https://forum.xda-developers.com/t/3880337/)**

### 音频修改库

音频修改库本质上是音频 mods 爱好者的“瑞士军刀”。这是一个兼容性框架，允许 Magisk 安装无缝集成多个音频模块。

**音频修改库:[下载](https://zackptg5.com/android.php#aml) || [GitHub 回购](https://github.com/Zackptg5/Audio-Modification-Library) || [XDA 讨论线程](https://forum.xda-developers.com/t/3745466/)**

### 蓝牙库修补程序

根深蒂固的三星 Galaxy 用户经常在重启或飞行模式切换后失去蓝牙配对。XDA 资深会员 [3arthur6](https://forum.xda-developers.com/m/3arthur6.4259991/) 开发的蓝牙库补丁程序旨在通过动态修补三星 ROM 的蓝牙库来解决这个问题。

**蓝牙库补丁: [GitHub 回购](https://github.com/Magisk-Modules-Repo/BluetoothLibraryPatcher) || [XDA 讨论线程](https://forum.xda-developers.com/t/4017735/)**

### 安卓 NDK 的 Busybox

静态 busybox 二进制，适用于所有 Android 架构(ARM/ARM64、x86/x86_64、MIPS/MIPS64)，采用 XDA 资深公认开发者 [osm0sis](https://forum.xda-developers.com/m/osm0sis.4544860/) 的 NDK 构建。

**安卓 NDK 的 Busybox:[GitHub Repo](https://github.com/Magisk-Modules-Repo/busybox-ndk)| |[XDA 讨论线程](https://forum.xda-developers.com/posts/64228091)**

### 通话记录器- SKVALEX

XDA 资深会员 [skvalex](https://forum.xda-developers.com/m/skvalex.2859866/) 为强大的[通话记录应用](https://play.google.com/store/apps/details?id=org.skvalex.cr)配套的 Magisk 模块。该模块允许应用程序使用高级根功能，例如在较新的 Android 版本上记录双方，并在电话实际接听时开始记录。

**通话录音器- SKVALEX: [GitHub 回购](https://github.com/Magisk-Modules-Repo/callrecorder-skvalex) || [XDA 讨论线程](https://forum.xda-developers.com/t/1441643/)**

### 去涂层剂

想要摆脱大量预装的 OEM 应用程序吗？XDA 资深会员 [veez21](https://forum.xda-developers.com/m/veez21.7296895/) 的去模糊模块是满足您需求的完美解决方案。打开终端窗口，调用`debloat`命令，瞧！

**解封: [GitHub 回购](https://github.com/Magisk-Modules-Repo/terminal_debloater) || [XDA 讨论线程](https://forum.xda-developers.com/t/3584163/)**

### 分离和分离 3

使用此模块，您可以从谷歌 Play 商店自动更新过程中“分离”应用程序。它完全隐藏了“我的游戏和应用程序”部分的更新，所以你不会看到你从 Play Store 分离的应用程序等待更新。

最初的 mod 是由 XDA 资深成员 [hinxnz](https://forum.xda-developers.com/m/hinxnz.1909299/) 创建的，他现在维护着一个名为 *Detach3* 的独立分支。另一方面，常规分离模块由来自的 XDA 资深成员[维护。](https://forum.xda-developers.com/m/rom.5332893/)

**分离:[下载](https://github.com/Magisk-Modules-Repo/Detach/releases) || [GitHub 回购](https://github.com/Magisk-Modules-Repo/Detach/) || [XDA 讨论线程](https://forum.xda-developers.com/t/3447494/)**

### 禁用安全标志

如果你正在寻找一个 Magisk 模块，让你禁用 FLAG_SECURE 变量，在通常不允许的应用程序中启用截图、屏幕共享和录制，那么看看 XDA 成员 [mehedihjoy](https://forum.xda-developers.com/m/mehedihjoy.12263329/) 的创作。

**禁用旗帜安全: [XDA 讨论线程](https://forum.xda-developers.com/t/4490475/)**

### 通电保护

该模块由 XDA 资深会员 [AdroitAdorKhan](https://forum.xda-developers.com/m/adroitadorkhan.6150654/) 创建，它从多个知名来源获取服务广告、跟踪脚本和恶意软件的域列表，并创建一个主机文件来阻止您的系统连接到它们。

**通电保护: [GitHub Repo](https://github.com/Magisk-Modules-Repo/energizedprotection) || [XDA 讨论线程](https://forum.xda-developers.com/t/3806865/)**

* * *

### F - J

### 字体管理器

如果你正在寻找一种方法来改变你的 Android 设备的默认字体，给一个迷你的用户界面改头换面，或者只是想用一个更通用的表情符号来替换现有的表情符号集，不用再找了。选择 XDA 资深会员 [androidacy](https://forum.xda-developers.com/m/androidacy.9834019/) 的字体管理模块，按照你的心意定制与字体和表情符号相关的一切。

**字体管理器:[下载](https://www.androidacy.com/downloads/?fm_rdme_links=&view=%2540Magisk-Modules%2540FontManager) || [GitHub 回购](https://github.com/Androidacy/FontManager-Module/) || [XDA 讨论线程](https://forum.xda-developers.com/t/4194631/)**

### Android 10-13 的全屏/沉浸式手势调整

手势爱好者们，欢呼吧！XDA 的资深成员 [DanGLES3](https://forum.xda-developers.com/m/dangles3.8714092/) 已经想出了这个简单而聪明的模块，可以让你随心所欲地调整手势参数。

**Android 10-13 的全屏/沉浸式手势调整:[下载](https://github.com/Magisk-Modules-Alt-Repo/HideNavBar/releases)| |[GitHub Repo](https://github.com/Magisk-Modules-Alt-Repo/HideNavBar)| |[XDA 讨论线程](https://forum.xda-developers.com/t/4086493/)**

### JamesDSP 音频管理器

该模块的灵感来自 Omnirom DSPManager，它为 Android 带来了一个经过改革的音频效果数字信号处理引擎，具有增强的内部音频引擎。

**JamesDSP 音频管理器:[下载](https://zackptg5.com/android.php#jdsp) || [GitHub 回购](https://github.com/Magisk-Modules-Repo/ainur_jamesdsp) || [XDA 讨论线程](https://forum.xda-developers.com/t/jamesdsp-audio-manager-mmt-ex.3607970/)**

* * *

### K - O

### MagiskHide 道具配置

MagiskHide Props Config 是由 XDA 高级主持人和开发委员会-开发关系成员 [Didgeridoohan](https://forum.xda-developers.com/m/didgeridoohan.4667597/) 开发的，它是一个迷人的模块，可以帮助你改变设备的道具值，而无需手动修改 [Magisk `resetprop`工具](https://github.com/topjohnwu/Magisk/blob/master/docs/details.md#resetprop)。您可以无缝地修改设备指纹、型号或任何您想要的属性。在定制和未经认证的 rom 上通过 SafetyNet CTS 配置文件检查非常有用。

**magis hide 道具配置:[下载](https://github.com/Magisk-Modules-Repo/MagiskHidePropsConf/releases) || [GitHub 回购](https://github.com/Magisk-Modules-Repo/MagiskHidePropsConf/) || [XDA 讨论线程](https://forum.xda-developers.com/t/3789228/)**

对于这个特殊的模块，ZIP 包本质上是混合的。你可以使用 Magisk 应用程序安装它，也可以通过像 TWRP 这样的自定义恢复来刷新它。安装模块并重新启动后，在终端模拟器应用程序中运行命令 props，并按照说明设置所需的选项。

### 微间隙等离子体

如果你想用 microG 替换谷歌专有的 Android 用户空间应用和库，可以从下面链接的 Magisk 模块入手。它充当了最新可用的稳定的 microG 构建资产的一体化包。

**microG-Gapps: [下载](https://github.com/Psk-Ita/microG-GApps/releases) || [GitHub 回购](https://github.com/Psk-Ita/microG-GApps)**

### 纳米机器人

XDA 资深成员 Setialpha 的 NanoDroid 是各种开源软件的安装程序，最引人注目的是 microG 和 F-Droid。

**NanoDroid: [下载](https://downloads.nanolx.org/NanoDroid/)| |[GitHub Repo](https://github.com/Nanolx/NanoDroid)| |[XDA 讨论线程](https://forum.xda-developers.com/t/3584928/)**

### 诺斯托雷特里克

NoStorageRestrict 是流行的 Xposed 模块的 Magisk 模块版本，在 Android 11 及更高版本上通过文件管理器选择文件夹(Downloads/Android)时取消了限制。

**NoStorageRestrict:[GitHub Repo](https://github.com/Magisk-Modules-Alt-Repo/NoStorageRestrict)| |[XDA 讨论线程](https://forum.xda-developers.com/t/4473419/)**

### 打开字体

由 XDA 成员 [F3FFO](https://forum.xda-developers.com/m/f3ffo.9627200/) 创建的 Open Fonts 是一个漂亮的 Magisk 模块，用来替换系统字体。

**打开字体:[下载](https://github.com/Magisk-Modules-Alt-Repo/open_fonts/releases) || [GitHub 回购](https://github.com/Magisk-Modules-Alt-Repo/open_fonts) || [XDA 讨论线程](https://forum.xda-developers.com/t/4446663/)**

### 打开 WebView

如果你想用 Bromite 或者类似的 forks 替换你 Android 系统的 webview 组件，那么你应该去看看 XDA 成员 [F3FFO](https://forum.xda-developers.com/m/f3ffo.9627200/) 的 Open WebView 模块。

**打开 WebView: [下载](https://github.com/Magisk-Modules-Alt-Repo/open_webview/releases) || [GitHub 回购](https://github.com/Magisk-Modules-Alt-Repo/open_webview) || [XDA 讨论线程](https://forum.xda-developers.com/t/4496119/)**

* * *

### P - T

### 快速开关

QuickSwitch 是一个 Magisk 模块，可以在任何支持的启动器中启用 Android Pie Recents Screen(quick step)。

**快速切换:[下载](https://github.com/skittles9823/QuickSwitch/releases) || [GitHub 回购](https://github.com/skittles9823/QuickSwitch/) || [XDA 讨论线程](https://forum.xda-developers.com/t/3884797/)**

Riru 是一个强大的模块，它将自己注入到 zygote 中，以便允许其他模块在应用程序或系统服务器中运行它们的代码。

**Riru: [下载](https://github.com/RikkaApps/Riru/releases) || [GitHub 回购](https://github.com/RikkaApps/Riru/)**

许多开发人员已经编写了依赖于 Riru 的附加模块。例如， [Xposed 框架](https://www.xda-developers.com/xposed-framework-hub/)有了一个新的继任者，名为 [EdXposed](https://forum.xda-developers.com/t/4070199/) ，这是一个基于 Riru 的 Magisk 模块。由 XDA 资深成员 [kdrag0n](https://forum.xda-developers.com/m/kdrag0n.7291478/) 开发的 [Universal SafetyNet Fix](https://www.xda-developers.com/universal-safetynet-fix-update-android-12-many-oem-skins/) 是另一个基于 Riru 的 Magisk 模块的典型例子。

### TWRP A/B 保留脚本

这不是一个典型的 Magisk 模块，但这个来自 XDA 资深公认开发人员 [osm0sis](https://forum.xda-developers.com/m/osm0sis.4544860/) 的特殊脚本可以帮助在后台安装 A/B OTA 后从 Magisk 应用程序刷新时保持 TWRP 安装在两个插槽中。

**TWRP A/B 留存脚本: [GitHub 回购](https://github.com/Magisk-Modules-Repo/twrp-keep) || [XDA 讨论线程](https://forum.xda-developers.com/posts/77770683)**

* * *

### U - Z

### ViPER4Android FX

除了作为广受欢迎的 ViPER4Android 软件的下载器和伴侣之外，该模块还包括来自最初 ViPER4Android 项目的配置文件转换器和 VDC。

**ViPER4Android FX: [下载](https://zackptg5.com/android.php#viper) || [GitHub 回购](https://github.com/Magisk-Modules-Repo/ViPER4Android-FX) || [XDA 讨论线程](https://forum.xda-developers.com/t/3774651/)**

### Webview 切换器

XDA 资深会员 [androidacy](https://forum.xda-developers.com/m/androidacy.9834019/) 的 Webview Switcher 允许用户用更加隐私友好以及性能更好的 Webview 提供商替代方案来替换现有的 Android WebView。

**Webview 切换器:[下载](https://www.androidacy.com/downloads/?f=reusable&view=%2540Magisk-Modules%2540WebviewManager) || [GitHub 回购](https://github.com/Magisk-Modules-Repo/bromitewebview) || [XDA 讨论线程](https://forum.xda-developers.com/t/3936964/)**

* * *

Magisk 最初是一个业余爱好者的项目，现在已经成为 Android 改造世界中的一个完整的生态系统。一旦您的设备启动并运行 Magisk，您就可以开始添加您想要的模块。这些模块为最终用户提供的惊人的修补机会确实令人着迷。现在您已经掌握了与 Magisk 模块相关的所有东西，让我们开始修补一些最好的模块吧！一定要看看我们其他的精选列表，比如[最受欢迎的定制 rom](https://www.xda-developers.com/most-popular-custom-roms-android/)和[最受欢迎的定制内核](https://www.xda-developers.com/most-popular-custom-kernels-for-android/)。