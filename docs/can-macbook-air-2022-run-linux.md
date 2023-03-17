# 在 MacBook Air (2022)上运行 Linux 的方式

> 原文：<https://www.xda-developers.com/can-macbook-air-2022-run-linux/>

2022 年 7 月，苹果公司发布了最新的 MacBook Air，搭载了 macOS Monterey 和 M2 芯片。近年来，苹果已经从英特尔转而使用自己的 ARM 处理器，人们普遍担心这意味着在 Mac 上运行 Linux 不再可能。我们是来告诉你好消息和坏消息的。

与之前的 M1 驱动的 MacBook Air 一样，最新一代目前不能在裸机上运行 Linux。这意味着你不能在 MacBook Air 上安装 Linux，就像你不能在台式电脑上安装唯一的操作系统一样，也不能在 macOS 旁边安装一个双重启动配置的操作系统。

然而，有多个项目致力于将 Linux 移植到苹果芯片上，一直到在 Linux 内核本身中构建支持。一个这样的项目是 [Asahi Linux](https://asahilinux.org/) ，它目前在 alpha 版中可用于一些 M1 驱动的 MAC 电脑。本质上，尤其是在 MacBook Air (2022 年)的早期，对 Linux 的裸机支持应该被认为是不可行的。

因此，我们必须转向虚拟化。

## 虚拟化 Linux 是 MacBook Air (2022)的发展方向

幸运的是，虚拟机很大程度上是苹果硅机器上的一个东西，并且有不止一种方法可以做到这一点。在 WWDC，苹果概述了使用 macOS 内置的虚拟化框架来引导 Linux 虚拟机。

这需要一点 Swift 编码的工作，但是，它是免费使用的，很可能是最好的整体性能。苹果为 Linux 虚拟化的 macOS Ventura 增加了一些性能增强，包括 virtio。此外，Rosetta 2 将允许 Linux 调用 x86_64 二进制文件，并将它们转换到 ARM。就像在 macOS 上做的一样。

需要注意的是，你必须使用一个 ARM 友好的 Linux 发行版(或“发行版”)，这样就可以排除你最喜欢的。但是 ARM 也有一些大牌，包括 Ubuntu 和 Debian。或者，使用虚拟化框架的是来自 Parallels、UTM 和 [VMWare](https://www.vmware.com/uk/products/fusion.html) 等公司的更加用户友好的工具。

或者，你也可以选择 [Parallels](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU42079/https://www.parallels.com/uk/pd/general/) ，但是这款要花钱，而且不便宜。你看到的是 100 美元的永久许可证，但它真的很好，很容易使用。同样，您将需要带有 ARM 版本的 Linux 发行版，但是 Parallels 让下载和安装它们变得非常简单。锦上添花的是 Coherence 模式，允许您在 Parallels 主窗口之外运行 Linux 应用程序，就好像它们是原生的 [Apple Silicon Mac 应用程序](https://www.xda-developers.com/best-apps-apple-silicon/)。

UTM 是另一个值得关注的虚拟化工具，它提供了其他工具目前没有的东西。在它的表皮下是 QEMU，一个非常古老但仍然非常好的工具。UTM 是免费和开源的，但 Mac 应用商店中的付费版本提供自动更新，并有助于支持开发。否则，无论你从哪里得到它都一样。

UTM 的优势还在于它能够在 ARM 上模拟 x86_64，尽管会有性能损失。运行基于 ARM 的 Linux 发行版，UTM 利用苹果虚拟化框架获得接近本地的速度。

* * *

所以，你肯定可以在最新的 MacBook Air 上运行 Linux，但它仍然局限于虚拟化。这在未来肯定会有所改进，但是对于需要能够引导到 Linux 的开发人员，甚至是那些希望两者都有，至少有一个相当简单的解决方案。MacBook Air (2022)是移动开发人员在 T2 最好的苹果电脑之一。

##### 苹果 MacBook Air (2022)

2022 款 MacBook Air 提供 M2 芯片、13.6 英寸显示屏和支持 MagSafe 3 的重新设计的机箱。它功能强大，几乎可以处理任何类型的工作。