# MacBook Air (2022)可以运行 Windows 吗？是的，但是它需要一些工作

> 原文：<https://www.xda-developers.com/can-macbook-air-2022-run-windows/>

苹果公司最近推出了第二代苹果芯片，从[苹果 M2](https://www.xda-developers.com/apple-m2-launch/) 芯片开始。这种新处理器首次出现在[全新 MacBook Air](https://www.xda-developers.com/macbook-air-2022/) 中，它比上一代产品有了一些重大的性能改进。但苹果芯片仍然相对较新，这种基于 Arm 的架构有很多不同之处。所以，你可能想知道 2022 款 MacBook Air 能否运行 Windows。嗯，是可以，但是没你想的那么简单。

首先，苹果已经将 Boot Camp 从苹果硅 MAC 电脑中完全移除。Boot Camp 是在 MAC 上运行 Windows 的主要方式，所以这让事情变得有点复杂，因为你现在必须依赖第三方软件。你还需要一个能在 Arm 处理器上运行的 Windows 版本。虽然微软确实为 Arm 开发了 Windows，但它不能下载——唯一的官方途径是购买一台已经安装了 Windows 的 Arm 设备。

这意味着需要一些变通办法，但在 MacBook Air 上运行 Windows 在技术上是可能的。为此，您需要 Parallels Desktop 的帮助，这是一款付费软件，这意味着您不仅需要购买 Windows 许可证，还需要购买 Parallels Desktop 许可证。

## 如何在 MacBook Air 上安装 Windows

正如我们提到的，要在 2022 年的 MacBook Air 上运行 Windows，你需要的第一件事就是获得 [Parallels Desktop 17](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU42046/https://www.parallels.com/products/desktop/) 的许可。这是 Parallels- virtualization 软件的最新版本，这里的关键是它正式支持苹果硅 MAC 上的 Windows 10 和 11。这意味着，如果你有任何问题，你可以期待该公司继续提供支持和技术援助。Parallels Desktop 17 作为订阅服务提供，每年起价 79.99 美元。标准版也可以一次性购买，价格为 99.99 美元，但这意味着您无法获得 24/7 高级支持或升级到最新版本。

接下来，你需要下载 Windows，但是正如我们提到的，你不能以一种典型的方式为 Arm 设备下载 Windows。为 Arm 下载 Windows 的唯一途径是通过 Windows Insider 程序。如果你进入 [Windows Insider 预览下载页面](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewarm64)，你可以下载一个 VHDX 文件，基本上就是一个已经安装了 Windows 11 的虚拟硬盘。但因为这是 Insider 计划的一部分，所以它不是 Windows 11 的最终版本——它是一个预览版，这意味着你可能会遇到一些稳定性问题。当然，你还需要一个 Windows 许可证。

一旦你有了这些东西，开始就相当容易了。您可以启动 Parallels Desktop 并创建新的虚拟机(VM)，选择您的 VHDX 文件作为其映像。关于如何在苹果电脑上安装 Windows 系统，我们有更详细的指南[。如果你需要如何设置它的一步一步的指导，你可能想看看它。请记住，本指南侧重于 Windows 10，但创建虚拟机的过程本质上是相同的。](https://www.xda-developers.com/windows-10-apple-silicon-mac/)

一旦你设置了虚拟机，你需要进入 Windows 11 上的设置应用程序，并进入**激活**页面(在**系统**部分)输入你的许可证密钥，以激活 Windows。你可能想做的其他事情是进入 **Windows Update** 部分，然后选择 **Windows Insider Program** 。从这里，打开选项**在下一个版本的 Windows 发布**时取消注册该设备。这将使你不再收到内部版本，一旦下一个主要版本的 Windows 可用，所以你可以实际安装一个稳定版本的 Windows。

* * *

事实上，在 2022 年的 MacBook Air 或任何由苹果芯片驱动的 Mac 上运行 Windows 比在基于英特尔的 Mac 上更麻烦、更昂贵，但这种选择确实存在。如果你喜欢新的 MacBook Air，但你需要特定的 Windows 应用程序，这是你唯一的解决方案。否则，你可以试着[买一台翻新的旧 MacBook Air](https://www.xda-developers.com/best-places-buy-refurb-macbook-air/) ，或者换一台 Windows 笔记本电脑——Windows 领域也有很多[很棒的笔记本电脑](https://www.xda-developers.com/best-laptops/)。

 <picture>![The latest MacBook Air from Apple featuring its M2 processor](img/2d91b63728e352151b7d0bb0af574cda.png)</picture> 

MacBook Air M2 2022

##### 苹果 MacBook Air (M1，2020 年)

2022 年的 MacBook Air 由新的苹果 M2 芯片驱动，另外它有一个新的更高的显示屏和全新的设计。

 <picture>![Parallels Desktop virtualization software for running Windows or Linux on macOS. The latest version also supports Apple Silicon Macs and Windows on Arm.](img/860b397f9ada5cc74cb9a18adfa6dc9a.png)</picture> 

Parallels Desktop

##### Parallels 桌面

用于在 macOS 上运行 Windows 或 Linux 的 Parallels Desktop 虚拟化软件。最新版本还支持苹果 Silicon Macs 和 Arm 上的 Windows。

 <picture>![Product key to activate Windows 11.](img/f0aac100e17e9826034b1e979981bd93.png)</picture> 

Windows 11 Home

##### Windows 11 主页

激活 Windows 11 的产品密钥。