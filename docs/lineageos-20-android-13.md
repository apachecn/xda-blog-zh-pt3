# 基于 Android 13 的 LineageOS 20 在这里，带来了新的功能和新的默认相机应用程序

> 原文：<https://www.xda-developers.com/lineageos-20-android-13/>

LineageOS 是定制 Android 开发领域的知名玩家。它是 CyanogenMod 的继任者，现在支持大量设备，为爱好者提供了一种定制和优化系统的方式，而不会被沉重的皮肤所困扰。LineageOS 团队最近发布了一个重大更新，LineageOS 20，它基于 [Android 13](https://www.xda-developers.com/android-13) 。

## LineageOS 20 中的新功能

LineageOS 20 具有许多新功能和增强功能:

*   2022 年 4 月至 2022 年 12 月的安全补丁已合并至 LineageOS 17.1 至 20。
*   LineageOS 现在有一个新的相机应用程序，名为 Aperture！它基于谷歌(主要是)令人敬畏的 [CameraX](https://developer.android.com/training/camerax) 库，并在许多设备上提供更接近“现货”的相机应用体验。非常感谢最初开发该产品的开发人员 SebaUbuntu、LuK1337 和 luca020400，以及设计师 Vazguard 和整个团队，感谢他们努力将其集成到 LineageOS 中，并使其适应我们支持的大量设备！
*   WebView 已更新至 Chromium 108.0.5359.79。
*   在 Android 13 中完全重做了音量面板，并进一步开发了侧面弹出式扩展面板。
*   完全支持[通用内核映像](https://www.xda-developers.com/google-generic-kernel-image/)和 Linux 5.10 构建，完全支持树外模块，以符合新的 AOSP 惯例。
*   AOSP 画廊应用程序的天堂分叉已经看到了许多修复和改进。
*   Updater 应用程序已经看到了许多错误修复和改进，以及一个花哨的新 Android 电视布局
*   我们的网络浏览器 Jelly 已经修复和改进了几个错误
*   更多的变化和改进回到他们不久前集成的自由软件日历应用程序的上游
*   对 [Seedvault](https://calyxinstitute.org/projects/seedvault-encrypted-backup-for-android) 备份应用程序的更多更改和改进。
*   Recorder 应用程序已经进行了调整，以适应 Android 的内置功能，同时仍然提供您所期望的 LineageOS 功能。
    *   这个应用程序被大量重组。
    *   您支持的材料已添加。
    *   高品质的录音机(WAV 格式)现在支持立体声，并有几个线程修复。

*   与谷歌支持广告的启动器不同，Android TV builds 现在附带了一个无广告的 Android TV 启动器——它还支持谷歌电视风格的构建，他们正在评估未来在受支持的设备上迁移到它。
*   多项谷歌电视功能，例如更具吸引力的双面板设置应用程序，已经移植到 LineageOS Android TV 版本中。
*   服务不再依赖于构建类型属性，这允许与许多第三方根系统的更大兼容性。
*   合并脚本在很大程度上得到了彻底改革，大大简化了 Android 安全公告的合并过程，并使像 Pixel 设备这样的支持设备更加精简。
*   LLVM 已经被完全接受，现在默认使用 LLVM 二进制工具，也可以选择使用 LLVM 集成汇编器。对于那些使用旧内核的人，不用担心，你可以随时退出。
*   已经开发了全局快速设置灯模式，以便该 UI 元素匹配设备的主题。
*   设置向导已经适应了 Android 13，有了新的风格，更无缝的过渡/用户体验。

## LineageOS 20 Aperture，一个新的默认相机应用程序

如果你曾经使用过 LineageOS 上的默认相机应用，你可能会失望。应用程序的名字“Snap”是高通自己的相机应用程序的一个分支，他们最终使用了 AOSP 默认的相机应用程序，名为 Camera2。这是一个基本的应用程序，但对于大多数人的需求来说，它太简单了。这就是光圈如此重要的原因。

Aperture 使用 CameraX API，该 API 近年来已经成熟，可以完整地用于相机应用程序。有了它，Aperture 能够实现以下功能:

*   辅助摄像头支持(设备维护人员必须启用它)
*   视频帧速率控制
*   完全控制 EIS(电子图像稳定)和 OIS(光学图像稳定)设置
*   一个水平仪来检查设备的方位角

对于外行来说，谷歌的 CameraX 库旨在简化 Android 上的相机应用程序开发过程。在引擎盖下，它包装了 Camera2，这是一个 API，允许应用程序探测设备上的相机功能，前提是 OEM 将这些相机功能暴露给 API。为了减少相机功能碎片，设备制造商可以选择在手机中附带 CameraX 兼容的扩展库，允许第三方开发人员无缝利用本机相机功能。

## LineageOS 20 建筑名册

以下是 LineageOS 20 首次推出的官方构建名单，如果你有一台这样的设备，你很快就可以安装 LineageOS 20 了。

| 

设备名称

 | 

维基网

 | 

保持器

 |
| --- | --- | --- |
| 华硕 Zenfone 5Z (ZS620KL) | [Z01R](https://wiki.lineageos.org/devices/Z01R) | rohanpurohit，Jackeagle，ThEMarD |
| 公平电话 4 | [FP4](https://wiki.lineageos.org/devices/FP4) | 米哈伊尔·奥尼娜 |
| F(x)tec Pro | [pro1](https://wiki.lineageos.org/devices/pro1) | BadDaemon、bgcngm、intervigil、mccreary、npjohnson、tdm |
| 谷歌像素 4a 5G | [荆棘](https://wiki.lineageos.org/devices/bramble) | 米哈伊尔·奥安尼娜·阿莱斯托 |
| 谷歌像素 4a | [翻车鱼](https://wiki.lineageos.org/devices/sunfish) | 彼得克西，克德赛，米凯拉尼亚 |
| 谷歌像素 4 | [火焰](https://wiki.lineageos.org/devices/flame) | -伊甸园字幕组=-翻译 |
| Google pixel 4x XL | [珊瑚](https://wiki.lineageos.org/devices/coral) | -伊甸园字幕组=-翻译 |
| Google 像素 5a | [胡子](https://wiki.lineageos.org/devices/barbet) | 退后，米凯伊诺娜 |
| Google 像素 5 | [redfin](https://wiki.lineageos.org/devices/redfin) | 退后，米凯伊诺娜 |
| Lenovo Z5 Pro GT | [心脏](https://wiki.lineageos.org/devices/heart) | 泰晤士报，optionaltoast |
| Lenovo Z6 Pro | [zippo](https://wiki.lineageos.org/devices/zippo) | 挂锁，themard |
| 摩托罗拉边缘 20 | [柏林](https://wiki.lineageos.org/devices/berlin) | npjohnson，SGCMarkus 公司 |
| 摩托罗拉边缘 30 | [迪拜](https://wiki.lineageos.org/devices/dubai) | themard，sb6596 |
| 摩托罗拉边缘公司 | [快手](https://wiki.lineageos.org/devices/racer) | 发明了努巴迪，jleeblanch，syberhexen |
| 摩托罗拉边缘 s / moto g100 | [不合格](https://wiki.lineageos.org/devices/nio) | dianlujitao(地名) |
| g 5G / one 5G ace 摩托车发动机 | [基辅](https://wiki.lineageos.org/devices/kiev) | 西波克兰，jleeblanch |
| 摩托罗拉 G5 加/one G5 | [奈罗](https://wiki.lineageos.org/devices/nairo) | 西碧尔森 |
| 摩托罗拉 g6 plus | [ever](https://wiki.lineageos.org/devices/evert) | jleeblanchh 先生 |
| 摩托罗拉 g7 游戏 | [频道](https://wiki.lineageos.org/devices/channel) | 西碧尔森，死神 96385，npjohnson 发明了 noabdi |
| 摩托罗拉 g7 plus | [湖](https://wiki.lineageos.org/devices/lake) | jleeblanch，npjohnson |
| 摩托罗拉 g7 电源 | [海洋](https://wiki.lineageos.org/devices/ocean) | 西碧尔森，诺亚迪，npjohnson |
| g7 摩托摩托摩托 | [河](https://wiki.lineageos.org/devices/river) | 发明了 no BDI，npjohnson，syberhexen |
| M4 摩托车发动机 | [佩顿](https://wiki.lineageos.org/devices/payton) | 泰晤士河 |
| 机动战士 z3 游戏 | [贝克汉姆](https://wiki.lineageos.org/devices/beckham) | jleeblanchh 先生 |
| 摩托罗拉 one power | [厨师](https://wiki.lineageos.org/devices/chef) | 哈萨伯 8 号 |
| Mini 5G 云 | [TP1803](https://wiki.lineageos.org/devices/TP1803) | 阿丽亚娜 16a，npjohnson |
| 加 5 | [芝士汉堡](https://wiki.lineageos.org/devices/cheeseburger) | 特劳塔木 |
| 加 5T | [倾销](https://wiki.lineageos.org/devices/dumpling) | 特劳塔木，国家情报局 |
| 加 6 | [交错](https://wiki.lineageos.org/devices/enchilada) | 卢克 1337 |
| 加 6T | [fajita](https://wiki.lineageos.org/devices/fajita) | 埃德温多克 |
| 加 7 | [鳄梨酱](https://wiki.lineageos.org/devices/guacamoleb) | 尚塔努-萨尔卡 |
| OnePlus 7 专业版 | [鳄梨](https://wiki.lineageos.org/devices/guacamole) | 托尔特尔卢克 1337 号 |
| 一加 7T | [hotdogb](https://wiki.lineageos.org/devices/hotdogb) | LuK1337 |
| 一加 7T 专业版 | [热狗](https://wiki.lineageos.org/devices/hotdog) | LuK1337 |
| 一加 8 | [方便面](https://wiki.lineageos.org/devices/instantnoodle) | 贾巴什克 |
| 一加 8 专业版 | [instantnoodlep](https://wiki.lineageos.org/devices/instantnoodlep) | LuK1337 |
| 一加 8T | [烤肉串](https://wiki.lineageos.org/devices/kebab) | LuK1337 |
| 一加 9 | [柠檬水](https://wiki.lineageos.org/devices/lemonade) | ZVNexus 唐阿尔伯 919 号 mikeioannina |
| 一加 9 专业版 | [莱蒙得普](https://wiki.lineageos.org/devices/lemonadep) | mikeioannina |
| 雷蛇手机 2 | [光环](https://wiki.lineageos.org/devices/aura) | npjohnson 的 mikeioannina |
| 三星 Galaxy Tab S5e (LTE) | [gts4lv](https://wiki.lineageos.org/devices/gts4lv) | bgcngm，LuK1337 |
| 三星 Galaxy Tab S5e (Wi-Fi) | [gts4lvwifi](https://wiki.lineageos.org/devices/gts4lvwifi) | LuK1337，bgcngm |
| 索尼 Xperia 1 II | [pdx203](https://wiki.lineageos.org/devices/pdx203) | hellobbn |
| 小米 Mi 8 | [铲斗](https://wiki.lineageos.org/devices/dipper) | infrag |
| 小米 Mi 8 探索者版 | [大熊星座](https://wiki.lineageos.org/devices/ursa) | bgcngm |
| 小米 Mi 8 Pro | [小马驹](https://wiki.lineageos.org/devices/equuleus) | bgcngm |
| 小米 Mi 8 SE | [xmsirius](https://wiki.lineageos.org/devices/xmsirius) | uixdess |
| 小米 Mi 9 SE | [格鲁什](https://wiki.lineageos.org/devices/grus) | 塞鲍本图 |
| 小米 Mi CC 9 / Mi 9 Lite | [pyxis](https://wiki.lineageos.org/devices/pyxis) | 塞拉茨 |
| 小米 Mi MIX 2S | [北极星](https://wiki.lineageos.org/devices/polaris) | bgcngm |
| 小米 Poco F1 | [铍](https://wiki.lineageos.org/devices/beryllium) | bgcngm，warabhishek |

### 通用目标

就像前几个版本一样，LineageOS 团队支持 Android 虚拟设备(AVD)，即由 [Android Studio](https://www.xda-developers.com/install-android-studio-windows-macos-linux-chrome-os/) 提供的默认仿真器环境，作为[构建目标](https://wiki.lineageos.org/emulator.html)。LineageOS 19 还增加了对 Android 汽车构建目标的支持。开发人员也可以在移动和 Android TV 配置中构建通用系统映像(GSI)包，尽管官方下载门户不会托管任何此类预编译版本。这是因为它依赖于原始设备制造商遵守(或不遵守)Treble 要求的程度。

### 如果我的设备没有列在这里，该怎么办？

仅仅因为你的设备没有列在这里并不意味着你现在不能享受 LineageOS 20。由于它的开源性质，我们的论坛上有许多设备的非官方版本，随着开发的进展，其中许多最终将成为官方版本。更重要的是:到目前为止，他们中的大多数都是非常稳定的日常司机，偶尔会有小毛病。

## 如何从旧版本升级到 LineageOS 20

如果你不熟悉安装定制 rom 或修改手机的过程，在尝试做任何事情之前，你首先需要解锁设备的引导加载程序并安装更新的定制恢复，如 LineageOS Recovery 或 [TWRP](https://www.xda-developers.com/how-to-install-twrp/) 。然后，一旦正式的 LineageOS 20 版本可以用于您的设备，您将需要通过定制的恢复环境来安装它们。设备特定的说明可能会有所不同，所以[提前查看你的设备](https://wiki.lineageos.org/upgrade_guides)的相应维基。

至于谷歌应用程序，它们不会预装在 LineageOS 版本中。你需要[选择一个合适的 GApps 发行版](https://www.xda-developers.com/download-google-apps-gapps/)并自己安装。

* * *

**来源:**[linegeos 博客](https://lineageos.org/Changelog-27/)