# MacBook Pro 13 (2022)可以运行 Linux 吗？

> 原文：<https://www.xda-developers.com/can-macbook-pro-13-2022-run-linux/>

除了全新的 MacBook Air T1，苹果还在 2022 年 WWDC 发布了 MacBook Pro 13 T3 的 T2 更新版。与 MacBook Air 不同，最新的 MacBook Pro 13 没有获得更新的设计，它只是有一些更有活力的内部部件，包括全新的[苹果 M2](https://www.xda-developers.com/apple-m2-launch/) 芯片。

这是第一款内置 M2 的 MacBook Pro，也是最实惠的 MacBook Pro，对于各种使用情况来说，这是一个有吸引力的提议。这包括发展。

开发人员通常希望能够在他们的 Mac 上运行 Linux，无论是本机运行还是虚拟化运行。好消息是，在 MacBook Pro 13 (2022)上运行 Linux 是完全可能的，但有一些警告。

## MacBook Pro 13 (2022)不会原生运行 Linux

和之前的 MacBook 一样，MacBook Pro 13 目前不能在裸机上运行 Linux。即使有基于 ARM 的 Linux 发行版，现在你也不走运。

有多个项目致力于将 Linux 移植到苹果芯片上，一直到在 Linux 内核本身中构建支持。一个这样的项目是 Asahi Linux，它目前在一些 M1 驱动的 MAC 电脑上有 alpha 版本。但是，即使这样，也远远不能用于生产机器。

本质上，原生安装 Linux 应该被认为是不可行的。因此，我们必须转向虚拟化。那里的消息要好得多。

## 运行 Linux 虚拟机的各种方法

虚拟机在苹果芯片上是非常可能的，有几种方法可以做到。在 WWDC，苹果概述了使用 macOS 内置的虚拟化框架来引导 Linux 虚拟机。这需要一点 Swift 编码的工作，但它是免费使用和最好的整体性能。

需要注意的是，你必须使用带有 ARM 版本的 Linux 发行版，这样就可以排除你最喜欢的版本。但是 ARM 也有一些大牌，包括 Ubuntu 和 Debian。但是虚拟化框架不会模拟在 ARM 上使用的 x86_64 Linux 发行版。

[VMware Fusion](https://www.vmware.com/products/fusion.html) 适用于 Apple Silicon，允许您运行 Linux 虚拟机。最新版本可从 VMware 网站下载。

或者，你可以选择[平行线](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU42058/https://www.parallels.com/uk/pd/general/)，但是要付出代价。你看到的是 100 美元的永久许可证，但它工作良好，易于使用。同样，您需要带有 ARM 版本的 Linux 发行版，但是 Parallels 让下载和安装它们变得非常简单。锦上添花的是 Coherence 模式，允许您在 Parallels 主窗口之外运行 Linux 应用程序，就好像它们是 Mac 的原生程序一样。目前这是 Parallels 独有的功能，可能值回票价。

[UTM](https://mac.getutm.app/) 是另一个值得关注的虚拟化工具，它提供了其他人目前没有的东西。在它的表皮下是 QEMU，一个非常古老但仍然非常好的工具。UTM 是免费和开源的，但 Mac 应用商店中的付费版本提供自动更新，并有助于支持开发。UTM 还能够在 ARM 上模拟 x86_64，尽管会有性能损失。在基于 ARM 的 Linux 发行版中，UTM 利用苹果虚拟化框架实现了接近原生速度的速度。

* * *

像所有 T4 最好的苹果电脑一样，MacBook Pro 是一款受欢迎的开发者笔记本电脑，即使过渡到苹果芯片，它仍然完全有可能使用 Linux。熟悉 Apple 的虚拟化框架可能是一个好主意，但是如果您不喜欢编写自己的配置，还有许多好的替代方案。

MacBook Pro 13 (2022)现已上市，但如果你想节省一些钱，你可以尝试现在就购买一台[已加油的 MacBook Pro](https://www.xda-developers.com/best-places-buy-refurb-macbook-pro/) 。

 <picture>![The 2022 MacBook Pro comes with the new Apple M2 processor, delivering even more performance than the M1 model.](img/e4a8883c71bef24fedaac615318f305b.png)</picture> 

MacBook Pro (2022)

##### 苹果 MacBook Pro 13 英寸(2022)

苹果公司的最新芯片出现在苹果 MacBook Pro 13 (2022)中，让你不在办公桌前也能完成更多工作。