# 三星 Galaxy S22 内核源代码现已推出

> 原文：<https://www.xda-developers.com/samsung-galaxy-s22-kernel-sources/>

在几乎所有关于三星 2022 年旗舰的信息都被泄露后，Galaxy S22 系列终于在上个月正式发布。这些手机代表了韩国 OEM 厂商今年在不同价格区间所能提供的最佳产品。我们[评测了 12GB 内存的 Galaxy S22 Ultra](https://www.xda-developers.com/samsung-galaxy-s22-ultra-review/) ，它为你能想到的任何用例提供了真正巨大的潜力。随着可用性的逐渐上升，我们一定会看到售后开发工作和定制修改开始为设备三重奏回升。正如预期的那样，三星现在已经发布了 Galaxy S22、Galaxy S22 Plus 和 Galaxy S22 Ultra 的内核源代码。

三星 Galaxy S22 系列在欧洲和少数亚洲国家采用该公司内部的 Exynos 2200 芯片。另一方面，骁龙 8 代 1 变种在北美、拉丁美洲、非洲、大洋洲和包括印度在内的大多数亚洲地区都有。就像任何其他 Android 设备版本一样，该公司必须发布其内核源代码，以符合 Linux 内核所受的 GPLv2 许可。三星已经做到了这一点，但到目前为止只针对 Exynos 变种。

如果你是一名开发人员，你现在可以前往三星开源发布中心，访问 Galaxy S22 (SM-S901B)、Galaxy S22 Plus (SM-S906B)和 Galaxy S22 Ultra (SM-S908B)的 Exynos 型号的内核源代码。初始版本基于软件版本 **S90xBXXU1AVA7** (普通 Galaxy S22 的 **AVA8** )。

由于 Galaxy S22 出厂时附带了一个 UI 4.1，因此内核源代码基于 Android 12。虽然每个型号都有单独的版本，但从技术上来说，通过组合相关的软件包来创建特定于 SoC 的统一树是可能的。

 <picture>![The vanilla Galaxy S22 offers powerful, flagship-level hardware in a compact package.](img/704caf448897c4cc21eb33ea04eececf.png)</picture> 

Samsung Galaxy S22

三星 Galaxy S22 是 2022 年的入门级旗舰产品，以适合许多口袋和预算的形式带来了顶级的性能和相机功能。

 <picture>![The Galaxy S22 Plus has a larger 4,5000mAh battery, and it supports 15W wireless charging.](img/2b6ba4ab9129d27fc50e575207b4dc61.png)</picture> 

Samsung Galaxy S22 Plus

##### 三星 Galaxy S22 Plus

三星 Galaxy S22 Plus 在高端机身中提供了可靠性能和强大功能的良好组合。

 <picture>![The Galaxy S22 Ultra has an even bigger 5,000mAh battery and it supports 15W wireless charging.](img/5fa0decfdccca6f3403821fdeed75792.png)</picture> 

Samsung Galaxy S22  Ultra

三星 Galaxy S22 Ultra 结合了 S 和 Note 系列的精华，是一款强大的机器，适合工作和娱乐。

有了内核源代码，开发人员可以开始移植流行的 TWRP 定制恢复，开发定制内核，并为上述设备发布定制 rom。然而，只有当设备的引导加载程序不可锁定时，这样的模块才是有用的，遗憾的是，对于一些骁龙驱动的型号来说，情况并非如此。您仍然可以查看特定于模型的 XDA 论坛，关注开发现场。

**XDA 论坛:[三星 Galaxy S22](https://forum.xda-developers.com/f/samsung-galaxy-s22.12511/)| |[Galaxy S22 Plus](https://forum.xda-developers.com/f/samsung-galaxy-s22-plus.12513/)| |[Galaxy S22 Ultra](https://forum.xda-developers.com/f/samsung-galaxy-s22-ultra.12515/)**

* * *

**来源:** [三星开源发布中心](https://opensource.samsung.com/main)