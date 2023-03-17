# 环境音乐 Mod v2 实践:谷歌像素的现在播放功能端口

> 原文：<https://www.xda-developers.com/google-pixel-now-playing-ambient-music-mod-v2-hands-on/>

大多数人都会同意，Pixel 智能手机上的软件展示了谷歌认为 Android *应该是*的样子，因此，该软件经常受到发烧友的欢迎。尽管如此，由于专门的修改社区，你不一定要拥有一个像素设备来利用其软件功能。例如，“正在播放”功能仍然是 Pixel 系列的专属功能，但开发者 Kieron Quinn，在我们的论坛上也被称为 [Quinny899](https://forum.xda-developers.com/m/quinny899.3563640/) ，成功地将它以混合 Xposed-Magisk 模块的形式[移植到其他 Android 智能手机](https://www.xda-developers.com/google-pixel-now-playing-feature-ported/)，该模块被命名为**环境音乐模块**。现在，奎因更进一步，彻底改革了 mod，使其成为一个非根解决方案。

## 满足环境音乐模式 v2

在没有 root 权限的情况下，让 Pixel 智能手机的[环境音乐识别功能与硬件无关并不是一件容易的事情，但 Quinny899 使用滴实现了这一壮举。不知情的是，滴使用了一种独特的服务，即](https://support.google.com/pixelphone/answer/7535326)[允许第三方应用程序通过 Android 调试桥(ADB)接口访问系统级 API](https://www.xda-developers.com/implementing-shizuku/)。自 v2 发布以来，环境音乐模式可以在运行 Android 12 或更高版本的设备上无需 root 访问即可工作**。**

另一个大的变化是移除了与 Xposed 相关的依赖项。不再需要安装像 [EdXposed](https://www.xda-developers.com/edxposed/) 或 [LSPosed](https://www.xda-developers.com/lsposed/) 这样的 Xposed 发行版，因为 mod 现在是一个独立的应用程序。请记住，你仍然可以在旧的 Android 版本上选择环境音乐模式的根版本。

## 环境音乐 Mod v2 有什么特点

以下是环境音乐模式提供的功能概要:

*   完全支持现在播放，基于 Pixel 设备的最新版本和最新的音乐数据库
*   自动环境音乐识别，通过设置控制识别运行的频率-在电池使用和便利性之间找到正确的平衡
*   现在播放历史和收藏夹支持
*   支持手动触发识别，包括一个主屏幕部件
*   在支持的设备上进行点播识别，对不在本地数据库中的歌曲使用 Google Assistant 支持的识别引擎(必须手动触发)
*   在锁定屏幕上显示正在播放的歌曲(需要辅助功能服务)
*   查看可识别歌曲的完整曲目列表，如果您的喜好与设备的区域设置不匹配，请更改数据库位置

在撰写本文时，开发人员已经在 v2 主版本之后推出了两个修补程序。现在，您可以选择替代编码选项并微调“增益”值，以修复失真和/或劈啪声问题。

## 如何下载和安装环境音乐 Mod v2

就像最初的版本一样，环境音乐 Mod v2 是一个免费的开源 Mod。你可以在下面链接的项目 GitHub repo 上找到 APK 的最新版本。

**[下载环境音乐模式](https://github.com/KieronQuinn/AmbientMusicMod/releases/latest)**

要安装下载的 APK，看一下[我们的侧装安卓应用包指南](https://www.xda-developers.com/how-to-sideload-install-android-app-apk/)。安装后，环境音乐模块将要求滴访问。根据底层 Android 版本，您可以继续使用 root 或非 root 模式。接下来，该应用程序将下载一些额外的组件，并提示您给予所需的权限——仅此而已。

## 比较 Google 的 Now Playing 和 Ambient Music Mod v2

在引擎盖下，Ambient Music Mod 使用了一款名为 Android System Intelligence 的谷歌应用的[修改版。设备上识别部分是在查询音乐数据库后执行的——这正是谷歌现在播放的内容。因此，Ambient Music Mod 在非谷歌设备上的真实表现或多或少类似于 Pixel 智能手机——尤其是在调整参数之后。然而，像素专属功能和 mod 之间有一些不同之处。](https://github.com/KieronQuinn/NowPlaying)

这里有一个快速的实践来展示 Google 官方实现和 Quinny899 的 mod 之间的区别。测试设备是运行 Android 13 Beta 3.2 的谷歌 Pixel 4a 和运行 Android 11 之上的 LineageOS 18.1 非官方版本的 Redmi 5。

### 1.用户界面

在 Pixel 智能手机上，可以访问*设置* = > *声音&振动*下的“正在播放”选项。然而，环境音乐模式是一个独立的应用程序，因此你可以在你的启动器的应用程序列表部分找到它的条目。点击图标后，您可以访问*正在播放*屏幕和其他选项。

### 2.识别环境音乐

一旦下载了音乐数据库，您应该能够为两者打开名为“识别附近播放的歌曲”的选项。在谷歌 Pixel 设备上，你周围播放的歌曲应该会被自动识别并显示在锁定屏幕上。

另一方面，环境音乐模式允许你切换这个选项。如果你不想弄乱你的锁屏，你可以选择手动“识别”按钮来识别音乐。

### 3.现在播放历史和音乐搜索

*现在播放历史*部分在两个实现中实际上是相同的。您可以探索已识别音乐的历史，将它们添加到*收藏夹*列表中，并可选择将该部分的快捷方式放在您的主屏幕上以便快速访问。

然而，手动搜索部分是不同的。在 Pixel 手机上，你只需打开名为*在锁屏上显示搜索按钮*的选项，就可以在锁屏上搜索歌曲。这种“按需”识别机制可能无法在所有开箱即用的设备上使用环境音乐模式。欲知详情，敬请[浏览开发者](https://github.com/KieronQuinn/AmbientMusicMod/wiki/Enabling-On-Demand)的解释。

### 4.多方面的

由于谷歌的 Now Playing 模块是 Pixel 固件的内置组件，因此没有太多需要修改的地方。为了推广它，Quinny899 必须在环境音乐 Mod 代码库中放置一些自定义参数。

您可以调整音乐识别周期和缓冲区，强制识别例程在小 CPU 内核上运行，调整增益，等等。这是大大提高兼容性的东西。例如，我必须在 Redmi 5 上选择备用编码(从 v2.0.2 版本开始可用)，否则，它将因失真而无法检测环境音乐。mod 还允许你备份你的自定义设置，并在以后恢复它们。

## 结论

Now Playing 功能从未在 AOSP 推出过，所以 Kieron 不得不进行逆向工程，并经历了大量的挑战，以使其适用于非谷歌设备。何[在他的博客里详细描述了这个过程](https://medium.com/@KieronQuinn/now-playing-ambient-music-mod-v2-93cd4042cc11)。如果你想了解幕后的一切，不妨读一读。

前往 GitHub 链接获取代码库和更多关于 mod 如何工作的信息。你也可以参与讨论，报告错误，或者通过在下面链接的论坛帖子中发帖来请求新功能。

**环境音乐 Mod:[GitHub Repo](https://github.com/KieronQuinn/AmbientMusicMod)| |[XDA 讨论线程](https://forum.xda-developers.com/t/4260761/)**

* * *

**来源:** [米沙·拉赫曼在推特上](https://twitter.com/MishaalRahman/status/1538628853949779969)