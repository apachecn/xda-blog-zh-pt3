# 谷歌 Pixel 6 和 Pixel 6 Pro 获得第一个定制内核

> 原文：<https://www.xda-developers.com/google-pixel-6-6-pro-first-custom-kernel/>

谷歌 Pixel 6 和 Pixel 6 Pro T1 在 2021 年下半年大出风头。谷歌决定加入内部硅俱乐部，这无疑让许多用户感到惊讶，第一代张量芯片[已经证明](https://www.xda-developers.com/google-tensor-pixel-6-call-screen-voice-typing/)足够强大[成为关注的焦点。Pixel 6/6 Pro 的工厂图像、内核源代码和设备树也已经](https://www.xda-developers.com/face-unblur-pixel-6/)[发布](https://www.xda-developers.com/google-pixel-6-6-pro-factory-images-kernel-source-code/)，这正是改装爱好者开始玩设备二人组所需的正确成分。现在，Pixel 6 家族的第一个定制内核已经登陆我们的论坛，这要归功于 XDA 公认的开发者兼贡献者 [Freak07](https://forum.xda-developers.com/m/freak07.3428502/) 。

**[谷歌 Pixel 6 Pro 评测:不可否认的 Exynos 灵感的奇妙日常手机](https://www.xda-developers.com/google-pixel-6-pro-review/)**

Freak07 的 Kirisakura 内核在[定制内核](https://www.xda-developers.com/most-popular-custom-kernels-for-android/)开发场景中已经是一个受欢迎的名字，Pixel 6 的加入——尽管目前只是一个“预览”版本——肯定会帮助该项目增加其用户群。然而，我们应该注意到 Kirisakura 自定义内核的当前版本的安装方式有一个显著的变化。谷歌正在新的 Android 设备上逐步实施通用内核映像(GKI)设计，这意味着构建一个传统的单片内核映像打包成一个 TWRP 可擦写的 ZIP 文件不再可行。这就是为什么定制内核的初始版本是作为一组映像提供的，并且你需要通过[快速启动](https://www.xda-developers.com/install-adb-windows-macos-linux/)来刷新它们。

以下是 Kirisakura kernel 为谷歌 Pixel 6 和谷歌 Pixel 6 Pro 提供的所有增强功能:

*   基于谷歌最新的 Android 12 内核源代码
*   Linux-稳定-上游包括到 5.10.44(股票是 5.10.43)
*   使用 [BBR](https://research.google/pubs/pub45646/) 作为默认的 TCP 拥塞算法
*   启用 TTL 欺骗支持
*   包括 [LRNG](https://github.com/smuellerDD/lrng)

**[Google Pixel 6/6 Pro 的 Kirisakura 内核——XDA 下载与讨论线程](https://forum.xda-developers.com/t/4358435/)**

在您尝试在 Pixel 6 或 Pixel 6 Pro 上安装 Kirisakura 内核之前，请记住进行设备外备份。那是因为你需要一个解锁的 bootloader 来启动，解锁过程**需要擦除手机上的所有数据，包括内部存储**上的文件。由于[安全网认证失败](https://www.xda-developers.com/safetynet-hardware-attestation-feature-here-to-stay/)，解锁引导程序后，您的银行应用也可能停止工作。幸运的是，在 Pixel 设备上恢复到库存配置非常容易，因为您只需要从匹配的工厂固件包中刷新适当的库存映像，并重新锁定引导加载程序。

**[谷歌 Pixel 6 XDA 论坛](https://forum.xda-developers.com/f/google-pixel-6.12311/) ||| [谷歌 Pixel 6 Pro XDA 论坛](https://forum.xda-developers.com/f/google-pixel-6-pro.12313/)**

 <picture>![The Pixel 6 comes with Google's new Tensor chip, a modern design, and flagship cameras.](img/7343f77af84019bd24844d3d2e495f29.png)</picture> 

Google Pixel 6

Pixel 6 配备了谷歌新的张量芯片、现代设计和旗舰相机。

 <picture>![The Pixel 6 Pro is the larger sibling that comes with Google's new Tensor chip, a modern design, and an extra telephoto camera.](img/5c825565a61d24d571df294787f045fc.png)</picture> 

Google Pixel 6 Pro

Pixel 6 Pro 是较大的兄弟，配有谷歌的新张量芯片、现代设计和额外的远摄相机。

* * *

**你打算在 Pixel 6/6 Pro 上运行定制内核或 ROM，还是继续使用现有固件？请在下面的评论中告诉我们！**