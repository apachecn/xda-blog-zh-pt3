# 基于 Android 12 的 LineageOS 19 现已正式上市

> 原文：<https://www.xda-developers.com/lineageos-19-android-12/>

LineageOS 一直是售后 Android 开发领域的强大驱动力。作为 CyanogenMod 的继任者，该项目涵盖了数百种设备，为发烧友社区提供了一种摆脱笨重臃肿的系统的方法，并为那些拥有最少皮肤的人提供了一种修改方法。现在，LineageOS 团队正在以 Android 12 为基础，将其主要版本升级到 LineageOS 19。

## 为什么是 LineageOS 19(而不是 19.0/19.1)？

如果你看一下[我们的 Android 12 和 12L 定制 rom 列表](https://www.xda-developers.com/android-12-custom-rom/)，你可以找到对应 LineageOS 19.0 以及 19.1 的众多条目。事实上，由于明显的主要平台更新，最初的非官方版本选择了“19.0”。随后的小版本号变化是随着 Android 12L 的发布而发生的。

与此同时，谷歌转向了安卓系统的[季度维护发布模式](https://www.xda-developers.com/android-12-qpr3-beta-1/)。自然，从长远来看，LineageOS 现有的 subversion 命名法对于普通用户来说会很麻烦。由于这个原因(也为了符合 AOSP 的版本约定)，团队决定放弃 subversion 字符串。新版本被简单地称为“LineageOS 19”，尽管你仍然可以在 ROM 文件名和代码库中找到“19.1”的引用。

## LineageOS 19 中的新功能

LineageOS 19 具有大量新功能和增强功能:

*   2021 年 3 月到 2022 年 4 月的安全补丁已经合并到 LineageOS 16.0 到 19。
    *   19 builds 目前基于 android-12.1.0_r4 标签，也就是 Pixel 6 系列标签。
*   WebView 已更新至 Chromium 100.0.4896.58。
*   该团队已经完全重做了 Android 12 中引入的音量面板，而是将其变成了一个侧弹出扩展面板。
*   AOSP 画廊应用程序的分叉已经经历了大量的修复和改进。
*   更新应用程序已经看到了大量的错误修复和改进。
*   Jelly 的 LineageOS 网络浏览器已经修复了许多错误，并进行了改进。
*   该团队已经对他们不久前集成的 FOSS [Etar](https://github.com/Etar-Group/Etar-Calendar) 日历应用程序做了大量的修改和改进。
*   该团队对 [Seedvault](https://calyxinstitute.org/projects/seedvault-encrypted-backup-for-android) 备份应用程序进行了大量的更改和改进。
*   LineageOS Recorder 应用程序已经修复了许多错误，进行了改进，并增加了许多功能。
*   Android TV builds 现在附带一个无广告的 Android TV 启动器，不像谷歌的带广告的启动器。
*   Android TV builds 现在附带了一个按键处理程序，使我们能够在各种蓝牙和红外遥控器上支持自定义按键。
*   LineageOS `adb_root`服务不再依赖于构建类型属性。
*   该项目的提取实用程序现在支持从大多数类型的工厂图像/打包的 OTA 图像中提取，大大简化了设备启动和 blob 提取。
*   我们的 SDK 中增加了对高接触轮询速率的支持，允许在支持的设备上启用它。
*   AOSP Clang 工具链现在是用于编译 LineageOS 内核的默认工具链。
*   高通的骁龙相机已经被丢弃，以前使用它的设备现在将使用 Camera2。
*   现在默认启用黑暗模式。
*   有一个全新的设置向导，所有新的 Android 12 风格的图标，动画和吨新的可配置页面。
*   几乎所有应用程序都有一套全新的图标，包括系统应用程序。

除了上面提到的改进之外，LineageOS 19 和 legacy 18.1 代码库中还包含了以下更改:

*   [全新的默认壁纸，还有全套壁纸可供选择](https://www.xda-developers.com/lineageos-19-1-new-wallpapers-icons/)。这些壁纸的设计考虑到了 Android 12 的 Monet 主题化功能。
*   Wi-Fi 显示可用于所有选择加入的设备，通过高通专有接口或新恢复的传统 Miracast 接口！
*   支持不同类型充电的定制充电声音，有线或无线。

## 进一步的变化

### 网络限制

内置的防火墙、受限网络模式和每个应用程序的数据隔离功能已经过重新编写，以支持 AOSP 新的受限网络模式和 BPF (Berkeley Packet Filter)设施。此外，数据限制和网络隔离功能已经合并到一个实施中。

### iptables 上的 eBPF

AOSP 现在包括一个[扩展的 Berkeley 数据包过滤器(eBPF)](https://source.android.com/devices/architecture/kernel/bpf) 加载器和库，它在引导时加载 eBPF 程序以扩展内核功能。它本质上反对`iptables`，并且没有简单的方法将这个特性移植到遗留的 Linux 内核变体上。LineageOS 团队已经为使用 Linux 内核 4.4 的设备创建了一个功能性的后端口，但是将它移植到 3.18 或更旧的内核是一项非常繁重的工作。此外，你不能在不破坏东西的情况下在 AOSP 代码库中恢复`iptables`。

因此，对于运行 Linux 内核 3.18 及更低版本的 Android 设备，将不会有对 LineageOS 19 的官方支持，直到为这些内核版本带来 BPF 的适当变通方法。

* * *

## linea geos 19–受支持设备的官方版本

以下是 LineageOS 19 首次推出的官方构建花名册:

| 

没有。

 | 

设备和论坛链接

 | 

设备代号和维基链接

 | 

维护者

 |
| --- | --- | --- | --- |
| 1. | [华硕 ZenFone 5Z](https://forum.xda-developers.com/c/asus-zenfone-5z.7546/) | [Z01R](https://wiki.lineageos.org/devices/Z01R/) | 罗安布鲁 hit，Jackeagle，ThEMarD |
| 2. | [华硕增辉 8](https://forum.xda-developers.com/f/asus-zenfone-8.12291/) | [清酒](https://wiki.lineageos.org/devices/sake/) | 兹韦克斯，恶魔 000 |
| 3. | [F(x)tec Pro1](https://forum.xda-developers.com/c/f-x-tec-pro1.9284/) | [亲 1](https://wiki.lineageos.org/devices/pro1/) | BadDaemon、bgcngm、intervigil、mccreary、npjohnson、tdm |
| 4. | [谷歌像素 2](https://forum.xda-developers.com/c/google-pixel-2.7067/) | [沃莱](https://wiki.lineageos.org/devices/walleye/) | Eamo5 号 |
| 5. | [谷歌像素 2 XL](https://forum.xda-developers.com/c/google-pixel-2-xl.7074/) | [泰门](https://wiki.lineageos.org/devices/taimen/) | Eamo5 号 |
| 6. | [谷歌像素 3](https://forum.xda-developers.com/c/google-pixel-3.8236/) | [蓝线](https://wiki.lineageos.org/devices/blueline/) | 拉齐奥，cdesai，采访者，mikeioannina |
| 7. | [谷歌像素 3 XL](https://forum.xda-developers.com/c/google-pixel-3-xl.8243/) | [交叉剖面线](https://wiki.lineageos.org/devices/crosshatch/) | 拉齐奥，cdesai，采访者，mikeioannina |
| 8. | [谷歌像素 3a](https://forum.xda-developers.com/c/google-pixel-3a.8868/) | [中士](https://wiki.lineageos.org/devices/sargo/) | -伊甸园字幕组=-翻译 |
| 9. | [谷歌像素 3 ~ XL](https://forum.xda-developers.com/c/google-pixel-3a-xl.8875/) | [漂亮](https://wiki.lineageos.org/devices/bonito/) | -伊甸园字幕组=-翻译 |
| 10. | [谷歌像素 4](https://forum.xda-developers.com/c/google-pixel-4.9014/) | [火焰](https://wiki.lineageos.org/devices/flame/) | -伊甸园字幕组=-翻译 |
| 11. | [谷歌像素 4 XL](https://forum.xda-developers.com/c/google-pixel-4-xl.9021/) | [珊瑚](https://wiki.lineageos.org/devices/coral/) | -伊甸园字幕组=-翻译 |
| 12. | [谷歌像素 4a](https://forum.xda-developers.com/c/google-pixel-4a.10249/) | [太阳鱼](https://wiki.lineageos.org/devices/sunfish/) | 彼得生，cdesai，mikeioannina |
| 13. | [谷歌像素 4 ~ 5g](https://forum.xda-developers.com/c/google-pixel-4a-5g.11321/) | [颤抖](https://wiki.lineageos.org/devices/bramble/) | 退后，米凯伊诺娜 |
| 14. | [谷歌像素 5](https://forum.xda-developers.com/c/google-pixel-5.11335/) | [redfin](https://wiki.lineageos.org/devices/redfin/) | 退后，米凯伊诺娜 |
| 15. | [谷歌像素 5a](https://forum.xda-developers.com/f/google-pixel-5a.12359/) | [胡子](https://wiki.lineageos.org/devices/barbet/) | 退后，米凯伊诺娜 |
| 16. | [联想 Z5 Pro GT](https://forum.xda-developers.com/c/lenovo-z5-pro-gt.8479/) | [心脏](https://wiki.lineageos.org/devices/heart/) | 泰晤士报，optionaltoast |
| 17. | [联想 Z6 Pro](https://forum.xda-developers.com/c/lenovo-z6-pro.10647/) | [zippo](https://wiki.lineageos.org/devices/zippo/) | 挂锁，themard |
| 18. | [g6+摩托车](https://forum.xda-developers.com/c/moto-g6-plus.8326/) | [ever](https://wiki.lineageos.org/devices/evert/) | jleeblanchh 先生 |
| 19. | [G7 摩托车](https://forum.xda-developers.com/c/moto-g7.8523/) | [河](https://wiki.lineageos.org/devices/river/) | 发明了 no BDI，npjohnson，syberhexen |
| 20. | [G7 加](https://forum.xda-developers.com/c/moto-g7-plus.8544/)摩托车 | [湖](https://wiki.lineageos.org/devices/lake/) | jleeblanch，npjohnson |
| 21. | [G7 电源](https://forum.xda-developers.com/c/moto-g7-power.8537/) | [海洋](https://wiki.lineageos.org/devices/ocean/) | 西碧尔森，诺亚迪，npjohnson |
| 22. | [x4 摩托车](https://forum.xda-developers.com/c/moto-x4.6912/) | [佩顿](https://wiki.lineageos.org/devices/payton/) | 泰晤士河 |
| 23. | [z2 力摩托车](https://forum.xda-developers.com/c/moto-z2-force.6776/) | [nash](https://wiki.lineageos.org/devices/nash/) | npjohnson 发明的 no BDI |
| 24. | [z3 摩托车玩](https://forum.xda-developers.com/c/moto-z3-play.7789/) | [贝克汉姆](https://wiki.lineageos.org/devices/beckham/) | jleeblanchh 先生 |
| 25. | [摩托罗拉 One Action](https://forum.xda-developers.com/c/motorola-one-action.9186/) | [三驾马车](https://wiki.lineageos.org/devices/troika/) | 严格，npjohnson |
| 26. | [摩托罗拉 One Power](https://forum.xda-developers.com/c/motorola-one-power.8159/) | [厨师](https://wiki.lineageos.org/devices/chef/) | 哈萨伯 8 号 |
| 27. | [摩托罗拉 one vision/摩托罗拉 P50](https://forum.xda-developers.com/c/motorola-one-vision.8889/) | [凯恩](https://wiki.lineageos.org/devices/kane/) | 严格，npjohnson |
| 28. | [诺基亚 6.1 (2018)](https://forum.xda-developers.com/c/nokia-6-1-2018.7479/) | [PL2](https://wiki.lineageos.org/devices/PL2/) | npjohnson，自己的冲动 |
| 29. | [诺基亚 6.1 Plus](https://forum.xda-developers.com/c/nokia-6-1-plus-aka-nokia-x6.8423/) | [DRG](https://wiki.lineageos.org/devices/DRG/) | npjohnson，自己的冲动 |
| 30. | [OnePlus 6](https://forum.xda-developers.com/c/oneplus-6.7609/) | [交错](https://wiki.lineageos.org/devices/enchilada/) | 卢克 1337 |
| 31. | [OnePlus 6T](https://forum.xda-developers.com/c/oneplus-6t.8257/) | [【fajita】](https://wiki.lineageos.org/devices/fajita/) | 埃德温多克 |
| 32. | [火箭电话 2](https://forum.xda-developers.com/c/razer-phone-2.8354/) | [灵气](https://wiki.lineageos.org/devices/aura/) | 迈克约阿尼纳，npjohnson |
| 33. | [三星银河 Tab S5e (LTE)](https://forum.xda-developers.com/c/samsung-galaxy-tab-s5e.9164/) | [gts4lv](https://wiki.lineageos.org/devices/gts4lv/) | bgcngm，LuK1337 号文件 |
| 34. | [三星 Galaxy Tab S5e (Wi-Fi)](https://forum.xda-developers.com/c/samsung-galaxy-tab-s5e.9164/) | [gts4lvwifi](https://wiki.lineageos.org/devices/gts4lvwifi/) | luk 1337 bgcngm 公司 |
| 35. | SHIFT SHIFT6mq | [axoltl](https://wiki.lineageos.org/devices/axolotl/) | 黄色，乔伊 |
| 36. | [索尼体验 XA2](https://forum.xda-developers.com/c/sony-xperia-xa2.7890/) | [先驱](https://wiki.lineageos.org/devices/pioneer/) | LuK1337，严格的，cdesai |
| 37. | 索尼 Xperia XA2 增强版 | 旅行者号 | LuK1337 |
| 38. | [索尼 Xperia XA2 超](https://forum.xda-developers.com/c/sony-xa2-ultra.7523/) | [发现](https://wiki.lineageos.org/devices/discovery/) | LuK1337 |
| 39. | [索尼 Xperia 10](https://forum.xda-developers.com/c/sony-xperia-10.8651/) | [麒麟](https://wiki.lineageos.org/devices/kirin/) | LuK1337 |
| 40. | [索尼 Xperia 10 Plus](https://forum.xda-developers.com/c/sony-xperia-10-plus.8658/) | [美人鱼](https://wiki.lineageos.org/devices/mermaid/) | LuK1337 |
| 41. | [小米 POCO F1](https://forum.xda-developers.com/c/xiaomi-poco-f1.8089/) | [铍](https://wiki.lineageos.org/devices/beryllium/) | bgcngm，warabhishek |

越来越多的设备将很快过渡到 LineageOS 19，所以请关注我们的首页，因为我们将在上面刊登定期报道。

### 通用目标

就像前一年的发布一样，LineageOS 团队支持 Android 虚拟设备(AVD)，即由 [Android Studio](https://www.xda-developers.com/install-android-studio-windows-macos-linux-chrome-os/) 提供的默认仿真器环境，作为[构建目标](https://wiki.lineageos.org/emulator.html)。随着 LineageOS 19 支持 Android 汽车制造目标，这一发展也在继续。开发人员也可以在移动和 Android TV 配置中构建通用系统映像(GSI)包，尽管官方下载门户不会托管任何此类预编译版本。

### 如果我的设备没有列在这里，该怎么办？

仅仅因为你的设备没有列在这里，并不意味着你现在不能享受 LineageOS 19。由于它的开源性质，在我们的论坛上有许多设备的非官方版本，随着开发的进展，其中许多最终将成为官方版本。更重要的是:到目前为止，他们中的大多数都是非常稳定的日常司机，偶尔会有小毛病。

**[XDA 论坛](https://forum.xda-developers.com/c/lineageos.6080/)**

* * *

## 如何从旧版本升级到 LineageOS 19

如果你不熟悉安装定制 rom 或修改手机的过程，在尝试做任何事情之前，你首先需要解锁设备的引导程序，并安装一个更新的定制恢复，如 LineageOS Recovery 或 [TWRP](https://www.xda-developers.com/how-to-install-twrp/) 。然后，一旦正式的 LineageOS 19 版本可供您的设备使用，您将需要通过自定义恢复环境来安装它们。特定于设备的说明可能会有所不同，所以请提前查看相应的维基页面。

至于谷歌应用程序，它们不会预装在 LineageOS 版本中。你需要[选择一个合适的 GApps 发行版](https://www.xda-developers.com/download-google-apps-gapps/)并自己安装。

* * *

## linea geos 18.1–受支持设备的官方版本

虽然维护人员致力于将设备升级到基于 Android 12 的官方 LineageOS 19，但您仍然可以找到 LineageOS 18.1 支持的这些设备的自动构建:

### LineageOS 18.1 官方构建列表。点击/单击以展开。

| 

没有。

 | 

设备和论坛链接

 | 

设备代号和维基链接

 | 

维护者

 |
| --- | --- | --- | --- |
| 1. | [华硕 ROG 手机 3](https://forum.xda-developers.com/c/asus-rog-phone-3.11025/) | [奥比万](https://wiki.lineageos.org/devices/obiwan/) | 奥尔登克里格·阿莱斯托 |
| 2. | [华硕 ZenFone Max M1](https://forum.xda-developers.com/c/asus-zenfone-max-m1.9963/) | [X00P](https://wiki.lineageos.org/devices/X00P/) | 达纳斯卡佩 |
| 3. | [华硕 ZenFone Max M2](https://forum.xda-developers.com/c/asus-zenfone-max-m2.8472/) | [X01AD](https://wiki.lineageos.org/devices/X01AD/) | 达纳斯卡佩 |
| 4. | [华硕 ZenFone Max Pro M1](https://forum.xda-developers.com/c/asus-zenfone-max-pro-m1.7656/) | [X00TD](https://wiki.lineageos.org/devices/X00TD/) | 维韦卡乔兹 |
| 5. | [华硕 ZenFone Max Pro M2](https://forum.xda-developers.com/c/asus-zenfone-max-pro-m2.8465/) | [X01BD](https://wiki.lineageos.org/devices/X01BD/) | Rk585 |
| 6. | BQ Aquaris X | 巴多克 | eloimuns，Quallenauge，团队 aquaris-dev |
| 7. | [BQ Aquaris X Pro](https://forum.xda-developers.com/c/bq-aquaris-x-pro-x2-x2-pro.7775/) | [巴多克普罗](https://wiki.lineageos.org/devices/bardockpro/) | Quallenauge，团队水族馆-开发 |
| 8. | [Fairphone 2](https://forum.xda-developers.com/f/fairphone-2.4281/) | [FP2](https://wiki.lineageos.org/devices/FP2/) | chrmhoffmann |
| 9. | 公平电话 3 | [FP3](https://wiki.lineageos.org/devices/FP3/) | dk1978 |
| 10. | [谷歌像素](https://forum.xda-developers.com/c/google-pixel.5910/) | [旗鱼](https://wiki.lineageos.org/devices/sailfish/) | npjohnson |
| 11. | [谷歌 Pixel XL](https://forum.xda-developers.com/c/google-pixel-xl.5916/) | [马林](https://wiki.lineageos.org/devices/marlin/) | npjohnson |
| 12. | [联想 P2](https://forum.xda-developers.com/c/lenovo-p2.6149/) | [坤涛](https://wiki.lineageos.org/devices/kuntao/) | mikeioannina，公路之星 |
| 13. | [联想瑜伽 Tab 3 Plus](https://forum.xda-developers.com/c/lenovo-yoga-tab-3-plus.8972/) | LTE:[ytx 703 l](https://wiki.lineageos.org/devices/YTX703L/)Wi-Fi:[ytx 703 f](https://wiki.lineageos.org/devices/YTX703F/) | 弗拉基米尔·奥尔特安·夸勒诺格 |
| 14. | [LG G3](https://forum.xda-developers.com/c/lg-g3.3147/) | AT&T: [d850](https://wiki.lineageos.org/devices/d850/) 加拿大:[【D3】国际:](https://wiki.lineageos.org/devices/d852/)[【D5】韩国:](https://wiki.lineageos.org/devices/d855/)[【f400】](https://wiki.lineageos.org/devices/f400/)冲刺:[ls 990](https://wiki.lineageos.org/devices/ls990/)【t-mobile:[d 851】](https://wiki.lineageos.org/devices/d851/) | HardStyl3r 火鸟 11 号 |
| 15. | [摩托罗拉边](https://forum.xda-developers.com/c/motorola-edge.10491/) | [快手](https://wiki.lineageos.org/devices/racer/) | 发明了努巴迪，jleeblanch，sybilehren |
| 16. | [摩托罗拉边 S/Moto G100](https://forum.xda-developers.com/f/motorola-moto-g100-edge-s.12173/) | [不合格](https://wiki.lineageos.org/devices/nio/) | dianlujitao(地名) |
| 17. | 摩托罗拉摩托车和 5 Plus | XT 1924-3/9:【XT 1924-6/7/8:[【Hannah】](https://wiki.lineageos.org/devices/hannah)【1924-1/2/4/5:[【rhanah】](https://wiki.lineageos.org/devices/rhannah) | Jarl-Penguin，karthick111，electimon，wh0dat .你好，我是 jarl-penguin，kart hick 111，electimon，wh 0dat |
| 18. | [摩托罗拉摩托车 g5g/摩托罗拉 One 5G Ace](https://forum.xda-developers.com/c/moto-g-5g-motorola-one-5g-ace.11863/) | [基辅](https://wiki.lineageos.org/devices/kiev/) | 西波克兰，jleeblanch |
| 19. | [摩托罗拉摩托 G5 加/摩托罗拉 One 5G](https://forum.xda-developers.com/c/moto-g-5g-plus-aka-motorola-one-5g.11139/) | [奈罗](https://wiki.lineageos.org/devices/nairo/) | 西碧尔森 |
| 20. | [摩托罗拉摩托车 G5](https://forum.xda-developers.com/c/moto-g5.6203/) | [塞德里克](https://wiki.lineageos.org/devices/cedric/) | Jarl 企鹅队 |
| 21. | [摩托罗拉摩托车 G5S](https://forum.xda-developers.com/c/moto-g5s.6804/) | [蒙大拿州](https://wiki.lineageos.org/devices/montana/) | Jarl 企鹅 wiktorek140 |
| 22. | [摩托罗拉摩托车 X 2014](https://forum.xda-developers.com/c/moto-x-2014.3586/) | [胜利](https://wiki.lineageos.org/devices/victara/) | 1979 年，林肯郡，npjohnson |
| 23. | [OnePlus 9](https://forum.xda-developers.com/f/oneplus-9.12151/) | [柠檬](https://wiki.lineageos.org/devices/lemonade/) | 唐艾伯特 919 |
| 24. | [OnePlus 9 Pro](https://forum.xda-developers.com/f/oneplus-9-pro.12153/) | [柠檬派](https://wiki.lineageos.org/devices/lemonadep/) | luk 1337 bgcngm 公司 |
| 25. | [三星 Galaxy A5 (2017)](https://forum.xda-developers.com/c/samsung-galaxy-a-series-2017.6083/) | [a5 和 17lte](https://wiki.lineageos.org/devices/a5y17lte/) | 分支机构 |
| 26. | [三星 Galaxy A7 (2017)](https://forum.xda-developers.com/c/samsung-galaxy-a-series-2017.6083/) | [7a 7 和 17lte](https://wiki.lineageos.org/devices/a7y17lte/) | 分支机构 |
| 27. | [三星 Galaxy M20](https://forum.xda-developers.com/c/samsung-galaxy-m20.8714/) | [m20lte](https://wiki.lineageos.org/devices/m20lte/) | 萨姆纳-121 战斗机 |
| 28. | [三星银河笔记 3 LTE](https://forum.xda-developers.com/c/samsung-galaxy-note-3.2492/) | N9005/P: [选取](https://wiki.lineageos.org/devices/hlte/)n 9008v:[hltechn](https://wiki.lineageos.org/devices/hltechn/)n900 k/l/s:[hltek or](https://wiki.lineageos.org/devices/hltekor/)n900 t/v/w8:[hltetmo](https://wiki.lineageos.org/devices/hltetmo/) | 哈格特，npjohnson |
| 29. | [三星银河 S III Neo](https://forum.xda-developers.com/c/samsung-galaxy-s3-neo.3727/) | 双 SIM: [s3ve3gds](https://wiki.lineageos.org/devices/s3ve3gds/) 三星相机:[s3ve 3gv](https://wiki.lineageos.org/devices/s3ve3gjv/)索尼相机: [s3ve3gxx](https://wiki.lineageos.org/devices/s3ve3gxx/) | 皮顿有限公司，fcuzzocrea，Teledurak |
| 30. | 三星 Galaxy S5 主动 | [klteactivexx](https://wiki.lineageos.org/devices/klteactivexx/) | javelinanddart，npjohnson 公司 |
| 31. | [三星 Galaxy S5 LTE](https://forum.xda-developers.com/c/samsung-galaxy-s-5.2792/) | g9006 v/8v:[kltech](https://wiki.lineageos.org/devices/kltechn/)【g900 az/s 902 l】[【klteaio】](https://wiki.lineageos.org/devices/klteaio/)【g900 f/m/R4/r7/t/v/w8:[【klte】](https://wiki.lineageos.org/devices/klte/)【g900 I/p】【KLT 28】g900 k/s | 哈哥克 |
| 32. | [三星 Galaxy S10e](https://forum.xda-developers.com/c/samsung-galaxy-s10e.8763/) | [超过 0lte](https://wiki.lineageos.org/devices/beyond0lte/) | Linux4 |
| 33. | [三星 Galaxy S10](https://forum.xda-developers.com/c/samsung-galaxy-s10.8507/) | [超过 1lte](https://wiki.lineageos.org/devices/beyond1lte/) | Linux4 |
| 34. | [三星 Galaxy S10 Plus](https://forum.xda-developers.com/c/samsung-galaxy-s10.8693/) | [超过 2lte](https://wiki.lineageos.org/devices/beyond2lte/) | Linux4 |
| 35. | [三星银河 s10g](https://forum.xda-developers.com/c/samsung-galaxy-s10-5g.8861/) | [碧昂斯](https://wiki.lineageos.org/devices/beyondx/) | Linux4 |
| 36. | [索尼体验 XZ2](https://forum.xda-developers.com/c/sony-xperia-xz2.7460/) | [阿卡里](https://wiki.lineageos.org/devices/akari/) | 奥利维尔 97，sjllls |
| 37. | [索尼体验 XZ2 契约](https://forum.xda-developers.com/c/sony-xperia-xz2-compact.7467/) | [xz2c](https://wiki.lineageos.org/devices/xz2c/) | 奥利维尔 97，sjllls |
| 38. | [索尼体验 XZ2 高级](https://forum.xda-developers.com/c/sony-xperia-xz2-premium.7918/) | [极光](https://wiki.lineageos.org/devices/aurora/) | 奥利维尔 97，sjllls |
| 39. | [索尼体验 XZ3](https://forum.xda-developers.com/c/sony-xperia-xz3.8117/) | 赤子 | dtrunk90，sjllls |
| 40. | [索尼体验 Z2](https://forum.xda-developers.com/c/sony-xperia-z2.2920/) | [小天狼星](https://wiki.lineageos.org/devices/sirius/) | 阿丽亚娜 16a |
| 41. | [索尼体验 Z3](https://forum.xda-developers.com/c/sony-xperia-z3.3544/) | [z3](https://wiki.lineageos.org/devices/z3/) | 汤姆 1000，我自己 5 |
| 42. | [索尼体验 Z3 契约](https://forum.xda-developers.com/c/sony-xperia-z3-compact.3537/) | [z3c](https://wiki.lineageos.org/devices/z3c/) | 阿丽亚娜 16a |
| 43. | [小米 6](https://forum.xda-developers.com/c/xiaomi-mi-6.6331/) | [明智](https://wiki.lineageos.org/devices/sagit/) | 阿丽亚娜 16a 电刑 |
| 44. | [小米 6X](https://forum.xda-developers.com/f/xiaomi-6x-wayne-roms-kernels-recoveries-oth.8391/) | [韦恩](https://wiki.lineageos.org/devices/wayne/) | 艾萨克·陈 |
| 45. | [小米 10t/小米 10T Pro/Redmi K30S Ultra](https://forum.xda-developers.com/c/xiaomi-mi-10t-10t-pro.11621/) | [阿波罗](https://wiki.lineageos.org/devices/apollon/) | 拉姆斯基，塞瓦班图 |
| 46. | [小米 10T Lite](https://forum.xda-developers.com/c/xiaomi-mi-10t-lite.11635/) / [小米 10i](https://forum.xda-developers.com/f/xiaomi-mi-10i.12065/) /Redmi 附注 9 Pro 5G | [高更](https://wiki.lineageos.org/devices/gauguin/) | 琳恩林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林林 |
| 47. | [小米 10 Lite](https://forum.xda-developers.com/c/xiaomi-mi-10-lite.10307/) | [莫奈](https://wiki.lineageos.org/devices/monet/) | xsylla 吗 |
| 48. | [小米 A1](https://forum.xda-developers.com/c/xiaomi-mi-a1.7044/) | [织物](https://wiki.lineageos.org/devices/tissot/) | abhi inavagupta 371 |
| 49. | [小米 A2](https://forum.xda-developers.com/c/xiaomi-mi-a2-mi-6x.7963/) | [茉莉 _sprout](https://wiki.lineageos.org/devices/jasmine_sprout/) | 米凯伊诺娜 |
| 50. | [小米 Mix 2](https://forum.xda-developers.com/c/xiaomi-mi-mix-2.6931/) | [手环](https://wiki.lineageos.org/devices/chiron/) | 迈克约阿尼纳，wight554 |
| 51. | [小米笔记 3](https://forum.xda-developers.com/c/xiaomi-mi-note-3.7428/) | [杰森](https://wiki.lineageos.org/devices/jason/) | dianlujitao(地名) |
| 52. | [小米小 F2 Pro/Redmi K30 Pro/Redmi K30 Pro 缩放版](https://forum.xda-developers.com/c/xiaomi-poco-f2-pro-redmi-k30-pro.10675/) | [lmi](https://wiki.lineageos.org/devices/lmi/) | 塞瓦班图 |
| 53. | [小米短促 F3/Redmi K40/Mi 11X](https://forum.xda-developers.com/f/xiaomi-poco-f3-xiaomi-mi-11x-redmi-k40.12161/) | [alioth](https://wiki.lineageos.org/devices/alioth/) | 塞瓦班图 |
| 54. | [小米矮 m2 pro](https://forum.xda-developers.com/c/poco-m2-pro.11067/)/[【redmi 音符 9S/Redmi 音符 9 Pro](https://forum.xda-developers.com/c/redmi-note-9s-note-9-pro-indian-model.10207/) / [Redmi 音符 9 pro](https://forum.xda-developers.com/c/redmi-note-9-pro-max.10221/) | [妙极](https://wiki.lineageos.org/devices/miatoll/) | 基准 23 |
| 55. | [小米 POCO X3](https://forum.xda-developers.com/c/xiaomi-poco-x3-nfc.11523/) | [苏亚](https://wiki.lineageos.org/devices/surya/) | Subhajeetmuhuri |
| 56. | [小米 POCO X3 Pro](https://forum.xda-developers.com/f/xiaomi-poco-x3-pro.12163/) | [vayu](https://wiki.lineageos.org/devices/vayu/) | 塞鲍本图 |
| 57. | [小米红米 Note 5 Pro](https://forum.xda-developers.com/c/xiaomi-redmi-note-5-pro.7419/) | [whyred](https://wiki.lineageos.org/devices/whyred/) | 塞鲍本图·斯法里亚斯 |
| 58. | [小米红米 Note 6 Pro](https://forum.xda-developers.com/c/xiaomi-redmi-note-6-pro.8406/) | [两唇](https://wiki.lineageos.org/devices/twolip/) | DD3Boh |
| 59. | [小米红米 Note 7/7S](https://forum.xda-developers.com/c/xiaomi-redmi-note-7.8500/) | [淡紫色](https://wiki.lineageos.org/devices/lavender/) | Giovix92，UltraGamerHD |
| 60. | [小米 Redmi Note 8/8T](https://forum.xda-developers.com/c/redmi-note-8.9200/) | [银杏](https://wiki.lineageos.org/devices/ginkgo/) | 达那斯卡佩市 DarkJoker360 号 |
| 61. | [ZUK Z2 加](https://forum.xda-developers.com/c/lenovo-zuk-z2-plus.6264/) | [z2 _ 加](https://wiki.lineageos.org/devices/z2_plus/) | DD3Boh |

就像 LineageOS 19 版本一样，我们应该会看到更多的智能手机进入 LineageOS 18.1 版本。LineageOS 17.1 上的一些设备目前失去了官方支持，但我们希望新的维护者将在未来几天内介入并恢复它们。

* * *

**来源:**[linegeos 博客](https://lineageos.org/Changelog-26/)

感谢米莎尔·拉赫曼的提示！