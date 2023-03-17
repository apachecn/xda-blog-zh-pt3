# 手机到 PC 屏幕镜像工具 scrcpy 的最新更新添加了对 Android 13 的无缝复制粘贴支持

> 原文：<https://www.xda-developers.com/scrcpy-update-android-13-clipboard-access/>

# 屏幕镜像工具 scrcpy 现在支持 Android 13 的剪贴板访问

从电脑上控制你的手机变得更加容易

scrcpy 的粉丝们今天有一些好消息，因为流行的 Android 屏幕镜像实用程序的维护者现在推出了该应用程序的 1.25 版本。这个版本主要集中在小的改进和修复上，但也有一些值得注意的变化，特别是如果你使用的是 [Android 13](https://www.xda-developers.com/android-13) 。

对于那些不熟悉这个工具的人来说，scrcpy(screen copy 的缩写)有两个组件。第一个是推送到目标 Android 设备的服务器应用程序，而另一个是 PC 的客户端，通过 [ADB](https://www.xda-developers.com/install-adb-windows-macos-linux/) 隧道与服务器通信。除了是一个免费的解决方案，scrcpy 也是开源的和高度可定制的，这使它成为最好的远程控制和屏幕镜像工具之一。

v1.25 更新的头条功能是 scrcpy 现在完全兼容 Android 13，包括复制粘贴支持。虽然以前版本的 scrcpy 可以镜像运行 Android 13 的设备的屏幕，但将剪贴板中的任何内容从主机粘贴到 Android 设备(反之亦然)会导致崩溃。现在服务器模块符合 Android 剪贴板管理器中的[属性标签，在剪贴板访问期间没有这样的错误。](https://android.googlesource.com/platform/frameworks/base.git/+/0e3e509b3bf4d561c26d87213387a290dfd688e3%5E%21/)

与 UI 相关的另一个改进是对高精度滚动的利用。如果主机支持更高级别的鼠标滚轮滚动精度，scrcpy 将自动使用它来实现更平滑的滚动。

scrcpy v1.25 中有许多较小的增强和更改，您可以在下面找到它们。

**scrcpy v1.25 变更日志:**

自 1.24 版以来的变化:

*   为 Android 13 调整复制粘贴内部功能( [#3497](https://github.com/Genymobile/scrcpy/issues/3497) )
*   增加对高精度滚动的支持( [#3363](https://github.com/Genymobile/scrcpy/issues/3363) ， [#3369](https://github.com/Genymobile/scrcpy/pull/3369) )
*   添加 Linux 的桌面入口文件( [#295](https://github.com/Genymobile/scrcpy/issues/295) 、 [#296](https://github.com/Genymobile/scrcpy/pull/296) 、 [#748](https://github.com/Genymobile/scrcpy/issues/748) 、 [#1636](https://github.com/Genymobile/scrcpy/issues/1636) 、 [#3351](https://github.com/Genymobile/scrcpy/pull/3351) )
*   为-s/ - serial ( [#3522](https://github.com/Genymobile/scrcpy/issues/3522) ， [#3523](https://github.com/Genymobile/scrcpy/pull/3523) )添加 bash 和 zsh 自动完成功能
*   将当前 adb 端口(如果有)用于- tcpip ( [#3591](https://github.com/Genymobile/scrcpy/issues/3591) ， [#3592](https://github.com/Genymobile/scrcpy/pull/3592) )
*   添加回退功能以获取一些设备的显示信息( [#3416](https://github.com/Genymobile/scrcpy/pull/3416) ， [#3573](https://github.com/Genymobile/scrcpy/pull/3573) )
*   修复设置了- forward-all-clicks 时的点击行为( [#3568](https://github.com/Genymobile/scrcpy/issues/3568) ， [#3579](https://github.com/Genymobile/scrcpy/pull/3579) )
*   修复窗口标题中非 ASCII 字符的支持( [#2932](https://github.com/Genymobile/scrcpy/issues/2932) ， [#3547](https://github.com/Genymobile/scrcpy/pull/3547) )
*   修复了 Android 13 beta ( [#3446](https://github.com/Genymobile/scrcpy/issues/3446) )某些版本的 getDisplayIds()崩溃问题
*   在 Windows 版本中将平台工具升级到 33.0.3 (adb)
*   在 Windows 64 位版本中将 FFmpeg 升级到 5.1.2
*   在 Windows 版本中将 SDL 升级到 2.26.1
*   各种技术修复

您可以在 GitHub 上探索并贡献于 scrcpy 存储库，也可以下载预编译的版本。如果您已经通过软件包管理器安装了应用程序，请检查其中的更新以获得最新版本。

**[下载 scrcpy](https://github.com/Genymobile/scrcpy/releases/latest)**