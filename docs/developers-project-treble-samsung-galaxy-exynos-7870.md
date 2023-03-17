# Project Treble 移植到搭载 Exynos 7870 的三星 Galaxy 手机上

> 原文：<https://www.xda-developers.com/developers-project-treble-samsung-galaxy-exynos-7870/>

# 开发人员通过 Exynos 7870 为几款三星 Galaxy 手机带来了 Project Treble 支持

一批基于 Exynos 7870 的三星 Galaxy 手机通过手动分区和定制供应商实施获得了 Project Treble 兼容性。

Exynos 7870 是三星使用最广泛的 SOC 之一。自 2016 年以来，原始设备制造商一直在其手机中使用这种八核(8 个 ARM Cortex-A53 内核，主频为 1.6GHz)片上系统，甚至在 2019 年发布了采用相同 14 纳米处理器的 [Galaxy M10](https://www.xda-developers.com/samsung-galaxy-m20-m10-india-launch/) 。有趣的是，一些更新的基于 Exynos 7870 的设备搭载了 Android Oreo，这使得它们与[项目 Treble](https://www.xda-developers.com/googles-project-treble-modularize-android-so-oems-can-update-devices-faster/) 兼容。虽然三星没有正式向后移植对传统 Exynos 7870 智能手机的三重支持，但 XDA 的开发者社区已经设法做到了这一点。

**[访问 XDA 项目三宝论坛](https://forum.xda-developers.com/project-treble)**

基于 XDA 认可开发人员 [ananjaser1211](https://forum.xda-developers.com/member.php?u=4637718) 、XDA 成员 [SPARTANICUS](https://forum.xda-developers.com/member.php?u=10011205) 和 XDA 资深成员 [Valera1978](https://forum.xda-developers.com/member.php?u=2047373) 的贡献，XDA 认可开发人员 [Astrako](https://forum.xda-developers.com/member.php?u=6917540) 创建了一个自动化分区工具和一个针对 Exynos 7870 平台的统一供应商内核组合。定制内核( **H-Kernel** )基于用于[三星 Galaxy A6 (2018)](https://www.xda-developers.com/samsung-galaxy-a70s-update-android-10-one-ui-2-0/) 的 Android 10 内核源代码，而名为“ **H-Vendor** ”的自制厂商分区则是从用于[三星 Galaxy J6](https://www.xda-developers.com/samsung-galaxy-j6-nokia-3-2-receive-stable-android-10-update/) 、 [Galaxy A7 (2018)](https://www.xda-developers.com/samsung-galaxy-a40-a80-a7-2018-android-10-one-ui-2-0-rollout/) 和 Galaxy S20 的 Android 10 固件移植而来。国防部使总共七部基于 Exynos 7870 的传统智能手机能够启动现有的 Android 10 [通用系统映像](https://www.xda-developers.com/tag/generic-systemimage/) (GSI)，并为基于 Android 11 的 GSIs 做好准备。

值得一提的是，离线充电和蓝牙通话在 H-vendor 的初始版本中被打破。此外，SELinux 在 H-Kernel 上被设置为许可的，不幸的是，这是一个主要的安全问题，我们希望很快得到解决。下面列出了特定于设备的已知问题:

需要更新的自定义恢复来执行供应商分区创建步骤，该步骤由**exy nos 7870 _ create vendor _ xx . zip**处理。尽管上述三星手机都没有采用 [A/B 双分区方案](https://www.xda-developers.com/how-a-b-partitions-and-seamless-updates-affect-custom-development-on-xda/)，但用户需要在刷新 H-Vendor zip 之前刷新 A/B ARM64 系统 GSI 映像。那些来自库存三星固件必须格式化数据分区(这将删除内部存储的内容)，然后再刷新这个模块，所以要执行完整的备份。

**[H-厂商和 H-Kernel 项目三重端口— XDA 下载讨论线程](https://forum.xda-developers.com/galaxy-j7/samsung-galaxy-j7-nxt--j701f-core-nxt-exynos-7870/treble-h-vendor-v1-0-t4116285)**