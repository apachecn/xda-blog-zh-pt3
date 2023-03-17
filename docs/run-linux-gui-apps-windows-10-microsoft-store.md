# 随着 WSL 在微软商店的发布，你现在可以在 Windows 10 上运行 Linux GUI 应用了

> 原文：<https://www.xda-developers.com/run-linux-gui-apps-windows-10-microsoft-store/>

微软宣布，允许用户在 Windows 设备上运行 Linux 应用程序的 Windows Linux 子系统(WSL)现已在微软商店全面上市。经过漫长的预览期后，普遍可用性意味着几件事，但最大的消息是 Windows 10 用户。

由于微软商店上列出的 Windows 子系统 for Linux 同时适用于 Windows 11 和 Windows 10，这意味着 Windows 10 用户现在可以访问 WSLg，而这在以前是 Windows 11 的专属。这是 WSL 的一个特定特性，它允许您运行基于 GUI 的 Linux 应用程序，这意味着您不局限于使用 Linux 终端来完成所有任务。如果你想要一个更友好的用户界面，GUI 应用程序大有可为，Windows 10 用户终于可以加入进来享受乐趣了。

随着 WSL 在 Microsoft Store 上的普遍可用，该版本也成为所有用户的默认版本，取代了 Windows 自带的版本。当您使用 Windows 终端安装 WSL(使用 **wsl - install** 命令)时，您现在将获得商店版本，而不是启用 Windows 附带的可选功能。也就是说，微软已经添加了新的命令，所以你可以安装你想要的特定 WSL 版本。您可以选择启用内置版本，也可以强制安装 WSL 1 而不是较新的 WSL 2 实现。还有一些命令可以禁用 Ubuntu 的安装，这通常在安装 WSL 时默认发生，并在安装完成时阻止它启动。

从微软商店安装用于 Linux 的 Windows 子系统的另一个优点是最新版本带有 systemd 支持。这是一组构建块和服务，在 Linux 系统中先于其他任何东西启动，在 Linux 发行版中很流行。一些 Linux 应用程序需要 systemd 支持，所以这可以极大地扩展 WSL 的功能。这是[微软在 9 月](https://www.xda-developers.com/the-windows-subsystem-for-linux-now-supports-systemd/)宣布的，但技术上它只在预览版中可用，因为 WSL 的商店版本并没有普遍可用——现在有了。

如果你有兴趣获得 WSL 的商店版本，你可以[在这里](https://www.microsoft.com/store/productId/9P9TQF7MRM4R)下载，或者在 Windows 终端(或者命令提示符)使用 **wsl - install** 命令安装。

* * *

**来源:** [微软](https://devblogs.microsoft.com/commandline/the-windows-subsystem-for-linux-in-the-microsoft-store-is-now-generally-available-on-windows-10-and-11/)