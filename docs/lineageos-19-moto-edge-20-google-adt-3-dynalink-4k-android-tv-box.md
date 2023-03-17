# LineageOS 19 现在可用于 Moto Edge 20、谷歌 ADT-3 和 Dynalink 4K 盒子

> 原文：<https://www.xda-developers.com/lineageos-19-moto-edge-20-google-adt-3-dynalink-4k-android-tv-box/>

在上月下旬为[一加 8 系列、Galaxy A52 4G 和 Galaxy A72](https://www.xda-developers.com/lineageos-19-oneplus-8-series-galaxy-a42-4g-galaxy-a72/) 发布基于 Android 12 的 LineageOS 19 之后，LineageOS 团队现在已经将支持扩展到另外三款设备。最新进入 LineageOS 19 生产名单的设备包括 Moto Edge 20、谷歌 ADT-3 和沃尔玛的 Dynalink 4K 盒子。

Moto Edge 20 是去年的一款中端设备。它装有高通的骁龙 778G 芯片，6.7 英寸 144Hz 有机发光二极管显示屏，108MP 四摄像头设置和 4,000mAh 电池。这款手机推出了 Android 11，但摩托罗拉后来将其更新为 Android 12。如果你不是 Android 12 版本的粉丝，你现在可以在上面闪现 LineageOS 19，看看它是否提供了更好的体验。

谷歌 ADT-3 是一款面向开发者的 Android 电视设备。早在 2020 年 1 月，谷歌就在 Android TV 10 上推出了这款应用，以帮助开发者在运行该版本的设备上测试他们的应用。如果你还留着它，你现在可以用 LineageOS 19 把它更新到 Android 12。

同样，Dynalink 4K 盒子是沃尔玛的一款 Android 电视设备，与 Android TV 10 一起推出。尽管 Dynalink 在发布设备固件更新方面做得不错，但它还没有推出操作系统升级。所以，如果你想在设备上试用 Android 12，你可以通过下面提供的链接来 flash LineageOS 19。

| 

序列号

 | 

设备和论坛链接

 | 

设备代号和维基链接

 | 

维护者

 |
| --- | --- | --- | --- |
| 1. | [Moto Edge 20](https://forum.xda-developers.com/f/motorola-edge-20.12419/) | [柏林](https://wiki.lineageos.org/devices/berlin/) |  |
| 2. | 谷歌 ADT-3 | [死池](https://wiki.lineageos.org/devices/deadpool/) | 

*   npjohnson
*   严格的
*   webgeek1234
*   死者 96385
*   特劳塔马基
*   卢卡 020400
*   阿莱斯托

 |
| 3. | Dynalink 4K 盒 | [韦德](https://wiki.lineageos.org/devices/wade/) | 

*   npjohnson
*   bgcngm
*   严格的
*   webgeek1234
*   死者 96385
*   特劳塔马基
*   卢卡 020400
*   阿莱斯托

 |

值得注意的是，在 Android 电视盒子上闪烁 LineageOS 与在智能手机/平板电脑上闪烁截然不同。例如，用于引导加载程序解锁的常规`fastboot oem unlock`或`fastboot flashing unlock`命令不适用于上述 Android 电视设备。此外，平台要求在定制恢复刷新之前刷新`dtb`和`dtbo`分区。我们强烈建议仔细阅读上面链接的 Wiki 页面中的安装说明以及我们论坛中提供的其他链接文档[，以避免不可预见的问题。](https://forum.xda-developers.com/t/4313743/)

然而，当在手机上安装 LineagesOS 时，这个过程相当简单。你必须先解锁你的设备的引导程序，然后安装一个像 TWRP 这样的自定义恢复。如果你不确定如何去做，你可以遵循我们的[如何安装自定义 ROM](https://www.xda-developers.com/how-to-install-custom-rom-android/) 和[如何安装 TWRP 指南](https://www.xda-developers.com/how-to-install-twrp/)中提供的步骤。一旦你完成了解锁引导程序和安装 TWRP，按照 LineageOS Wiki 的安装说明。此外，请备份您的数据，否则您可能会在安装过程中丢失数据。

请注意，LineageOS 19 没有预装谷歌应用套件。如果你想使用任何谷歌应用或服务，你必须在安装 ROM 后刷新一个合适的 GApps 包。查看我们关于[如何下载和安装最新 GApps](https://www.xda-developers.com/download-google-apps-gapps/) 的指南，获取详细说明。请记住，并非所有的 GApps 发行版都提供 Android TV 兼容的软件包，因此请确保为 Android TV 设备选择正确的软件包。

除了将 LineageOS 19 支持扩展到这三款设备，LineageOS 团队还将索尼 Xperia X 和索尼 Xperia X Compact 添加到了 LineageOS 18.1 构建名册中。此外，该团队已经从 LineageOS 18.1 构建名册中删除了 Zenfone Max M1 和 Zenfone Max M2。