# 开发人员将 One UI 2.1 移植到采用 Exynos 7870 的三星 Galaxy 手机上

> 原文：<https://www.xda-developers.com/developer-ports-one-ui-2-1-galaxy-s20-features-several-samsung-galaxy-phones-exynos-7870/>

回到 2020 年 4 月，三星向 Galaxy J6 提供了 [Android 10 更新，没有](https://www.xda-developers.com/samsung-galaxy-j6-nokia-3-2-receive-stable-android-10-update/) [One UI 2.1 特定软件功能](https://www.xda-developers.com/samsung-bringing-galaxy-s20-software-features-s10-note-10-plus-one-ui-21/)。这款手机由 Exynos 7870 芯片组提供支持，这是一款 2016 年推出的 14 纳米八核 SoC，也为几款中端三星 Galaxy 手机提供支持。许多配备 Exynos 7870 的设备被排除在从三星获得官方 Android 10 更新[之外，尽管他们理论上能够运行它。为了填补这一空白，XDA 知名开发商 Astrako 现在已经为 Exynos 7870 平台编译了一个通用的 Android 10 ROM，其中包含了 Galaxy S20 系列的一系列 One UI 2.1 功能。](https://www.xda-developers.com/samsung-reveals-one-ui-2-0-android-10-update-schedule-galaxy-smartphones/)

被称为 **H-ROM** 的 [GSI](https://www.xda-developers.com/tag/generic-systemimage/) 风格 ROM 兼容七款传统 Exynos 7870 驱动的三星智能手机，包括 Galaxy A3 (2017)和 Galaxy J5/J6/J7 的不同版本。ROM 的基础取自 Galaxy S20 5G，而开发商则从 Galaxy S10 推出了一款经过修改的 CSC，可以实现原生通话记录等功能。整个包依赖于由同一个开发者为这些设备进行的[非官方项目三重实现。](https://www.xda-developers.com/developers-project-treble-samsung-galaxy-exynos-7870/)

搭载[2020 年 7 月](https://www.xda-developers.com/july-2020-android-security-update-google-pixel-samsung-galaxy-s20/) Android 安全补丁，最新版本的 *H-ROM* 足够稳定，可以作为日常驱动。不过，这款相机有一些已知的小故障，内置的 [**H-Kernel**](https://gitlab.com/android_samsung_universal7870/common/android_kernel_samsung_exynos7870/-/tree/oneui_q) 让 SELinux 处于许可模式，这是一个主要的安全问题。如果您想要 root 访问，最好选择 Magisk 的 Canary 版本。在这个 ROM 的当前版本上闪烁 Magisk stable 会给你一个引导循环，所以现在避免它。

* * *

## 下载只读存储器

一旦你成功地将你的设备增加三倍并安装了 **H-Vendor** ，你必须在刷新 *H-ROM* ZIP 之前完全擦除它。没有特定于设备的版本，因为统一安装程序足够智能，可以检测型号并应用适当的模块。 *H-ROM* 的基本版本针对系统分区较小的设备进行了优化。开发者提供了一个单独的 Samsung stock 应用程序包，用于侧向加载。

**三星 Exynos 7870 设备的 H-ROM:[one Drive](https://1drv.ms/u/s!AlW_pXiDXt9bjAJTSrLTDVEf9DDm?e=EfSVX2)| |[Google Drive](https://drive.google.com/drive/folders/1nvrCOT-1_q_Ax1GtiUs2pOxuly_paY3l)| |[MEGA](https://mega.nz/folder/QI92hIzZ#JV7YFmBiOjj7tgiUNj-9Ow)**

具体型号的讨论线索如下: