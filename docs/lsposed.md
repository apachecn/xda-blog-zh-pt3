# 什么是 LSPosed，你可以在你的 Android 设备上用它做什么？

> 原文：<https://www.xda-developers.com/lsposed/>

我们过去已经讨论过 Magisk 和它的模块,以及它们如何提供一个以“无系统”方式完成的修改世界。Magisk 基于覆盖的界面像 Xposed 一样越来越受欢迎，这也不无道理。除了无系统带来的所有好处，Magisk 还可以用于通过 [Riru](https://www.xda-developers.com/riru/) 在 [Android Zygote 进程](https://developer.android.com/topic/performance/memory-overview)的环境中运行代码。对于一些修改者来说，这些理由足以让他们涉足所有没有系统的东西。

最初的 Xposed 框架早就被抛弃了，但是后市场社区却出现了屈指可数的精神继承者。以 Magisk 和 Riru 为基础， **LSPosed** 就是这样一个项目，提供了一个无系统的艺术挂钩框架。

## 什么是假的？

LSposed is another Xposed implementation in the form a Riru module. Originally started as a fork of [EdXposed](https://www.xda-developers.com/edxposed/), the project has been maintained by LoveSy (aka [yujincheng08](https://github.com/yujincheng08)), 南宫雪珊 (aka [vvb2060](https://github.com/vvb2060)), NekoInverter (aka [tehcneko](https://github.com/tehcneko)), and several other developers. The team developed an in-house Android ART hook library called [LSPlant](https://github.com/LSPosed/LSPlant) and created the framework on top of it. The front-end is known as *LSPosed Manager*.

## LSPosed 的特点是什么？

*   兼容 Riru 和 Zygisk。
*   支持多用户设置。
*   您可以隐藏管理器应用程序。
*   与 Android Oreo 8.1 到 [Android 13 Beta 1](https://www.xda-developers.com/android-13-beta-1-released/) 兼容。

## 如何下载 LSPosed？

LSposed 的最新版本可以在其 GitHub repo 上找到。请记住，该模块同时支持 Riru 和 Zygisk，因此您应该根据您现有的设置选择合适的版本。

**[下载 LSposed](https://github.com/LSPosed/LSPosed/releases/latest)**

虚拟经理位于谷歌 Play 商店。请记住，仅仅安装应用程序不足以激活框架。

[app box Google play " org . lsposed . manager "]

## 如何安装 LSPosed？

在安装 LSposed 之前，请确保在目标设备上安装了最新版本的 Magisk 和 Riru。

1.  从前面提到的 URL 下载 LSposed ZIP 包。如果您已经在 PC 或 Mac 上下载了它，那么将您的 Android 设备连接到它，并将下载的 ZIP 文件复制到目标设备的内存中。
2.  打开 Magisk 应用程序，使用底部导航菜单切换到*模块*选项卡。
3.  点击名为*从存储器安装*的按钮。接下来，浏览并选择您之前下载的 ZIP 文件。
    *   如果您使用的是 Zygisk，那么刷新名为 LSPosed-xxx-zygisk-release.zip 的文件。
    *   如果你用的是 Riru，那就闪存名为 LSPosed-xxx-riru-release.zip 的文件，

4.  成功安装后，重新启动您的设备。
5.  您应该会在启动器中看到 LSPosed Manager 图标。
    *   如果图标不存在，您可以拨`*#*#5776733#*#*`(又名 LSPosed)来启动管理器界面。这一招在隐藏 app 后也有效。

6.  就是这样！

## LSPosed 和原始 Xposed 框架之间的比较

Android Oreo 之后，遗留的 Xposed 框架停止工作。此外，它修改了核心系统文件，以取代 app-process 和 ART 运行时。这样的设计对于现代安卓版本来说是不可行的。

另一方面，LSPosed 是一个强大的 Magisk 模块，有很大的潜力。维护人员经常向代码库添加补丁和新特性。它不仅兼容各种定制的 Android 皮肤，而且还支持 Zygisk(即 Zygote 中的 Magisk)，这在长期可持续性方面是一大优势。

**[XDA 提出的讨论思路](https://forum.xda-developers.com/t/4228973/)**

## 结论

一旦你安装并配置了 LSPosed，请查看[最佳曝光模块](https://www.xda-developers.com/best-xposed-modules/)，为你的 Android 改造之旅充能。为了释放 root 权限的全部力量，你还应该看看适用于 rooted Android 设备的[最佳应用](https://www.xda-developers.com/best-android-root-apps/)。