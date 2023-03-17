# XDA Mods | XDA 开发者

> 原文：<https://www.xda-developers.com/category/developments/>

[](/lenovo-smart-display-bootloader-unlock-android-apps/)

现在，您可以解锁联想智能显示器的引导加载程序，绕过 AVB，安装调试固件，并运行常规的 Android 应用程序。

谷歌试图让 Android Things——一个面向物联网(IoT)设备的高度精简的、基于 Android 的操作系统——起航的努力一直不太成功。也就是说，有一件事它非常擅长:启动谷歌助手支持的智能扬声器和显示器。然而，从改装的角度来看，这些设备远不如普通的 Android 智能手机和平板电脑。但这是 XDA，我们尽量不歧视。

[](/how-to-install-one-ui-5-samsung-emoji-root-magisk-module/)

从三星即将推出的基于 Android 13 的 One UI 5 更新中获得新的表情符号，可以在任何使用 Magisk 模块的根 Android 设备上使用。

Android 爱好者不断来到 XDA 论坛的最大原因之一是寻找新的方式来给他们的手机添加主题。幸运的是，对于没有被严重锁定的设备，你可以继续进行广泛的修改，包括那些完全来自不同 OEM Android 皮肤的修改。XDA 资深成员 [RKBD](https://forum.xda-developers.com/m/rkbd.7544065/) 也有同样的感觉，并希望增加表情符号的体验。由于他的工作，如果你有 root 权限，你现在可以在任何设备上使用三星基于 Android 13 的 One UI 5 的表情符号。

[](/magisk-25-2-release-rust-logging/)

Magisk 稳定版的最新版本(v25.2)为 MagiskInit 和 Rust-powered 日志接口提供了大量的错误修复。

回到 2021 年，我们看到了在 Android 代码库中采用内存管理的 Rust 编程语言的第一步[。吴炯，也就是 XDA 公认的高级开发人员](https://www.xda-developers.com/google-developing-android-rust/) [topjohnwu](https://forum.xda-developers.com/m/topjohnwu.4470081/) ，显然也在为 Magisk 项目考虑同样的问题。据吴介绍，Magisk 的 v25.0 版本通过稳定渠道发布后[的实验就已经开始了](https://twitter.com/topjohnwu/status/1538462758332575744)。现在，topjohnwu 以 v25.2 的形式推出了 Magisk 的新的稳定版本，整个日志记录基础设施都过渡到了 Rust。

[](/how-to-bootloader-unlock-root-magisk-nothing-phone-1/)

想根你的全新无手机 1？以下是如何解锁引导加载程序，刷新修改后的引导镜像，并安装 Magisk！

在新智能手机发布时，许多 Android 爱好者承担的一项任务是解锁引导加载程序并 [root 设备](https://www.xda-developers.com/root/)。在这之后，通常会出现大量定制 rom、内核和其他修改和调整形式的开发。可以说，在 XDA 这里，一个设备的生命并没有真正开始，直到钩环(读“锁定引导加载器”)被彻底摧毁。对于[虚无电话 1](https://www.xda-developers.com/nothing-phone-1-review/) 社区来说，这个旅程现在就可以开始了！

[](/pixel-experience-12-hands-on/)

我们花了一些时间来体验 Pixel Experience 定制 ROM 的 vanilla 和 Plus 版本，以体验所有的新功能和变化。

对于许多智能手机爱好者来说，谷歌 Pixel 设备上的软件是普通 Android 体验的缩影。与准系统的 AOSP 版本相比，它有许多难以移植到其他设备的创新功能。这就是 Pixel Experience 定制 ROM 的用武之地。

[](/asus-rog-phone-6-bootloader-unlock-tool-kernel-sources/)

华硕发布了新推出的 ROG 手机 6 系列的引导加载器解锁工具和内核源代码。请继续阅读，了解更多相关信息！

华硕的“玩家国度”(ROG)智能手机系列在手机游戏玩家中非常受欢迎。随着每一代 ROG 手机的推出，这家台湾代工企业都在不断拓展智能手机硬件的边界。最近发布的 [ROG 手机 6 系列](https://www.xda-developers.com/rog-phone-6-launch/)就是一个最好的例子，提供 6.78 英寸 165Hz AMOLED 显示屏，高通骁龙 8 Plus Gen 1 芯片组，高达 18GB 的内存，总容量为 6,000mAh 的电池，65W 快速充电，3.5 毫米耳机插孔(是的！)、众多游戏功能等等。现在，为了符合 GPL v2 的要求，并帮助售后开发社区开始构建 rom 和内核，华硕发布了官方引导加载器解锁工具和 ROG 手机 6 和 ROG 手机 6 Pro 的内核源代码。

[](/3d-pinball-for-windows-android-port/)

多亏了一个开源项目，现在可以在没有仿真的情况下在你的 Android 手机上玩 3D 弹球游戏了。

你可以在谷歌 Play 商店找到很多游戏，包括几款复古游戏。即使你最喜欢的经典游戏不在那里，你也可以选择[模拟器](https://www.xda-developers.com/aethersx2-playstation-emulator/)在你的 Android 设备上玩。为了保留经典的标题(并重温童年的记忆)，一些人进一步接受了反编译游戏代码的挑战，以便可以在现代平台上分析和玩游戏。这一次，一名开发人员将经典的 Windows 3D 弹球移植到一个可以在任何 Android 设备上工作的表单中。

[](/how-to-bootloader-unlock-root-magisk-tmobile-lg-velvet/)

你现在可以解锁 LG Velvet 的 T-Mobile 变种的引导加载程序，并使用 Magisk 进行 root。继续读下去就知道怎么做了！

解锁引导程序、[给设备找根](https://www.xda-developers.com/root/)和刷新售后光盘是 XDA 这里流行的爱好。超级用户群体非常重视修改他们设备的能力，如果他们不能解锁引导程序，他们几乎不会对手机感兴趣。许多传统设备实际上是由第三方 rom 保持活力的，这对站在失去官方支持边缘的智能手机来说也是天赐之物。例如，LG 不再生产 Android 智能手机，因此 LG 设备的所有者可能希望在不久的将来使用[定制 rom](https://www.xda-developers.com/most-popular-custom-roms-android/)。然而，由于 LG 的引导程序解锁政策，这个过程并不简单。

[](/shizuku/)

滴允许你在没有 root 用户的情况下修改你的 Android 设备。您可以在这里查看这意味着什么以及如何设置它！

Android Debug Bridge，简称 ADB，是一个方便的开发工具，可以与您的手机进行接口，用于调试和测试。通过 ADB，开发者和高级用户可以访问 Android 内置的 Linux 命令行 shell，拥有比用户安装的应用程序更大的权限。值得注意的是，ADB shell 权限并不等同于超级用户权限，因此您可能仍然需要 [root 您的设备](https://www.xda-developers.com/root/)来完全控制操作系统。但是，根据您的修改需求，shell 访问足以授予或拒绝权限、更改系统设置值以及执行更多操作。这就是滴应用程序发挥作用的地方。

[](/descendant-custom-rom-june-2022-release/)

2022 年 6 月发布的后裔定制 ROM 带来了许多新功能和对更多手机的官方支持，包括一加 7。

今年 4 月初，后裔定制 ROM 背后的团队发布了[后裔 12.1](https://www.xda-developers.com/android-12l-custom-rom-descendant-pixel-experience/)——第一个稳定的基于 Android 12L 构建的 ROM。起初，该团队为少数设备发布了 ROM，其中包括几个错误修复。此后不久，该团队发布了 5 月更新，其中包含了一系列底层更改。现在，它已经开始播种 2022 年 6 月发布的后代，支持 3 个以上的设备和几个新功能。

[](/google-pixel-now-playing-ambient-music-mod-v2-hands-on/)

环境音乐模式将谷歌 Pixel 现在播放的音乐移植到其他安卓设备上。最新版本的 mod 带来了几个新功能。

大多数人都会同意，Pixel 智能手机上的软件展示了谷歌认为 Android *应该是*的样子，因此，该软件经常受到发烧友的欢迎。尽管如此，由于专门的修改社区，你不一定要拥有一个像素设备来利用其软件功能。例如，“正在播放”功能仍然是 Pixel 系列的专属功能，但开发者 Kieron Quinn，在我们的论坛上也被称为 [Quinny899](https://forum.xda-developers.com/m/quinny899.3563640/) ，成功地将它以混合 Xposed-Magisk 模块的形式[移植到其他 Android 智能手机](https://www.xda-developers.com/google-pixel-now-playing-feature-ported/)，该模块被命名为**环境音乐模块**。现在，奎因更进一步，彻底改革了 mod，使其成为一个非根解决方案。

[](/twrp-oneplus-nord-2-motorola-moto-g40-fusion-g60-official/)

TWRP 现在正式支持一加 Nord 2，摩托罗拉 Moto G40 Fusion 和 Moto G60。继续阅读，了解更多信息！

Team Win Recovery Project(简称 TWRP)是 Android 爱好者的必备工具，他们希望在自己的设备上修补售后软件。借助这款定制恢复解决方案，您可以[刷新新的定制 rom](https://www.xda-developers.com/how-to-install-custom-rom-android/)，进行完整数据备份，修改受保护的文件，并开辟设备定制的新途径。上个月我们看到[三星 Galaxy S20 和 Note 20 获得 TWRP 官方支持](https://www.xda-developers.com/twrp-samsung-galaxy-s20-note-20-official/)。现在，三款新智能手机加入了这个名单:摩托罗拉 Moto G40 Fusion、Moto G60 和一加 Nord 2。

[](/magisk-v25-release-selinux-fix/)

Magisk (v25.0)的最新更新已经发布，包含大量的错误修复和功能改进。继续阅读，了解更多信息！

在这一点上，我们 XDA 肯定你们大多数人至少听说过 Magisk。该项目由吴炯创建，又名 XDA 认可的开发者 [topjohnwu](https://forum.xda-developers.com/m/topjohnwu.4470081/) ，该项目最初是作为一个无系统的根方法开始的，并逐渐发展成为一个更加多样化和强大的解决方案，不仅仅是一个简单的超级用户权限提供者。不言而喻，开发者和贡献者总是积极地努力完善它。Magisk 最新的重大更新，对应的是第二十五版(v25)，现在已经到了公测分支。变更日志是微妙但非常重要的，所以让我们深入了解它。

[](/lineageos-19-oneplus-9-9-pro-poco-x3-pro-mi-a1/)

一加 9、一加 9 专业版、POCO X3 专业版和小米米 A1 都有官方支持。继续阅读，了解更多信息！

自从今年 4 月初推出 ROM 以来，LineageOS 团队已经将 LineageOS 19 支持扩展到了几款设备。上个月，三星 Galaxy S10、POCO F3 和 OnePlus 5/5T 等设备获得了对基于 Android 12 的定制 ROM 的支持。自从我们之前的报道以来，该团队已经在官方构建列表中添加了四个新设备。

[](/browservio-webview-browser/)

Browservio 是一个基于 WebView 的 Android 开源浏览器，它包含了一个有趣的功能列表。继续阅读，了解更多信息！

Android 的一大优点是可以选择不同的默认浏览器。你有谷歌 Chrome 最受欢迎的选项，还有其他 Chrome 衍生的选项，如微软 Edge、Vivaldi、Brave 等等。然而，如果你有一个更便宜(或更老)的设备，你可能会发现上面的选择不令人满意，而且占用内存。

[](/lineageos-19-oneplus-5-5t-samsung-galaxy-tab-s6-lite/)

LineageOS 团队已经将 LineageOS 19 支持扩展到另外三种设备，包括 OnePlus 5、5T 和三星 Galaxy Tab S6 Lite LTE。

想给你的旧手机注入新的活力吗？厌倦了设备上陈旧的 OEM 皮肤，想要尝试新的东西？如果你有 OnePlus 5、OnePlus 5T 或三星 Galaxy Tab S6 Lite 的 LTE 版本，那么你很幸运。这些设备的所有者现在可以安装官方的 LineageOS 19 版本，这是基于 Android 12 的 LineageOS 的最新版本。

[](/basic-call-recorder-magisk-module/)

多亏了这个 Magisk 模块，你现在可以在任何运行 Android 10-13 的 Android 设备上启用通话记录功能。请继续阅读！

记录通话通常与高风险业务有关，但人们出于多种原因寻求这一功能。当你想确保在面试或商务电话中不会错过任何重要的细节，而不必手动记下事情时，电话录音机就派上了用场。然而，由于谷歌最近的打击，从 Play Store 获得第三方通话记录应用是不可行的。此外，现在很少有原始设备制造商提供本地区域无关的呼叫记录解决方案。这就是**基本通话记录器**的用武之地。

[](/lsposed/)

好奇想知道 LSPosed 吗？下面是如何通过 Magisk 安装 Riru 模块，以及您可以用 Xposed 框架的继任者做些什么。

我们过去已经讨论过 Magisk 和[的模块](https://www.xda-developers.com/best-magisk-modules/)，以及它们如何提供一个以“无系统”方式完成的修改世界。Magisk 基于覆盖的界面像 Xposed 一样越来越受欢迎，这也不无道理。除了无系统带来的所有好处之外，Magisk 还可以用于通过 [Riru](https://www.xda-developers.com/riru/) 在 [Android Zygote 进程](https://developer.android.com/topic/performance/memory-overview)的上下文中运行代码。对于一些修改者来说，这些理由足以让他们涉足所有没有系统的东西。

[](/vivo-unofficial-bootloader-unlock-x70-pro-plus/)

你现在可以非正式地解锁 Vivo X70 Pro Plus 和其他几款 Vivo 智能手机的引导程序。继续阅读，了解更多信息！

现在市场上最好的修改友好的 Android OEM 是什么？取决于你问谁这个问题，答案可能从谷歌到一加到小米，再到其他完全不同的东西。这完全没问题，因为每家公司在售后市场发展方面都有自己的优势和劣势，它们满足不同人的不同需求。但如果你想买一部价格适中的智能手机，仅仅是为了改装，Vivo 肯定不会是你的首选。

[](/realme-gt-2-pro-bootloader-unlock/)

Realme 终于为其旗舰 Realme GT 2 Pro 发布了 bootloader 解锁工具，开始了该设备的第三方开发。

Realme GT 2 Pro 是一个可笑的设备，至少可以这么说。正如属于旗舰产品类别的产品一样，Realme 已经在设备上的几乎所有东西上走了极端，给了我们迄今为止最强大的 Android 智能手机之一。这款手机配备了最新的高通骁龙 8 Gen 1 SoC，高达 12GB 的 RAM 和 512GB 的 UFS 3.1 存储，120Hz 的 QHD+ AMOLED LTPO 显示屏，据称具有 1000Hz 的触摸采样率，双立体声扬声器，50MP 索尼 IMX766 主传感器，当然，还有一个 5,000 mAh 的大容量电池，支持 65W 快速充电。现在，Realme 正在为软件部门的用户提供更多选择，因为该公司已经开放了设备上的引导加载器解锁。