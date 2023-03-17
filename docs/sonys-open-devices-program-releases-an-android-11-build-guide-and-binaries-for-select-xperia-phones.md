# 索尼开放设备计划提供 AOSP Android 11 构建指南

> 原文：<https://www.xda-developers.com/sonys-open-devices-program-releases-an-android-11-build-guide-and-binaries-for-select-xperia-phones/>

# 索尼的开放设备计划为部分 Xperia 手机发布了 Android 11 构建指南和二进制文件

索尼通过其开放设备倡议发布了几款 Xperia 手机的 Android 11 构建指南和软件二进制文件。请继续阅读！

与一些主要的原始设备制造商不同，索尼移动尚未公布 Android 11 更新发布的详细路线图。该公司甚至没有提供一个公共测试程序来评估 Xperia 智能手机上 Android 的最新版本，但这不是全部。随着 Android 的每一次重大修订，索尼都会发布软件二进制文件以及为属于其[开放设备计划](https://www.xda-developers.com/tag/open-device-program/)一部分的设备编译最新版 AOSP 的指令。由于 Android 11 [的代码库已经在 AOSP](https://www.xda-developers.com/android-11-source-code-aosp/) 正式发布了一段时间，这家日本 OEM 厂商现在已经发布了 Android 11 兼容的二进制文件，以及为一系列 Xperia 设备构建 AOSP 11.0 的分步指南。

首先，您需要访问一个合适的构建环境，以便可以从源代码编译 AOSP 构建。你应该理想地选择一台运行 Linux 的 PC，但是 Windows 10 用户也可以使用 Windows Subsystem for Linux(WSL)做同样的事情[。下一部分是配置构建环境，即，您必须安装适当版本的 Java 开发工具包、一些软件包和库，以及](https://www.xda-developers.com/how-to-build-lineageos-on-windows-10-using-wsl-2/) [Repo 工具](https://source.android.com/source/developing.html)来跨多个存储库工作。最后，你需要下载完整的 Android 11 源代码树，Xperia 设备的本地清单，并按照指南的一步一步的指示(链接如下)来成功编译 AOSP 图像。如果一切顺利，你应该已经准备好了 AOSP 11.0 的图片，可以在你的索尼智能手机上播放了。

**[为索尼 Xperia 设备构建 AOSP Android 11.0](https://developer.sony.com/develop/open-devices/guides/aosp-build-instructions/build-aosp-android-android-11-0-0/)**

请注意，在刷新生成的版本之前，您必须[解锁 Xperia 设备](https://www.xda-developers.com/sonys-open-device-program-releases-an-updated-guide-for-unlocking-bootloader-of-the-xperia-devices/)的引导加载程序。此外，包含低级软件二进制文件的特定于平台的映像需要刷新为供应商映像。以下是首批从 OEM 收到 AOSP 11.0 软件二进制文件的 Xperia 智能手机。

由于我们天才的售后开发社区，一些 Xperia 设备已经获得了一些工作[基于 Android 11 的定制 rom](https://www.xda-developers.com/android-11-custom-rom-list/)。现在，官方的 AOSP 11.0 软件二进制文件已经发布，我们可能不用再等太久就可以获得用于上述智能手机的相当稳定的第三方 rom。