# MacBook Pro 13 (2022)可以运行 Windows 吗？技术上来说，是的

> 原文：<https://www.xda-developers.com/can-macbook-pro-13-2022-run-windows/>

苹果最近推出了 MacBook Pro 13 的 [2022 年更新，它主要集中在新的苹果 M2 芯片上。这种新一代的苹果硅带来了显著改善的性能，但它仍然基于 Arm 技术，这意味着存在一些限制。其中之一就是能够像英特尔机型一样运行 Windows。2022 年的 MacBook Pro 13 实际上可以运行 Windows，但现在这是一个更加繁琐的过程。](https://www.xda-developers.com/macbook-pro-2022/)

最大的原因是，根本没有一个版本的 Windows 可以在 Arm 设备上运行，至少不是一个你可以自己下载的产品。Windows 可用于采用 Arm 处理器的设备，但获得它的唯一方法是购买一台开箱即可在 Arm 上运行 Windows 的设备。可能正因为如此，苹果也没有将 Boot Camp 作为苹果硅 MAC 电脑上 macOS 的一部分。这意味着你在 MacBook Pro 上运行 Windows 的传统方法已经过时了，但你仍然有办法做到这一点。

## 如何在 MacBook Pro 13 (2022)上运行 Windows 11

这可能不是理想的方法，但有一种方法可以在 MacBook Pro 13 上运行 Windows 11，这都要归功于虚拟化和 Parallels Desktop 17 的强大功能。如果您不熟悉的话，Parallels Desktop 是已经问世一段时间的 Mac 虚拟化软件，它提供了一种在 Mac 上运行操作系统的方式，而无需完全的双启动设置。你可以启动一个虚拟机来访问你想要使用的操作系统。并且有了最新版本，Parallels Desktop 17，支持苹果硅 MAC，包括可以运行 Windows 10 或 11。

所以您首先需要的是 Parallels Desktop 17 许可证。该软件基于订阅的价格为每年 79.99 美元，但你可以以 99.99 美元的价格购买标准版的永久许可证，其中不包括未来的重大更新或高级支持。

但是你如何解决 Arm 缺少 Windows 版本的问题呢？这就是 Windows Insider 程序发挥作用的地方。微软确实提供了 Windows on Arm 的下载，但只是作为预装操作系统的虚拟硬盘。您可以在 Windows Insider 下载网页上下载最新版本。这是一个开发中的操作系统版本，这意味着你肯定会遇到一些问题，但如果你能忍受一段时间，你最终可以进入一个稳定的版本，并选择退出内部计划。当然，你还需要一个 Windows 许可证，尽管这一直是个问题。

一旦您完成所有这些，您就可以运行 Parallels Desktop 17 并创建一个新的虚拟机，加载您刚刚下载的虚拟硬盘文件。如果你需要如何设置的分步说明，我们有一个关于如何在苹果硅 MAC 电脑上运行 Windows 10 的指南，同样的步骤也适用于 Windows 11。完成操作系统安装后，你需要转到 Windows 中的设置应用，并使用许可证密钥激活 Windows。

你还可以去设置应用的**窗口更新**部分，然后去**窗口内部程序**。选择在下一版本 Windows 发布时**取消注册该设备的选项。这将使得当 Windows 11 的下一个主要更新可用时，您的虚拟机将停止接收内部版本，您可以保持稳定的操作系统版本。**

* * *

的确，在 13 英寸 MacBook Pro (2022)上运行 Windows 现在有点麻烦，而且启动成本更高，因为你还需要 Parallels Desktop 许可证。但是，如果你真的需要一些 Windows 应用程序，而又不放弃苹果芯片的性能和效率，这是一种方法。虚拟化确实会带来一些性能成本(这就是为什么我们通常建议运行为苹果芯片设计的[应用)，但苹果 M2 处理器足够快，仍然可以流畅地运行 Windows。](https://www.xda-developers.com/best-apps-apple-silicon/)

有兴趣的可以看看下面这款 MacBook Pro 13 寸(2022)。这是目前市面上最好的苹果电脑之一，尽管它的设计没有改变。您也可以在下面购买 Parallels Desktop 和 Windows 11 许可证。

 <picture>![The 2022 MacBook Pro comes with the new Apple M2 processor, delivering even more performance than the M1 model.](img/e4a8883c71bef24fedaac615318f305b.png)</picture> 

MacBook Pro (2022)

##### 苹果 MacBook Pro 13 英寸(2022)

2022 款 MacBook Pro 配备了新的苹果 M2 处理器，性能甚至超过了 M1 型号。它不能原生运行 Windows，但有替代选项。

 <picture>![Parallels Desktop virtualization software for running Windows or Linux on macOS. The latest version also supports Apple Silicon Macs and Windows on Arm.](img/860b397f9ada5cc74cb9a18adfa6dc9a.png)</picture> 

Parallels Desktop

##### Parallels 桌面

用于在 macOS 上运行 Windows 或 Linux 的 Parallels Desktop 虚拟化软件。最新版本还支持苹果 Silicon Macs 和 Arm 上的 Windows。

 <picture>![Product key to activate Windows 11.](img/f0aac100e17e9826034b1e979981bd93.png)</picture> 

Windows 11 Home

##### Windows 11 主页

激活 Windows 11 的产品密钥。