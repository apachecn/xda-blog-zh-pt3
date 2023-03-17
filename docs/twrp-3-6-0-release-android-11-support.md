# TWRP 3.6.0 发布，支持搭载 Android 11 的设备

> 原文：<https://www.xda-developers.com/twrp-3-6-0-release-android-11-support/>

Team Win Recovery Project(简称 TWRP)已经存在了几年，它已经发展成为 Android 社区的首选，以更先进、功能更丰富的替代品取代他们设备上的股票恢复。对于大多数用户来说，安装任何一种售后软件修改，无论是[定制 ROM](https://www.xda-developers.com/most-popular-custom-roms-android/) 、[定制内核](https://www.xda-developers.com/most-popular-custom-kernels-for-android/)、 [Magisk](https://www.xda-developers.com/how-to-install-magisk/) 还是其他工具，都需要使用 TWRP。自定义恢复是开源的，它支持数百种设备。今天，该项目已经升级到 3.6.0 版本，带来了 Android 11 支持，解密方面的许多改进，新功能，大量新支持的设备，以及 TWRP 安装方式的重大变化。

## TWRP 3.6.0 的新功能

到目前为止，在带有 A/B 分区的设备上刷新 TWRP 需要临时启动 TWRP 镜像(使用`fastboot boot`命令),然后使用*安装恢复 Ramdisk* 选项永久安装。然而，在这个实现中，ramdisk 不能自己填充，因为您仍然需要将它指向下载的 TWRP 映像。今后，用户将在自定义恢复的*高级*部分看到一个新的*闪光电流 TWRP* 选项。选择该选项会将您刚刚启动的 TWRP 映像永久安装到设备上，从而简化整个安装过程。

与高级用户最相关的另一个变化是包含了两个与[动态分区](https://www.xda-developers.com/android-q-dynamic-system-updates-project-treble/)和[虚拟 A/B 分区设置](https://www.xda-developers.com/google-virtual-ab-seamless-updates-android-11/)相关的新故障排除选项。首先，有一个名为 *Unmap Super Devices* 的选项，允许您轻松禁用所有动态分区并卸载它们。第二个称为*合并快照*，如果您遇到快照合并的问题，并且想要强制提交对动态分区的更新，这可能会很方便。它们都可以在 TWRP 主菜单的*高级*部分找到。

除此之外，TWRP 现在完全兼容工厂安装的 Android 11 设备。由于 TWRP 代码库的主要部分已经在本课程中从头开始重写，以支持谷歌引入的架构变化，项目维护者希望看到一个更快的 Android 12 发布过程。

TWRP 3.6.0 的[完整变更日志如下:](https://twrp.me/site/update/2021/11/28/twrp-3.6.0-released.html)

### TWRP 3.6.0 变更日志

**安卓 9 分支:**

*   修理
    *   clarity 的 SAR 更新脚本名称- CaptainThrowback
    *   修复 android-7.1 中的构建工具箱- CaptainThrowback
    *   修复巴什-贾尔-企鹅

**安卓 11 分支:**

*   添加对安装 realme/OPPO OTA - Ctapchuk 的支持
*   更新定制 makefiles 到 golang 模块
*   策略更新- nebrassy、bigbiff、CaptainThrowback
*   a11 - bigbiff、micky387、CaptainThrowback 的加密更新
*   供应商内核模块加载器- bigbiff
*   虚拟 A/B 更新- bigbiff
*   快照合并- bigbiff
*   重新打包警告- CaptainThrowback
*   f2fs 格式化修复- systemad
*   bootdevice 中的 symlink 动态分区- Mohd Faraz
*   修理
    *   修复解析清除缓存的 get_args
    *   供应商 hal fixes - Mohd Faraz
    *   修复三星 haptics - soulr344
    *   摘要检查修复- epicX
    *   ozip 解密修复- Ctapchuk
    *   改变空白屏幕的工作方式-肖恩·霍伊特

**安卓 9 和安卓 11 分支:**

*   为 PIN 输入添加数字模板- CaptainThrowback
*   忽略 A12 XML 文件二进制格式- zhenyolka
*   添加对 A12 keymaster_key_blob 文件结构的支持- zhenyolka
*   keymaster 恢复:当 pin、密码或模式启用时发出警告
*   作为引导设备进行恢复的新闪存方法:
*   高级>闪光电流 twrp - nebrassy
    *   工厂擦除和 mtp 修复- CaptainThrowback
*   添加印度尼西亚语言- Xdisk
*   更新俄语- Ctapchuk
*   添加取消加密页面- CaptainThrowback
*   在 TWRP 复制日志时复制 logcat
*   修理
    *   FBE 加密修复- CaptainThrowback
    *   用于压缩的重新打包修复程序- nebrassy
    *   修复恢复 Bootloop - CaptainThrowback 的排除标准
    *   如果供应商不可用，卸载供应商- LinkBoi00
    *   主题更新- LinkBoi00

* * *

## 新支持的设备

如前所述，TWRP 可用于过多的设备，并且名单还在不断增加。除了发布新的主要版本，该团队现在还正式添加了对以下智能手机的支持:

此外，一些设备(如下所列)已经获得了新的维护者。就长期发展支助而言，这对它们来说确实是一个好迹象。

* * *

## [计] 下载

您可以从下面链接的官方网站为您的设备下载最新版本的 TWRP。请务必查看您的设备的 XDA 分论坛，因为当新版本上线时，TWRP 维护者可能会在那里发布更多特定于设备的说明。

**[为您的设备下载 TWRP](https://twrp.me/Devices/)**

最后，一定要从 Google Play 下载 TWRP 官方应用。当新版本的自定义恢复可用时，该应用程序会提醒您。它还能让你从你的设备上下载最新版本。

[app box Google play " me . twrp . twrpapp "]