# Linux 的 Windows 子系统现在支持 systemd

> 原文：<https://www.xda-developers.com/the-windows-subsystem-for-linux-now-supports-systemd/>

微软发布了一个新的 Linux 版 Windows 子系统的预览版，即版本 0.67.6，它带来了一些重大消息。从此版本开始，Linux 的 Windows 子系统现在支持 systemd。

对 systemd 最好的描述可能是由[官方网站](https://systemd.io)提供的，该网站将其描述为“Linux 系统的基本构建块套件”，它作为进程 ID (PID) 1 运行，这意味着它是系统启动的第一个进程，它帮助其余组件启动。默认情况下，一些 Linux 发行版，如 Ubuntu 和 Debian，会附带 systemd，这意味着有一些 Linux 应用程序依赖于它。有了这个更新，Linux 的 Windows 子系统现在也支持它们了。

依赖 systemd 支持的应用程序的一些例子包括 snap，这是一个用于在 Ubuntu 中安装和管理软件的包管理器。有了这个，你就可以使用`snap install`这样的命令轻松安装一个 app 了。还有 microk8s，可以让你在本地机器上快速运行 Kubernetes。

微软表示，它必须对 Linux 架构的 Windows 子系统进行更改，对 WSL init 进程(之前作为 PID 1 运行)进行调整，以适应这种包含。允许 Linux 系统仍然与 Windows 组件通信，以及保持与 Linux GUI 应用程序的兼容性，存在一些挑战。需要注意的一点是，systemd 不会像以前的 WSL 实现那样让您的 Linux 实例保持活动状态。除非您正在运行后台任务，否则关闭 Linux 控制台将会终止您的会话。

如果你想在 Linux 的 Windows 子系统中获得 systemd 支持，你需要从微软商店下载最新的 WSL 预览版，你可以使用下面的链接。这一更新不会直接发布到内置于 [Windows 11](https://www.xda-developers.com/windows-11/) 的 WSL 版本中，而且可能要过一段时间才会发布。

https://apps.microsoft.com/store/detail/9P9TQF7MRM4R

* * *

**来源:** [微软](https://devblogs.microsoft.com/commandline/systemd-support-is-now-available-in-wsl/)