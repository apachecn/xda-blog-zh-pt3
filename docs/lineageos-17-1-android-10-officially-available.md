# 基于 Android 10 的 LineageOS 17.1 现已正式上市

> 原文：<https://www.xda-developers.com/lineageos-17-1-android-10-officially-available/>

如果你自称是一个定制 ROM 的老手，你肯定听说过 LineageOS。LineageOS 的根源可以追溯到 CyanogenMod，这是一款在 HTC Dream/T-Mobile G1 上流行的定制 ROM，是第一款可供购买的 Android 智能手机。反过来，CyanogenMod 继续成为众多设备中最受欢迎的定制 rom 之一，当 [Cyanogen 决定停止支持 CyanogenMod](https://www.xda-developers.com/the-death-of-cyangenmod-and-whats-in-store-for-the-future/) 时，该项目的几个关键开发者和维护者[继续建立 linegeos](https://www.xda-developers.com/xda-forums-dedicated-to-lineage-os-now-live/)。随着 LineageOS 13.0 和 LineageOS 14.1 的发布，LineageOS [接手了这个项目](https://lineageos.org/Update-and-Build-Prep/)，这个项目已经持续了很多年。现在，LineageOS 正在以 Android 10 为基础将主要版本升级到 LineageOS 17.1 。

**[XDA 论坛](https://forum.xda-developers.com/lineage)**

## 为什么是血统 17.1 而不是 17.0？

Android 10 的源代码[于 2019 年 9 月到达 AOSP](https://www.xda-developers.com/android-10-source-code-aosp/)，LineageOS 团队一直在努力工作，将他们的 ROM 及其功能带到新的 Android 版本基础上。不过，AOSP 在某些领域进行了大规模的重构，这使得移植花费的时间比预期的要长。AOSP 还引入了新的[权限中心](https://www.xda-developers.com/android-q-dark-theme-desktop-mode-permission-revamp/)等功能，这与定制 ROM 的隐私保护功能[相冲突，迫使他们放弃了它](https://www.xda-developers.com/lineageos-dropping-superuser-addonsu-implementation-favor-magisk-manager/)。这两个变化意味着团队必须更加努力，花费更多的时间将 ROM 作为一个整体引入 Android 10。

与此同时，谷歌发布了[2019 年 12 月 Android 安全公告，LineageOS 团队决定重新基于功能更丰富的谷歌 AOSP Pixel 4/4XL 标签。因此，团队也决定从 17.0 升级到 17.1。对于未来，如果在不同的标签上进行任何大规模的重新排序，团队将会跳到 subversion number 上。](https://www.xda-developers.com/december-2019-android-security-patches/)

作为这一跳跃的结果，团队将锁定所有血统-17.0 分支对其 Gerrit 的贡献，并放弃现有的 17.0 更改。尽管如此，开发者仍然可以自由选择 17.1 的修改。

* * *

## 管理和维护变更

升级到官方的 LineageOS 17.1 意味着大多数当前的构建资源将集中在为支持的设备构建这些新的更新上。这具有从旧版本转移资源的预期副作用。随着 17.1 分支达到与 16.0 相当的功能和稳定性，它将成为最新和最积极开发的分支，从 2020 年 1 月 31 日开始为支持的设备定期进行夜间构建。因此，16.0 将被转移到每周构建中，而 [15.1 将从自动构建中弃用](https://review.lineageos.org/c/LineageOS/lineage_wiki/+/265767)。

LineageOS 17.1 将推出针对一小部分设备的构建，随着更多设备的到来，它们将被标记为符合[宪章](https://wiki.lineageos.org/submitting_device.html)，并准备好由其维护者进行构建。

沿袭团队也将重点放在了他们的维基更新上。[linegeos Wiki](https://wiki.lineageos.org/)最近进行了扩展，设备维护人员获得了更多选项来定制他们设备的单独安装、更新和升级说明。从 LineageOS 17.1 开始，维护人员需要在他们的设备 wiki 上运行完整的说明，并验证这些信息是否适用于他们的设备。对 wiki 的这种重新关注是根据对 AOSP 的不断增加的改变，例如 System-As-Root、A/B 分区方案和[动态分区](https://www.xda-developers.com/android-q-dynamic-system-updates-project-treble/)，它们的综合效果是废弃了我们许多人多年来凭记忆遵循的指令——那些指令现在要么不再有效，要么缺少非常关键的步骤。例如，Heimdall(三星闪存工具)说明已经过时，所以[已经更新](https://review.lineageos.org/c/LineageOS/lineage_wiki/+/267527)以反映新信息。因此，如果你想升级到 LineageOS 17.1 或者只是对定制 rom 感兴趣，查看你的设备的维基页面仍然是一个好主意。

* * *

## LineageOS 17.1 中的新功能

LineageOS 17.1 为 ROM 系列带来了几个新特性:

*   新的部分截屏用户界面，让您手动选择屏幕的较小部分，并编辑截屏。
*   新改编自 AOSP 的 ThemePicker 应用程序，支持常见的口音、字体变化、图标(快速设置和启动器)形状和图标资源变化(如改变 Wi-Fi/蓝牙图标的形状)。
*   使用指纹传感器隐藏和保护投石机发射器内的应用程序
*   合并 2019 年 10 月、11 月、12 月、2020 年 1 月、2020 年 2 月、2020 年 3 月的安全补丁。
*   Wi-Fi 显示再次可用。
*   增加了对屏幕指纹传感器(FOD)的支持。
*   增加了对弹出式和旋转摄像机的支持。
*   WebView 已更新至 Chromium 80.0.3987.132。
*   ROM 目前基于 AOSP 的 android-10.0.0_r31 标签，也就是 Pixel 4/4 XL 的标签。

* * *

## 进一步的变化

### 血统恢复

Lineage 也将 Lineage Recovery 作为安装 LineageOS 的实际解决方案。默认情况下，将为所有官方支持的设备构建沿袭恢复。该团队提到，这一变化纯粹是为了简化他们自己的流程，而不是劝阻用户放弃其他自定义恢复。设备维护者保留在其设备的 Wiki 页面上推荐替代恢复的自由，并附有完整的使用说明。

### AOSP 的许可中心和 LineageOS 的隐私卫士

过去我们已经[讨论过这个变化，现在变化终于来了。LineageOS 17.1 放弃了对自制 PrivacyGuard 实现的支持，转而支持](https://www.xda-developers.com/lineageos-dropping-superuser-addonsu-implementation-favor-magisk-manager/) [AOSP 的权限中心](https://www.xda-developers.com/android-q-dark-theme-desktop-mode-permission-revamp/)，因为该团队无法将 PrivacyGuard 框架移植到 Android 10。谷歌没有在 Android 10 中发布权限中心，但它的代码仍然存在于 AOSP。因此，Lineage 团队对其进行了分支，并将其作为解决方案，因为它据称在功能上几乎相同，但在与 PrivacyGuard 共存的尝试中存在冲突。

### 无附加二进制支持

作为移除 PrivacyGuard 和切换到 Permission Hub 的副产品，通常作为简单的根访问解决方案提供的 addonsu 二进制文件不再可行，[正如我们在](https://www.xda-developers.com/lineageos-dropping-superuser-addonsu-implementation-favor-magisk-manager/)之前所告知的。对 root 感兴趣的用户可以选择使用 ADB root 或 flash 兼容的第三方解决方案，如 Magisk。该团队澄清说，这并不意味着任何特定的第三方解决方案被认可为官方支持——因此您仍然需要注意与您的 ROM 和谐工作的根解决方案。

### 样式 API 的弃用

样式 API 现在也被弃用，取而代之的是 AOSP 的 ThemePicker 应用。该团队声称与 ThemePicker 完全功能对等，甚至功能优越。

* * *

## LineageOS 17.1 的升级说明

如果您使用的是官方 LineageOS 16，并且您的设备出现在 LineageOS 17.1 官方支持的设备列表中，您仍需要按照设备特定 wiki 页面上的说明手动更新您的设备。LineageOS updater 应用程序一般不支持从 LineageOS 的一个版本升级到另一个版本，因此用户必须有意识地决定更新，而不是被 OTA 吓一跳。

特定于设备的指令可能会有所不同，但对于我们检查的大多数设备，更新指令依赖于使用 *adb reboot sideload* 命令，然后使用 *adb sideload /"filepath"* 命令。Lineage 团队还提到，官方发布渠道版本中的更新不需要用户擦除他们的设备；但是从非官方版本转移到官方版本将需要从恢复中擦除设备。

您很可能能够通过自定义的第三方恢复来安装 LineageOS，但这不是开发人员推荐的升级方法，因此您的收益可能会因设备而异。请务必查看您设备的 wiki、其支持页面和我们自己的论坛，以确保您遵循正确的方法进行升级，从而避免任何问题。

你还应该注意，你的 ROM 安装将不包括谷歌应用，原因很简单，这些应用是专有的。你需要下载一个单独的 GApps 包，优先选择你的设备维护者/开发者推荐的 GApps 包，原因[我们会在单独的 PSA](https://www.xda-developers.com/gapps-package-recommended-rom-developer/) 中解释。顺便说一下，[Open gapp 最近也发布了他们官方的 Android 10 flashable 包](https://www.xda-developers.com/open-gapps-android-10-roms/)。

正如我们在前面的段落中解释的那样，您的 ROM 也不会附带默认的根解决方案。您需要单独刷新第三方解决方案。

* * *

## LineageOS 17.1 -受支持设备的官方版本

以下是 LineageOS 17.1 首次展示的第一批正式构建花名册:

| 

设备和论坛链接

 | 

设备代号和维基链接

 | 

维护者

 |
| --- | --- | --- |
| [华硕 Zenfone 6](https://forum.xda-developers.com/zenfone-6-2019) (ZS630KL) | [I01WD](https://wiki.lineageos.org/devices/I01WD) | 奥登克里格·卢卡 020400 |
| [BQ 水族箱 X](https://forum.xda-developers.com/aquaris-x-pro) | [巴多克](https://wiki.lineageos.org/devices/bardock) | eloimuns，Quallenauge，团队 aquaris-dev |
| [BQ Aquaris X Pro](https://forum.xda-developers.com/aquaris-x-pro) | [巴多克普罗](https://wiki.lineageos.org/devices/bardockpro) | Quallenauge，团队水族馆-开发 |
| [Fairphone FP2](https://forum.xda-developers.com/fairphone-2) | [FP2](https://wiki.lineageos.org/devices/FP2) | chrmhoffman |
| [谷歌 Nexus 6](https://forum.xda-developers.com/nexus-6) | [沙木](https://wiki.lineageos.org/devices/shamu) | npjohnson 公司 Elektroschmock |
| [谷歌像素](https://forum.xda-developers.com/pixel) | [赛菲尔什](https://wiki.lineageos.org/devices/sailfish) | 干预主义者，拉扎勒斯 |
| [谷歌像素 XL](https://forum.xda-developers.com/pixel-xl) | [马林](https://wiki.lineageos.org/devices/marlin) | 干预主义者，拉扎勒斯 |
| [HTC One 2014](https://forum.xda-developers.com/htc-one-m8) | [m8](https://wiki.lineageos.org/devices/m8) | bgcngm 公司 |
| [HTC One 2014 双 SIM](https://forum.xda-developers.com/htc-one-m8) | [m8d](https://wiki.lineageos.org/devices/m8d) | bgcngm 公司 |
| [LG G2(at & 【t】t17】](https://forum.xda-developers.com/att-g2) | [d800](https://wiki.lineageos.org/devices/d800) | 学名:Kapricomus,Arnau,YoDevil |
| [LG G2 (T-Mobile)](https://forum.xda-developers.com/tmobile-g2) | [【D1】](https://wiki.lineageos.org/devices/d801) | 学名:Kapricomus,Arnau,YoDevil |
| [LG G2(国际)](https://forum.xda-developers.com/lg-g2) | [d202](https://wiki.lineageos.org/devices/d802) | 学名:Kapricomus,Arnau,YoDevil |
| [LG G2(加拿大)](https://forum.xda-developers.com/lg-g2) | [D3](https://wiki.lineageos.org/devices/d803) | 学名:Kapricomus,Arnau,YoDevil |
| [LG G3 (AT &T)](https://forum.xda-developers.com/att-lg-g3) | [d850(T19)](https://wiki.lineageos.org/devices/d850) | 火鸟 11 号 HardStyl3r |
| [LG G3(加拿大)](https://forum.xda-developers.com/lg-g3) | [d852](https://wiki.lineageos.org/devices/d852) | 火鸟 11 号 HardStyl3r |
| [LG G3(国际)](https://forum.xda-developers.com/lg-g3) | [d855](https://wiki.lineageos.org/devices/d855) | 火鸟 11 号 HardStyl3r |
| [LG G3(韩国)](https://forum.xda-developers.com/lg-g3) | [F400](https://wiki.lineageos.org/devices/f400) | 火鸟 11 号 HardStyl3r |
| LG G3 (T-Mobile) (T27) | [d851](https://wiki.lineageos.org/devices/d851) | 火鸟 11 号 HardStyl3r |
| LG G3 (Verizon) (T31) | [vs985(T33)](https://wiki.lineageos.org/devices/vs985) | 火鸟 11 号 HardStyl3r |
| [【LG G5(全球)](https://forum.xda-developers.com/lg-g5) | [rs988](https://wiki.lineageos.org/devices/rs988) | npjohnson 先生 |
| [LG G5(国际)](https://forum.xda-developers.com/lg-g5) | [h850](https://wiki.lineageos.org/devices/h850) | npjohnson 先生 |
| LG G5 (T-Mobile) (T39) | (T40) h830 (T41) | npjohnson 先生 |
| [【LG v20(at & 【t】t69】](https://forum.xda-developers.com/v20) 】 | (T44) H910 (T45) | npjohnson 先生 |
| [LG V20(全球)](https://forum.xda-developers.com/v20) | (T46) h990 (T47) | npjohnson 先生 |
| [LG V20(冲刺)](https://forum.xda-developers.com/v20) | [ls997](https://wiki.lineageos.org/devices/ls997) | npjohnson 先生 |
| [LG V20(T-Mobile)](https://forum.xda-developers.com/v20) | (T52) h918 (T53) | npjohnson 先生 |
| [LG V20(美国解锁)](https://forum.xda-developers.com/v20) | [美国 996](https://wiki.lineageos.org/devices/us996) | npjohnson 先生 |
| LG V20 (Verizon) (T55) | (T56) vs995 (T57) | npjohnson 先生 |
| [摩托罗拉摩托车 Z](https://forum.xda-developers.com/moto-z) | [格里芬](https://wiki.lineageos.org/devices/griffin) | DD3Boh 发明了 noabdi SHR 3ps stargo 牛 |
| [摩托罗拉摩托车 g6 plus(XT 1926-2/3/5/6/7/8/9)](https://forum.xda-developers.com/g6-plus) | (T58) Ever (T59) | jleeblanchh 先生 |
| [摩托罗拉摩托车 G7](https://forum.xda-developers.com/moto-g7) | [河](https://wiki.lineageos.org/devices/river) | 发明了 nolen、Nolen Johnson (npjohnson)、syberhexen |
| [摩托罗拉摩托车 G7 Plus (XT1965-2/3/6)](https://forum.xda-developers.com/g7-plus) | [湖](https://wiki.lineageos.org/devices/lake) | jleeblanchh 先生 |
| [摩托罗拉摩托车 X4](https://forum.xda-developers.com/moto-x4) | [佩顿](https://wiki.lineageos.org/devices/payton) | 发明了 no BDI |
| [摩托罗拉摩托车 Z2 力](https://forum.xda-developers.com/z2-force) | [纳什(T61)](https://wiki.lineageos.org/devices/nash) | npjohnson 发明的 no BDI |
| [摩托罗拉单功率(XT1942-1/2)](https://forum.xda-developers.com/one-power) | [厨师](https://wiki.lineageos.org/devices/chef) | 哈萨伯 8 号 |
| 一加 3/3T(T63) | (T64) oneplus3 (T65) | dianlujitao(地名) |
| 型号: OnePlus 6 (T67) | [交错](https://wiki.lineageos.org/devices/enchilada) | 卢卡 020400，卢克 1337 |
| [OnePlus 6T](https://forum.xda-developers.com/oneplus-6t) 中 | [Fafita(T69)](https://wiki.lineageos.org/devices/fajita) | 卢克 1337 |
| OnePlus 7 Pro(T71) | [鳄梨](https://wiki.lineageos.org/devices/guacamole) | 卢克 1337 号派特尔 |
| [火箭电话](https://forum.xda-developers.com/razer-phone) | [谢丽尔](https://wiki.lineageos.org/devices/cheryl) | 米凯伊诺娜 |
| [三星 Galaxy S4 有源(GT-I9295)](https://forum.xda-developers.com/galaxy-s4-active) | [吹牛](https://wiki.lineageos.org/devices/jactivelte) | 弓，npjohnson，侧面 |
| [三星 Galaxy S4 (SGH-I337)](https://forum.xda-developers.com/galaxy-s4) | (T72) jtexttt (T73) | 弓，npjohnson，侧面 |
| [三星 Galaxy S4 (SCH-R970/C/X，SPH-L720)](https://forum.xda-developers.com/galaxy-s4) | [【JTF PR】](https://wiki.lineageos.org/devices/jfltespr) | 弓，npjohnson，侧面 |
| [三星 galaxy S4 value edition(gt-I 9515/l)](https://forum.xda-developers.com/galaxy-s4) | (T76) jfvelte (T77) | 阿科，约翰逊，这边 |
| [三星 Galaxy S4 (SCH-I545)](https://forum.xda-developers.com/galaxy-s4) | (T78) jfltevzw (T79) | 阿科，约翰逊，这边 |
| [三星 Galaxy S4 (GT-I9505/G，SGH-I337M，SGH-M919)](https://forum.xda-developers.com/galaxy-s4) | [jfltexx (T81)](https://wiki.lineageos.org/devices/jfltexx) | 阿科，约翰逊，这边 |
| [三星 Galaxy Tab S5e](https://forum.xda-developers.com/tab-s5e) Wi-Fi (SM-T720) | [gts4lvwifi (T83)](https://wiki.lineageos.org/devices/gts4lvwifi) | bgcngm,LuK1337 |
| [索尼 Xperia 10](https://forum.xda-developers.com/xperia-10) | [麒麟](https://wiki.lineageos.org/devices/kirin) | 卢克 1337 |
| [索尼 Xperia 10 Plus](https://forum.xda-developers.com/10-plus) | [美人鱼](https://wiki.lineageos.org/devices/mermaid) | 卢克 1337 |
| [索尼 Xperia XA2](https://forum.xda-developers.com/xperia-xa2) | [先锋](https://wiki.lineageos.org/devices/pioneer) | cdesai，LuK1337，严格 |
| [索尼 Xperia XA2 超](https://forum.xda-developers.com/xa2-ultra) | [发现](https://wiki.lineageos.org/devices/discovery) | 卢克 1337 |
| [小米米 6](https://forum.xda-developers.com/mi-6) | [萨吉特](https://wiki.lineageos.org/devices/sagit) | 艾丽安克·特罗斯克·16a |
| [小米米 8](https://forum.xda-developers.com/mi-8) | [铲斗](https://wiki.lineageos.org/devices/dipper) | infrag |
| [小米米 Mix 2](https://forum.xda-developers.com/mi-mix-2) | [凯龙](https://wiki.lineageos.org/devices/chiron) | mikeioannina，重量 554 |
| [小米米 Mix 2S](https://forum.xda-developers.com/xiaomi-mi-mix-2s) | [北极星](https://wiki.lineageos.org/devices/polaris) | bgcngm |
| [小米 POCO F1](https://forum.xda-developers.com/poco-f1) | [铍](https://wiki.lineageos.org/devices/beryllium) | bgcngm, warabhishek |
| [联想 ZUK Z2 Plus](https://forum.xda-developers.com/lenovo-zuk-z2) | [z2 _ 加](https://wiki.lineageos.org/devices/z2_plus) | DD3Boh |

越来越多的设备将很快过渡到 LineageOS 17.1，所以请关注我们的首页，因为我们将在上面刊登定期报道。

* * *

## LineageOS 16.0 分支中的新功能

除了最新的分支，较老的 LineageOS 16.0 分支也有一些重大变化:

*   Wi-Fi 显示再次可用。
*   您现在可以通过设备的 VPN 路由热点连接。
*   增加了对屏幕指纹传感器(FOD)的支持。
*   增加了对弹出式和旋转摄像机的支持。
*   合并 2019 年 7 月、8 月、9 月、10 月、11 月、12 月、2020 年 1 月、2020 年 2 月、2020 年 3 月的安全补丁。
*   WebView 已更新至 Chromium 80.0.3987.132。
*   现在可以在 macOS 上编译 LineageOS 16.0 了。

* * *

## linegeos 16-受支持设备的官方版本

虽然维护人员正在努力将设备升级到基于 Android 10 的官方 LineageOS 17.1，但您仍然可以找到 LineageOS 16 支持的这些设备的每周自动版本:

### LineageOS 16 官方建造清单。点击/单击以展开。

| 

设备和论坛链接

 | 

设备代号和维基链接

 | 

维护者

 |
| --- | --- | --- |
| [华硕 ZenFone 3](https://forum.xda-developers.com/zenfone-3) (ZE520KL，ZE552KL) | zenfone 3 | 麦坤 645 |
| [华硕 Zenfone Max Pro M1](https://forum.xda-developers.com/asus-zenfone-max-pro-m1) | [X00TD](https://wiki.lineageos.org/devices/X00TD) | 萨加尔马哈尔 |
| [华硕 Zenfone Max Pro M2](https://forum.xda-developers.com/max-pro-m2) | [X01BD](https://wiki.lineageos.org/devices/X01BD) | kubersharma 001 战斗机 |
| [BQ 水族箱 X](https://forum.xda-developers.com/aquaris-x-pro) | [巴多克](https://wiki.lineageos.org/devices/bardock) | eloimuns，Quallenauge，团队 aquaris-dev |
| [【bq aquaris x pro】](https://forum.xda-developers.com/aquaris-x-pro) | [巴多克普罗](https://wiki.lineageos.org/devices/bardockpro) | Quallenauge，团队水族馆-开发 |
| X2 水族馆 | [藏雅](https://wiki.lineageos.org/devices/zangya) | eloimuns，Kra1o5，团队 aquaris-dev |
| [BQ 宝瓶 X2 Pro](https://forum.xda-developers.com/aquaris-x-pro) | [藏雅罗](https://wiki.lineageos.org/devices/zangyapro) | eloimuns，Kra1o5，团队 aquaris-dev |
| [基本 PH-1](https://forum.xda-developers.com/essential-phone) | [马塔](https://wiki.lineageos.org/devices/mata) | haggertk，采访者，jrior 001，rashed |
| [【fairphone 2】](https://forum.xda-developers.com/fairphone-2) | [fp2](https://wiki.lineageos.org/devices/FP2) | 克里斯莫夫曼 |
| [谷歌 Nexus 6](https://forum.xda-developers.com/nexus-6) | [沙木](https://wiki.lineageos.org/devices/shamu) | npjohnson 公司 Elektroschmock |
| [谷歌像素](https://forum.xda-developers.com/pixel) | [旗鱼](https://wiki.lineageos.org/devices/sailfish) | 采访，razorloves |
| [谷歌 Pixel XL](https://forum.xda-developers.com/pixel-xl) | [马林](https://wiki.lineageos.org/devices/marlin) | 采访，razorloves |
| [纪念 5X](https://forum.xda-developers.com/honor-5x) | [猕猴桃](https://wiki.lineageos.org/devices/kiwi) | 巴德戴蒙、多博、乔尔赫 |
| [荣誉观 10](https://forum.xda-developers.com/honor-view-10) | [伯克利](https://wiki.lineageos.org/devices/berkeley) | 卢克 1337 |
| [华为 P20 Pro](https://forum.xda-developers.com/huawei-p20-pro) | [夏洛特](https://wiki.lineageos.org/devices/charlotte) | 卢克 1337 |
| [乐视乐 2](https://forum.xda-developers.com/le-2) | [s2](https://wiki.lineageos.org/devices/s2) | 代号 orkx，Rk585 |
| [LeEco 乐 Max2](https://forum.xda-developers.com/le-max-2) | [x2](https://wiki.lineageos.org/devices/x2) | 特尔泰尔，ThEMarD |
| [LeEco Le Pro3/Le Pro3 精英](https://forum.xda-developers.com/le-pro3) | [zl1](https://wiki.lineageos.org/devices/zl1) | 代号 orkx |
| [联想 P2](https://forum.xda-developers.com/lenovo-p2) | [昆陶](https://wiki.lineageos.org/devices/kuntao) | mikeioannina，高速公路司机 |
| [联想瑜伽 Tab 3 Plus](https://forum.xda-developers.com/yoga-tab-3-plus) | [YTX703F](https://wiki.lineageos.org/devices/YTX703F) | 水母，海参崴 |
| [联想瑜伽 Tab 3 Plus LTE](https://forum.xda-developers.com/yoga-tab-3-plus) | [YTX703L](https://wiki.lineageos.org/devices/YTX703L) | 水母，海参崴 |
| [联想 ZUK Z1](https://forum.xda-developers.com/zuk-z1) | [ham](https://wiki.lineageos.org/devices/ham) | S7-1200 可编程控制器 |
| [LG G3(冲刺)](https://forum.xda-developers.com/sprint-lg-g3) | [ls990](https://wiki.lineageos.org/devices/ls990) | 火鸟 11 号 HardStyl3r |
| [摩托罗拉摩托车 G7](https://forum.xda-developers.com/moto-g7) | [河](https://wiki.lineageos.org/devices/river) | 发明了 no BDI，npjohnson，syberhexen |
| [摩托罗拉摩托车 X 2014 (XT1092/3/5/6/7)](https://forum.xda-developers.com/moto-x-2014) | [胜利](https://wiki.lineageos.org/devices/victara) | 林肯哈克，派特尔 |
| [【next bit robin】](https://forum.xda-developers.com/nextbit-robin) | [以太](https://wiki.lineageos.org/devices/ether) | javelinanddart，mikeioannina，npjohnson |
| [z17 云团](https://forum.xda-developers.com/nubia-z17) | [nx563j](https://wiki.lineageos.org/devices/nx563j) | 贝克尔克 |
| [OnePlus One](https://forum.xda-developers.com/oneplus-one) | [培根](https://wiki.lineageos.org/devices/bacon) | jrior 001，npjohnson |
| [OnePlus 2](https://forum.xda-developers.com/oneplus-2) | [oneplus2](https://wiki.lineageos.org/devices/oneplus2) | ozzyscmacc，aviraxp |
| [OnePlus 3](https://forum.xda-developers.com/oneplus-3) | [oneplus3](https://wiki.lineageos.org/devices/oneplus3) | dianlujitao(地名) |
| [OnePlus 5](https://forum.xda-developers.com/oneplus-5) | [芝士汉堡](https://wiki.lineageos.org/devices/cheeseburger) | -=伊甸园美剧 http://sfile . ydy . com =-荣誉出品本字幕仅供学习交流，严禁用于商业途径 |
| [OnePlus 5T](https://forum.xda-developers.com/oneplus-5t) | [倾销](https://wiki.lineageos.org/devices/dumpling) | amartinz，codeworkx |
| [鸦片 F1(国际)](https://forum.xda-developers.com/oppo-f1) | [f1f](https://wiki.lineageos.org/devices/f1f) | 高速公路系统 |
| [opo 查找 7a/7s](https://forum.xda-developers.com/find-7) | [查找 7](https://wiki.lineageos.org/devices/find7) | 米凯伊诺娜 |
| [opo r5/r5 s(国际)](https://forum.xda-developers.com/oppo-r5) | [r5](https://wiki.lineageos.org/devices/r5) | 木薯 103 号 |
| opo r7s(国际) | [r7sf](https://wiki.lineageos.org/devices/r7sf) | 凯尔特人 |
| [opo r7 加](https://forum.xda-developers.com/r7-plus) | [r7 加](https://wiki.lineageos.org/devices/r7plus) | 马尼亚克 103 |
| [Realme 3 Pro(T3)](https://forum.xda-developers.com/realme-3-pro) | [RMX1851](https://wiki.lineageos.org/devices/RMX1851) | 地址: Karthick111, Nibaji, Darshan1205 |
| 三星 Galaxy A3 2016 (SM-A310F/M/N0/Y) | [a3 xee](https://wiki.lineageos.org/devices/a3xelte) | danwood76, 严格 |
| 三星 Galaxy A5 2016 (SM-A510F/M/Y/K/L/S/8) | [至 5xelte](https://wiki.lineageos.org/devices/a5xelte) | danwood76, 严格 |
| 三星 Galaxy A5 2017 (SM-A520F/DS/W) | [a5 和 17lte](https://wiki.lineageos.org/devices/a5y17lte) | 分支机构，raymanfx |
| 三星 Galaxy A7 2017 (SM-A720F/DS) | [至 7a 7 及 17lte](https://wiki.lineageos.org/devices/a7y17lte) | 分支机构，raymanfx |
| 三星 Galaxy Note 3 (SM-N9005/P) | [选择](https://wiki.lineageos.org/devices/hlte) | 作者 : Haggertk, npjohnson |
| 三星 Galaxy Note 3(SM-N9008V) | [hltechn](https://wiki.lineageos.org/devices/hltechn) | 作者 : Haggertk, npjohnson |
| 三星 Galaxy Note 3 (SM-N900K/L/S) | (T32) hltekor (T33) | 作者 : Haggertk, npjohnson |
| 三星 Galaxy Note 3 (SM-N900T/V/W8) | [hltetmo (T37)](https://wiki.lineageos.org/devices/hltetmo) | 作者 : Haggertk, npjohnson |
| 三星 Galaxy S III Neo Dual-SIM(GT-I9300I) | [s3ve3gds](https://wiki.lineageos.org/devices/s3ve3gds) | 皮顿有限公司 |
| [三星 Galaxy S III Neo 三星相机(GT-I9301I/Q)](https://forum.xda-developers.com/galaxy-s3-neo) | [S3 ve 3 gv](https://wiki.lineageos.org/devices/s3ve3gjv) | 皮顿有限公司 |
| [三星 Galaxy S III Neo Sony 相机(GT-I9300I/Q)](https://forum.xda-developers.com/galaxy-s3-neo) | [s3ve3gxx](https://wiki.lineageos.org/devices/s3ve3gxx) | 皮顿有限公司 |
| 三星 Galaxy S5 Active (T51) | (T52) klteactivexx (T53) | 关于 Javelinanddart |
| 三星 Galaxy S5 LTE(G900AZ/F/M/R4/R7/T/V/W8,S902L) | [KLT(t57)](https://wiki.lineageos.org/devices/klte) | 饰 Haggertk |
| 三星 Galaxy S5 LTE(G9006V/8V) | [kltechn(T61)](https://wiki.lineageos.org/devices/kltechn) | 饰 Haggertk |
| [三星 Galaxy S5 LTE (G900I/P)](https://forum.xda-developers.com/galaxy-s5) | KLT 电视 | 哈哥克 |
| [三星 Galaxy S5 LTE (SCL23)](https://forum.xda-developers.com/galaxy-s5) | [kltekdi](https://wiki.lineageos.org/devices/kltekdi) | 哈哥克 |
| [三星 Galaxy S5 LTE (G900K/L/S)](https://forum.xda-developers.com/galaxy-s5) | [kltek 或](https://wiki.lineageos.org/devices/kltekor) | 哈哥克 |
| [三星 Galaxy S5 LTE-A](https://forum.xda-developers.com/galaxy-s5) | [透镜](https://wiki.lineageos.org/devices/lentislte) | cvxda 萨斯曼 |
| [三星 galaxy S5 LTE duo(g 9006 w/8w)](https://forum.xda-developers.com/galaxy-s5) | [kltechndum](https://wiki.lineageos.org/devices/kltechnduo) | 哈哥克 |
| [三星 galaxy S5 LTE duo(g900 FD/MD)](https://forum.xda-developers.com/galaxy-s5) | [【klteduos】](https://wiki.lineageos.org/devices/klteduos) | 哈哥克 |
| [三星 Galaxy S5 Neo](https://forum.xda-developers.com/galaxy-s5-neo) | [s5neolte](https://wiki.lineageos.org/devices/s5neolte) | 丹伍德 76 号，严格 |
| [三星 Galaxy S5 Plus](https://forum.xda-developers.com/galaxy-s5) | [kccat6](https://wiki.lineageos.org/devices/kccat6) | cvxda，sassmann |
| [三星 Galaxy Tab S2 8.0 Wi-Fi (2016)](https://forum.xda-developers.com/tab-s2) | [gts28vewifi](https://wiki.lineageos.org/devices/gts28vewifi) | mccrea ry syphyr Luca 020400 |
| [三星 Galaxy Tab S2 9.7 Wi-Fi (2016)](https://forum.xda-developers.com/tab-s2) | [gts210vewifi](https://wiki.lineageos.org/devices/gts210vewifi) | 锡菲，卢卡 020400 |
| [索尼体验 Z3](https://forum.xda-developers.com/z3) | [z3](https://wiki.lineageos.org/devices/z3) | 汤姆 1000，我自己 5 |
| [索尼体验 Z3 契约(d5803/d 583)](https://forum.xda-developers.com/z3-compact) | [z3c](https://wiki.lineageos.org/devices/z3c) | 阿丽亚娜 16a |
| [【威力福克斯风暴】](https://forum.xda-developers.com/wileyfox-storm) | [倾卸机](https://wiki.lineageos.org/devices/kipper) | jrior 001 |
| [威尔 eyfox Swift](https://forum.xda-developers.com/wileyfox-swift) | [开裂](https://wiki.lineageos.org/devices/crackling) | jrior 001 |
| [小米 5](https://forum.xda-developers.com/mi-5) | [双子座](https://wiki.lineageos.org/devices/gemini) | bgcngm”防御 h2o64 |
| [小米 5s](https://forum.xda-developers.com/mi-5s) | [反复无常](https://wiki.lineageos.org/devices/capricorn) | 卢克 1337 |
| [小米 5s 加](https://forum.xda-developers.com/mi-5s-plus) | [钠](https://wiki.lineageos.org/devices/natrium) | 卢克 1337 |
| [小米 A1](https://forum.xda-developers.com/mi-a1) | [织物](https://wiki.lineageos.org/devices/tissot) | flex1911，TheScarastic .弹性 1911，the scarastic |
| [小米混合物](https://forum.xda-developers.com/mi-mix) | [锂](https://wiki.lineageos.org/devices/lithium) | balika011，闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边闪边 |
| [小米笔记 2](https://forum.xda-developers.com/mi-note-2) | [天蝎座](https://wiki.lineageos.org/devices/scorpio) | 乔·2k 01 |
| [小米 Mi Note 3](https://forum.xda-developers.com/mi-note-3) | [杰森](https://wiki.lineageos.org/devices/jason) | 电路集陶 |
| [小米 Redmi 3S/X](https://forum.xda-developers.com/xiaomi-redmi-3s) | [土地](https://wiki.lineageos.org/devices/land) | 艾萨克·陈 |
| [小米 Redmi 4/X](https://forum.xda-developers.com/xiaomi-redmi-4x) | [桑托尼](https://wiki.lineageos.org/devices/santoni) | 艾萨克·陈 |
| [小米红米 Note 4](https://forum.xda-developers.com/redmi-note-4) | [美度](https://wiki.lineageos.org/devices/mido) | 艾莉安克达 |
| Yandex 电话 | [琥珀色](https://wiki.lineageos.org/devices/Amber) | 高速之星，vm03 |

就像 LineageOS 17.1 版本一样，我们应该会看到更多的设备出现在每周的 LineageOS 16 版本列表中。

* * *

## 支撑线

LineageOS 一直是一项社区工作，依靠志愿者为社区的整体利益贡献自己的资源。如果你想为 LineageOS 做贡献，有多种方法。

### 成为设备维护者

帮助 LineageOS 扩展到更多设备的主要方法是尽可能维护设备的 ROM。如果你是一名开发者，想要将你的设备提交给官方支持，你可以[按照这里的指示](https://wiki.lineageos.org/submitting_device.html)。提交后，您将收到一些关于您提交内容的反馈。如果达到标准，你将被邀请到 Lineage 的通信渠道，你的设备资源将被分流到 LineageOS 的官方存储库。

### 提供翻译

或者，你也可以通过 Crowdin 提供不同语言[的翻译。该团队提到，即使您的语言在 Android 中没有得到官方支持，您也可以联系该团队，他们会采取措施纳入您的语言。但是，团队要求您只有在对该语言有合理的熟练程度时才提交翻译。](http://crowdin.com/project/lineageos)

### 捐款

为如此广泛的设备运行自动构建需要资源。你可以通过他们的 PayPal 或 Patreon 向 LineageOS 捐款来支付这些费用。

**捐赠给 linegeos:[通过 PayPal](https://paypal.me/LineageOS)| |[通过 Patreon](https://patreon.com/LineageOS)**

* * *

*本文于美国东部时间 2020 年 4 月 10 日下午 4:35 更新，将谷歌 Nexus 6、谷歌 Pixel、谷歌 Pixel XL、BQ Aquaris X 和 BQ Aquaris X Pro 添加到官方 LineageOS 17.1 版本的设备列表中。*