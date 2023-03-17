# Mac 工作室可以运行 Linux 吗？是的，但不是天生的

> 原文：<https://www.xda-developers.com/can-mac-studio-run-linux/>

苹果最新的桌面工作站 [Mac Studio](https://www.xda-developers.com/mac-studio/) 很有诱惑力。由于新的苹果 M1 超处理器，Mac Studio 可能是迄今为止最强大的 Mac，甚至可以与“奶酪刨丝器”Mac Pro 竞争。开箱即用，Mac Studio 将运行 [macOS Monterey](https://www.xda-developers.com/macos-monterey/) ，但如果你想在不同的操作系统中利用这种能力呢？如果你想知道你是否能在 Mac Studio 上运行 Linux，我们有好消息和坏消息要告诉你。

坏消息是仍然不可能在 macOS 上本地运行 Linux 或者 Windows。虽然基于英特尔的机型更容易安装不同的操作系统，但运行苹果芯片的 MAC 电脑则更受限制。这里的一线希望是，你可以在 Mac Studio 上运行 Linux，但必须通过一个虚拟机。

## 使用虚拟机在 Mac Studio 上运行 Linux

如果你真的想在 Mac Studio 上使用 Linux 发行版，你首先需要支持 Arm 架构的虚拟化软件。这里有一些选项，但是一个很棒的解决方案是 [Parallels Desktop 17](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU40440/https://www.parallels.com/products/desktop/) 。这种虚拟化软件允许你在 macOS 上运行 Windows、Linux 和其他操作系统，包括 Apple Silicon Macs。不过，这是付费软件，所以你必须支付至少 99.99 美元来获得永久许可，或者如果你想要订阅模式，每年支付 79.99 美元。

Parallels Desktop 实际上使在 macOS 上运行 Linux 变得非常容易，因为您可以选择下载您喜欢的 Linux 发行版，选项包括 Ubuntu、Fedora、Debian 或 Kali Linux。您也许可以使用其他发行版，但是您需要确保它们为 Arm 设备提供图像，而许多发行版都没有。大多数操作系统仍然是为 x86 或 AMD64 处理器设计的，所以您最好使用提供给您的映像之一。

这实际上比在 macOS 上使用 Windows 更容易，因为这需要你单独下载一个预览版的 Windows，然后自己进行设置(另外，你将不得不运行一个未完成的 Windows 版本)。在 Parallels 中运行 Linux 的另一个优势是您可以使用一种叫做 Coherence mode 的东西。这实际上使得在你的 Mac 应用旁边打开 Linux 应用成为可能，以至于你可以在 macOS dock 上看到你的 Linux 应用。你不必每次都进入 Linux 界面，这是你在 Windows 上做不到的。

如果你想要一个在 Mac Studio 上运行 Linux 的免费解决方案，另一个选择是使用一个名为 UTM 的应用。它可以在[UTM 官方网站](https://mac.getutm.app)上免费获得，或者在 Mac App Store 上售价 9.99 美元，它还为 Linux 提供了相对简单的设置。多亏了可用操作系统的[库](https://mac.getutm.app/gallery/)，你也可以轻松地设置一个新的虚拟机并开始使用。然而，你不会得到一个像相干模式这样的特性，但这并不是每个人都需要的。

* * *

如果这已经说服你得到 Mac Studio，你可以在下面订购。大部分配置只能直接从苹果获得，但从百思买购买可能对一些客户来说更可靠。由于高需求，发货日期似乎推迟了几周，考虑到这是你现在可以买到的[最好的 MAC 电脑](https://www.xda-developers.com/best-macs/)之一，这并不令人惊讶。如果您选择走虚拟化这条路，您也可以在下面停靠 Paralells Desktop。

 <picture>![The new Mac Studio is powered by Apple Silicon, but it can run Windows through virtualization.](img/7eb65c40aabeb44dfc3666e1e424d286.png)</picture> 

Mac Studio

##### 苹果 Mac 工作室

新的 Mac Studio 由苹果硅驱动，但它可以通过虚拟化运行 Windows。

 <picture>![Parallels Desktop virtualization software for running Windows or Linux on macOS. The latest version also supports Apple Silicon Macs and Windows on Arm.](img/860b397f9ada5cc74cb9a18adfa6dc9a.png)</picture> 

Parallels Desktop

##### Parallels 桌面

用于在 macOS 上运行 Windows 或 Linux 的 Parallels Desktop 虚拟化软件。最新版本还支持苹果 Silicon Macs 和 Arm 上的 Windows。