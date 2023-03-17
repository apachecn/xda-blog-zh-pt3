# 三星 Galaxy S23 Ultra 获得非官方 TWRP 端口

> 原文：<https://www.xda-developers.com/samsung-galaxy-s23-ultra-twrp-unofficial/>

TeamWin Recovery Project，或者简称为 [TWRP](https://www.xda-developers.com/how-to-install-twrp/) ，是目前为止 Android 修改场景中最流行的定制恢复解决方案。虽然这些年来修补爱好者已经明显减少，但仍然有人致力于这种工艺，这意味着最近的旗舰接收 TWRP 港是一件相当大的事情。这正是发生在 [Galaxy S23 系列](https://www.xda-developers.com/samsung-galaxy-s23/)上的事情，XDA 资深成员 [afaneh92](https://forum.xda-developers.com/m/afaneh92.4770483/) 已经设法为三星的最新产品提供了一个几乎功能性的 TWRP 构建。

当谈到 Galaxy S 系列时， [Exynos 与骁龙](https://www.xda-developers.com/samsung-flagship-cpu-performance-exynos-vs-snapdragon/)一直是一个大话题——无论是在普通消费者还是在售后开发圈。韩国 OEM 厂商过去在比骁龙更多的地区销售 Exynos 变体。此外，美国和加拿大骁龙型号的引导加载程序无法解锁，这一设计基本上迫使大多数修改工作围绕 Exynos 驱动的版本进行。随着 Galaxy S23 系列的出现，这种情况发生了变化，因为所有地区的变体现在都由经过修改的骁龙 8 Gen 2 芯片组提供支持。因此，您不再需要为 Galaxy S 系列处理两套独立的 TWRP 版本。

目前，非官方的 TWRP 只兼容 [Galaxy S23 Ultra](https://www.xda-developers.com/samsung-galaxy-s23-ultra-review/) ，准确地说是 SM-S918B 型号。这一发展是一项重要成就的原因有很多。首先， *afaneh92* 依靠设备自带的股票内核编译恢复镜像。由于三星尚未公布 Galaxy S23 系列的内核源代码，开发者无法查看实际的代码库。不支持处理加密例程，并且您不能读/写 EROFS 格式的分区，但是其余的功能应该可以正常工作。

**[下载三星 Galaxy S23 Ultra 的非官方 TWRP](https://forum.xda-developers.com/t/4551215/)**

请务必通读逐步安装说明，以避免遇到引导循环或其他问题。即使你有一个引导加载程序可解锁的 Galaxy S23 型号，请记住，安装第三方二进制文件(如 TWRP) **会不可逆转地触发 Knox 保修位**并且**会禁用后续 OTA 更新**，因此请谨慎操作。

**XDA 论坛:[三星 Galaxy S23](https://forum.xda-developers.com/f/samsung-galaxy-s23.12707/)| |[Galaxy S23 Plus](https://forum.xda-developers.com/f/samsung-galaxy-s23-plus.12709/)| |[Galaxy S23 Ultra](https://forum.xda-developers.com/f/samsung-galaxy-s23-ultra.12713/)**

Galaxy S23 Ultra 是市场上最好的手机之一，装有全新的 200MP 传感器，精致的设计，为 Galaxy 芯片组定制的骁龙 8 Gen 2，以及一个 UI 5.1。