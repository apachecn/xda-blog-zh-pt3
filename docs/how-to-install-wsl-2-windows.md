# 如何在 Windows 10 和 11 上设置和安装 WSL 2

> 原文：<https://www.xda-developers.com/how-to-install-wsl-2-windows/>

如果你没听说，微软喜欢 Linux。这句话引起了怀疑，但后来我们看到了 Linux 的 Windows 子系统(WSL ),并开始看到其中的真相。WSL 2 允许你在 Windows 11 或 10 中安装一个运行完整 Linux 内核的 Linux 环境，如果你还在使用的话，两者之间有相当紧密的集成。WSL 的第一个版本没有内核，性能也不尽如人意。WSL 本质上仍然是一个虚拟机，但是和它的 Windows 主机有很深的联系。

对于开发者来说，WSL 意味着无缝访问 Windows 和 Linux，而不需要使用传统的虚拟机。虽然你不必是一个开发人员，但它是一个可靠的工具，任何人都可以使用，不管他们是老手还是刚开始使用 Linux。微软在入职体验方面也做了很多工作，WSL 2 现在比以往任何时候都更容易启动和运行。下面是怎么做的。

## 在 Windows 10 和 11 上运行 WSL 2 需要什么

你不需要一台超级强大的 PC 来运行 WSL 2，也不需要传统上使用 Hyper-V VM 工具的“Pro”版本的 Windows。WSL 2 确实利用了 Hyper-V 架构，但是你不需要为此支付额外的费用。WSL 2 还支持 x64 和 ARM 处理器。然而，如果你在基于 ARM 的机器上使用它，你将需要使用一个有 ARM 版本的 Linux 版本，比如 Ubuntu。

WSL 2 也可以在虚拟机内部的 Windows 上运行，只要您使用的 VM 软件支持嵌套虚拟化，并且启用了嵌套虚拟化。

## 如何在 Windows 10 和 11 上安装 WSL 2

WSL 2 的安装过程现在非常简单，只需几分钟就可以启动并运行。唯一的先决条件是您已经安装了 KB5004296 补丁，并且已经安装了 Windows 10 版或更高版本(现在您确实应该安装了)。

有两个选项可供选择:使用微软商店或使用 PowerShell。

对于第一种方法，只需打开微软商店并下载“ [Windows 子系统 Linux 预览版](https://apps.microsoft.com/store/detail/windows-subsystem-for-linux-preview/9P9TQF7MRM4R)”应用程序。从长远来看，这有望成为获取 WSL 的地方，因为它允许团队更新它，而不需要通过 Windows Update。

或者，在 PC 上打开 PowerShell 并输入以下命令:

**wsl -安装**

坐下来，等待它做它的事情，当收到信号时重启你的电脑，瞧！WSL 2 现在已经安装在您的 PC 上了。默认的发行版是 Ubuntu，但是你可以自由地使用微软商店或者第三方资源如 Github 或者直接从发行版制造商那里获得的任何其他版本。

如果你使用的是 Windows 11，那么 Windows 终端应用将被预装，这是在你的电脑上使用 WSL 的最佳方式。您可以通过 PowerShell 使用命令" **wsl -d** "命令后跟名称来启动发行版，但是使用 Windows 终端，您可以从下拉菜单中访问您已经安装的每个发行版。

如果没有安装 Windows 终端，可以从[微软商店](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701)或者通过 [Windows 包管理器](https://winstall.app/apps/Microsoft.WindowsTerminal)抓取。