# 谷歌上传 Pixel 6 和 Pixel 6 Pro 的工厂图像、设备树、内核源代码

> 原文：<https://www.xda-developers.com/google-pixel-6-6-pro-factory-images-kernel-source-code/>

本月早些时候，谷歌推出了 Pixel 6 和 Pixel 6 Pro T1，这是该公司第一批由自己的[张量硅](https://www.xda-developers.com/google-says-its-tensor-chip-is-80-faster-than-the-pixel-5s-cpu/)驱动的旗舰产品。这些设备一直是太多泄露的接收端，在很大程度上，[发射](https://www.xda-developers.com/google-pixel-6-launch/) [事件](https://www.xda-developers.com/google-pixel-6-pro-launch/)并没有带来任何重大惊喜。Pixel 6 系列计划从今天起面向消费者，谷歌现在已经上传了所有工具、文件和文档，供有兴趣在手机上运行定制软件的售后开发者使用。

**[谷歌 Pixel 6 Pro 评测:不可否认的 Exynos 灵感的奇妙日常手机](https://www.xda-developers.com/google-pixel-6-pro-review/)**

### 谷歌 Pixel 6 和谷歌 Pixel 6 Pro 的工厂图像

工厂图像对设备来说很重要，因为它们使软件实验在思想上更容易，因为你知道你可以选择在事情变糟的情况下回到一个工作的设备。即使对于那些没有购买手机的人来说，工厂图像也可以访问 Pixel 6 的应用程序(例如[最新的谷歌相机版本](https://www.xda-developers.com/google-camera-8-4-167-rolling-out/))和其他系统文件，这些文件有助于将独家功能移植到其他设备。

**下载工厂图片:[谷歌 Pixel 6(代号:“黄鹂”)](https://developers.google.com/android/images#oriole)| |[谷歌 Pixel 6 Pro(代号:“渡鸦”)](https://developers.google.com/android/images#raven)**

如果您想返回到库存软件，您可以从上面的链接中提取并刷新相应的工厂映像固件。有四组工厂图像可用:三组用于美国运营商型号，另一组用于未锁定单元。发布的软件包带有与 2021 年 10 月[Android 安全补丁级别](https://www.xda-developers.com/october-2021-android-security-bulletin/)相对应的 **SD1A.210817.01x** 内部版本号。

值得注意的是，谷歌已经以 **SD1A.210817.036** (威瑞森为 **SD1A.210817.036.A8** )的形式[推出了新版本](https://support.google.com/pixelphone/thread/132599975/)，2021 年 11 月的补丁作为第一天的更新，但我们还没有看到相应的工厂图像。

### 内核源代码和设备树

新像素的框架源代码、内核源代码和设备树也已经上传。这些资源将对定制内核、恢复和 ROM 开发人员非常有帮助，以便在这些手机上启动售后开发工作。

| 

设备

 | 

内核源代码

 | 

设备树

 | 

分离政策

 |
| --- | --- | --- | --- |
| 谷歌 Pixel 6/6 Pro Unified(代号:“raviole”) | [链接](https://android.googlesource.com/device/google/raviole-kernel/) | [链接](https://android.googlesource.com/device/google/raviole/) | 不适用的 |
| 常见 SoC 元件(代号:“gs101”) | 不适用的 | [链接](https://android.googlesource.com/device/google/gs101/) | [链接](https://android.googlesource.com/device/google/gs101-sepolicy/) |

**[谷歌 Pixel 6 XDA 论坛](https://forum.xda-developers.com/f/google-pixel-6.12311/) ||| [谷歌 Pixel 6 Pro XDA 论坛](https://forum.xda-developers.com/f/google-pixel-6-pro.12313/)**

 <picture>![The Pixel 6 comes with Google's new Tensor chip, a modern design, and flagship cameras.](img/7343f77af84019bd24844d3d2e495f29.png)</picture> 

Google Pixel 6

Pixel 6 配备了谷歌新的张量芯片、现代设计和旗舰相机。

 <picture>![The Pixel 6 Pro is the larger sibling that comes with Google's new Tensor chip, a modern design, and an extra telephoto camera.](img/5c825565a61d24d571df294787f045fc.png)</picture> 

Google Pixel 6 Pro

Pixel 6 Pro 是较大的兄弟，配有谷歌的新张量芯片、现代设计和额外的远摄相机。