# Magisk v25.0 引入了重新设计的 MagiskInit 来解决 SELinux 问题

> 原文：<https://www.xda-developers.com/magisk-v25-release-selinux-fix/>

# Magisk v25.0 改进了 SELinux 处理，修改了根权限管理，等等

Magisk (v25.0)的最新更新已经发布，包含大量的错误修复和功能改进。继续阅读，了解更多信息！

在这一点上，我们 XDA 肯定你们大多数人至少听说过 Magisk。该项目由吴炯创建，又名 XDA 认可的开发人员 [topjohnwu](https://forum.xda-developers.com/m/topjohnwu.4470081/) ，该项目最初是作为一个无系统的根方法开始的，并逐渐发展成为一个更加多样化和强大的解决方案，不仅仅是一个简单的超级用户权限提供者。不言而喻，开发者和贡献者总是积极地努力完善它。Magisk 最新的重大更新，对应的是第二十五版(v25)，现在已经到了公测分支。变更日志是微妙但非常重要的，所以让我们深入了解它。

**[Magisk XDA 论坛](https://forum.xda-developers.com/f/magisk.5903/)**

此次更新的第一件事(可能也是最重要的一件事)是重新编写的 MagiskInit 软件。对于不知情的人来说，`magiskinit`二进制程序负责替换股票`init`进程作为第一个运行的程序，将 Magisk 服务注入`init.rc`，并修补 SELinux 策略规则。由于引入了全新的策略注入机制，开发人员已经成功解决了大多数与 SELinux 相关的不兼容问题。此外，MagiskInit 现在支持 [Android 13 的通用内核映像](https://www.xda-developers.com/google-pixel-6-6-pro-mainline-linux-kernel-support/) (GKI)格式。

最后但并非最不重要的一点是，新版本为 MagiskSU 组件提供了一些安全性增强。根权限管理已经过改进，以防止恶意 UID 重用攻击。Magisk 现在强制执行根管理器 APK 签名验证，以保护用户免受已被篡改的 Magisk 管理器的修改版本的影响。尽管如此，开发人员在从 Magisk 的代码库构建 Magisk 时，仍然可以使用他们自己的签名密钥。你也可以选择官方的调试版本，以防你为了修补而需要去掉签名验证。

这是 Magisk v25.0 的官方变更日志:

*   [MagiskInit]更新 2SI 实现，显著提高设备兼容性(如索尼 Xperia 设备)
*   [MagiskInit]推出新的`sepolicy`注射机制
*   [MagiskInit]支持 Oculus Go
*   【MagiskInit】支持 Android 13 GKIs(像素 6)
*   [MagiskBoot]修复 vbmeta 提取实现
*   [应用]修复旧版本 Android 上的存根应用
*   使用`sharedUserId`正确支持应用程序
*   [MagiskSU]修复了`magiskd`中可能出现的崩溃
*   [MagiskSU]一旦`system_server`重新启动就删除未使用的 UID，以防止 UID 重用攻击
*   [MagiskSU]验证并强制执行已安装的 Magisk 应用程序的证书，以匹配分销商的签名
*   [MagiskSU] [Zygisk]适当的软件包管理和检测
*   [Zygisk]修复运行旧内核 Android 12 的设备上的函数挂钩
*   [Zygisk]修复 Zygisk 的自代码卸载实现
*   [DenyList]修复共享 UID 应用程序上的 DenyList
*   [BusyBox]为运行旧内核的设备添加解决方法

您可以通过下面的链接下载最新版本。如果您不熟悉 Magisk，您应该查看我们关于如何使用该工具根化您的设备的深入指南。如果你碰巧遇到了最新版本的任何问题，确保在项目的 [GitHub 库](https://github.com/topjohnwu/Magisk/issues)上提交一份错误报告。

**T5 下载 Magisk v 25.0**

* * *

**来源:** [吴炯在推特上](https://twitter.com/topjohnwu/status/1534117522424811520)