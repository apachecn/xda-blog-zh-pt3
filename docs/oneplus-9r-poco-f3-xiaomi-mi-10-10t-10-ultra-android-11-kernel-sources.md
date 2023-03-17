# 一加 9R 和 POCO F3 内核源代码现已推出

> 原文：<https://www.xda-developers.com/oneplus-9r-poco-f3-xiaomi-mi-10-10t-10-ultra-android-11-kernel-sources/>

除了旗舰智能手机[一加 9](https://www.xda-developers.com/oneplus-9/) 和[一加 9 Pro](https://www.xda-developers.com/oneplus-9-pro-review/) 之外，一加还推出了一款更实惠的型号，名为[一加 9R](https://www.xda-developers.com/oneplus-9r-launch/) 。这款印度专用设备的规格有所变化，以满足较低的价格，同时仍然保留了一些重要的部分，以符合 9 系列徽章的要求。如果你打算只为售后市场开发而购买这款手机，那么你会很高兴地知道，该公司已经发布了该设备 OxygenOS 软件附带的 Linux 内核二进制文件的内核源代码。

一加 9R 搭载了高通新的[骁龙 870](https://www.xda-developers.com/qualcomm-unveils-snapdragon-870/) 芯片，这是对去年旗舰 SoC——骁龙 865 的一次小升级。除了速度更快的 prime 内核之外，这两种 SOC 之间唯一的根本区别是支持的蓝牙版本。这就是为什么一加在与[一加 8T 版本](https://www.xda-developers.com/oneplus-8t-kernel-source-code-unbrick-tool/)相同的分支中发布了一加 9R 的内核源代码，它本身驻留在[一加 8/8 Pro 的 Android 11 内核源代码树](https://www.xda-developers.com/oneplus-releases-kernel-sources-android-11-update-oneplus-8-pro/)中。

**[一加 9R 内核来源](https://github.com/OnePlusOSS/android_kernel_oneplus_sm8250/commit/5fa9472bc20be3fd57ff6bfadac53ce8bc2ed43a)**

小米还通过发布几款新发布的基于高通骁龙 870 SoC 的设备的内核源代码，更新了其 Github 知识库。其中， [Redmi K40](https://www.xda-developers.com/redmi-k40-launched-china/) 上个月在中国首次亮相，搭载了基于 Android 11 的 MIUI 12。就在几天前，这款名为 POCO F3 的手机在全球发布。米 10S 是最近在中国推出的另一款骁龙 870 设备，尚未在全球发布。

**[XDA 动手:POCO F3 拥有旗舰级别的触觉和屏幕，整整少了一大截](https://www.xda-developers.com/poco-f3-hands-on/)**

最后，我们有一个 Mi 10 家族的主要子集，中国 OEM 已经发布了一组针对 Android 11 的新内核源代码。值得注意的是，所有这些设备都由骁龙 865 SoC 供电。完全没有必要处理[小米过于隐晦的命名惯例和令人困惑的更名](https://www.xda-developers.com/opinion-smartphone-branding-out-of-control/)，因为你可以参考下表来清楚地了解这些发布。

具有适当提交历史的内核源代码版本对于售后开发场景非常有帮助。修改社区可以修改代码，通过修补现有内核来提高设备的整体性能。此外，这种版本还帮助开发者为设备构建 TWRP 和端口流行的定制 ROM(例如 [LineageOS](https://www.xda-developers.com/tag/lineageos/) ),这反过来又有利于对现有 ROM 不满意的用户。