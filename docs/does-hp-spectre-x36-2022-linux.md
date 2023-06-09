# 惠普 Spectre x360 运行 Linux 吗？你能安装它吗？

> 原文：<https://www.xda-developers.com/does-hp-spectre-x36-2022-linux/>

惠普最近推出了 Spectre x360 的 [2022 更新版，这是一对很有前途的设备。他们本质上是建立在市场上已经有的一些](https://www.xda-developers.com/hp-spectre-x360-2022/)[最好的笔记本电脑](https://www.xda-developers.com/best-laptops/)之上的——现在有了更新的处理器和一些其他升级。但是，就像大多数笔记本电脑一样，HP Spectre x360 配备了 Windows，有些人可能更喜欢 Linux。如果你是其中之一，你会很高兴知道有多种方法可以在你的新笔记本电脑上安装 Linux。

事实上，如果你需要运行一些 Linux 应用程序，你甚至不需要安装完整的操作系统。让我们来看看可用的选项。

## 用于 Linux 的 Windows 子系统

Windows 子系统 for Linux (WSL)最初是在 Windows 10 中推出的，它可能是在 HP Spectre x360 上运行 Linux 应用程序的最简单方式，无需移除 Windows，甚至无需离开它。有了 Windows 11，WSL 甚至可以运行基于图形用户界面的 Linux 应用程序，它们可以在你电脑上的 Windows 应用程序旁边打开。这是通过虚拟化实现的，但你绕过了创建虚拟机可能带来的一些麻烦，而且一切都集成到一个单一的体验中。

为了以这种方式运行 Linux 应用程序，您首先需要从微软商店安装 Linux 的 Windows 子系统(预览版),然后重新启动您的 PC。一旦完成，你可以回到微软商店，找到你喜欢的 Linux 发行版。有几个选项可用，包括 Ubuntu、Kali Linux 等等。运行 Linux 操作系统本身通常会在命令行界面中进行，但如果你安装了一个基于 GUI 的应用程序，你可以打开它并在你的其他应用程序旁边看到它，如下图所示。

不过，这确实意味着你无法获得完整的 Linux 体验，使用 Linux 桌面和所有这些东西。但是，如果您只想在 HP Spectre x360 上运行特定的 Linux 应用程序，WSL 是最方便的方法。另外，如果你还需要的话，你不必离开 Windows。

## 在 HP Spectre x360 上安装 Linux

如果您确实想要更完整的 Linux 体验，从技术上讲，您可以在 HP Spectre x360 上实现，并且有几种方法可以实现。如果你想让 Windows 继续作为你的主操作系统，你可以创建一个虚拟机，或者你可以尝试双引导。

创建虚拟机是更无风险的方法，尽管这意味着您会损失一些性能。虚拟化需要大量资源，所以您会注意到它不如正常运行操作系统那么快。不过，有了虚拟机，你可以获得完整的 Linux 桌面体验和所有你想安装的应用程序，这也是熟悉操作系统的好方法。你需要使用虚拟化软件，比如 Hyper-V(在 Windows 11 Pro 中)或 VMware Workstation Player，然后下载你喜欢的 Linux 发行版的 ISO，比如 Ubuntu。我们有一个关于如何创建 Windows 11 虚拟机的指南，你通常可以遵循相同的步骤，只需使用你选择的 Linux ISO。

如果你想以完全的本机性能运行 Linux，那么你可能想在你的 PC 上尝试双启动 Linux 和 Windows 11。这样做的缺点是，每次你想切换操作系统时，你都必须重启笔记本电脑，但当你运行它们时，两者都可以本地运行，不会有任何性能损失。例如，如果你想在工作中使用 Linux，在游戏中使用 Windows，这可能是一个不错的设置。我们还有一个关于如何在同一台电脑上双启动 Windows 11 和 Linux 的指南，所以我们建议查看一下。如果你发现你更喜欢一直使用 Linux，你可以在以后删除你的 Windows 分区(尽管你需要备份你的数据)。请注意，您将无法获得惠普对 Linux 的支持，因为它没有得到官方支持。

* * *

如果你有兴趣购买惠普 Spectre x360 (2022)，你可以使用下面的链接。这些是惠普制造的最好的笔记本电脑中的一些，根据不同类型的用户对功能和便携性的需求来迎合他们。

 <picture>![The HP Spectre x360 13.5 is a premium convertible laptop with a stunning deisng and great performance for everyday tasks.](img/3116aac455db3b2da28af3fcd8c8a579.png)</picture> 

HP Spectre x360 13.5

##### 惠普 Spectre x360 13.5

2022 HP Spectre x360 13.5 采用 3:2 显示屏和 10 核 12 线程的第 12 代英特尔处理器。它可以直接运行 Windows，但也有运行 Linux 应用的方法。

 <picture>![The HP Spectre x360 16 is a powerful convertible laptop with high-end processors and discrete graphics, plus a fantastic display.](img/51e1b3dba34e25ccec1221618101e2b4.png)</picture> 

HP Spectre x360 16

##### 惠普 Spectre x360 16 (2022)

HP Spectre x360 配备了一个 16:10 的大显示屏，您可以根据自己的需求选择 28W 和 45W 处理器。通过一些工作，你也可以在上面运行 Linux 应用程序。