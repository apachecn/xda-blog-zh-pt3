# 惠普蜻蜓 Pro 能运行 Linux 吗？

> 原文：<https://www.xda-developers.com/can-the-hp-dragonfly-pro-run-linux/>

与其他笔记本电脑系列不同，[惠普蜻蜓 Pro](https://www.xda-developers.com/hp-dragonfly-pro/) 系列同时使用 ChromeOS 和 Windows 11。有运行 ChromeOS 的[惠普蜻蜓 Pro Chromebook](https://www.xda-developers.com/hp-dragonfly-pro-chromebook/) ，还有运行 Windows 的惠普蜻蜓 Pro。但是 Linux 呢？虽然你可以在这两款[伟大的惠普笔记本电脑](https://www.xda-developers.com/best-hp-laptops/)上运行 Linux，但你需要一些变通办法。

在标准的惠普蜻蜓专业版上，您可以虚拟化 Linux，使用面向 Linux 的 Windows 子系统运行 Linux 应用，或者尝试运行它来代替 Windows，但存在驱动程序问题和设备某些部分无法正常运行的风险。然后，借助惠普蜻蜓 Pro [Chromebook](https://www.xda-developers.com/best-chromebooks/) ，你可以在 ChromeOS 应用之上运行 Linux 应用。这是你需要知道的一切。

## 惠普蜻蜓专业版上的 Linux

根据官方说法，惠普蜻蜓专业版只能运行 Windows 11。如果你想尝试 Linux 这样的替代操作系统，最好在 Windows 11 之上进行虚拟化。您可以使用 VMWare 或 Oracle Virtualbox 等应用程序来实现这一点。只需下载适合您的 Linux 风格的 ISO 文件，下载应用程序，然后按照应用程序内的说明进行操作。这是在惠普蜻蜓专业版上运行 Linux 最安全的方式。您不会影响您的主 Windows 操作系统，因为 Linux 将在虚拟化环境中运行。

或者，您也可以使用 Linux 的集成 Windows 子系统(WSL)，它可以让您在 Windows 上运行图形用户界面(GUI) Linux 应用程序。你不会得到完整的 Linux 体验。我们有一个关于[设置 WSL](https://www.xda-developers.com/how-to-install-wsl-2-windows/) 的指南。

如果你是技术型的，你有一些选择。你可以[双启动 Windows 和 Linux](https://www.xda-developers.com/dual-boot-windows-11-linux/) (更安全的选择)，或者你可以在惠普蜻蜓 Pro 上用 Linux 替换 Windows 操作系统。这样做伴随着巨大的风险，因为 Linux 上可能没有网络摄像头、触控板和键盘等设备的驱动程序，最终你可能会拥有一台无法正常工作的设备。如果您接受风险，您可以通过下载适用于您的 Linux 版本的 ISO，创建一个安装程序驱动器，然后从该驱动器启动您的 HP 蜻蜓 Pro 并格式化笔记本电脑的 SSD 以用于 Linux 来运行 Linux。除非重新安装操作系统，否则您将丢失所有数据，并且无法返回 Windows。

## 惠普蜻蜓 Pro Chromebook 上的 Linux

在惠普蜻蜓 Pro Chromebook 上，你不能用 Linux 替换 ChromeOS，因为设备上的引导加载程序默认锁定在 ChromeOS 上。不过，你能做的是在 ChromeOS 上运行 Linux GUI 应用程序。这个过程只需要 10 分钟就可以完成。我们有一个指南解释如何在 ChromeOS 上开始使用 [Linux。只需要几个简单的步骤，一旦一切都设置好了，你就可以进入企鹅终端运行命令来安装你最喜欢的 Linux 应用程序。](https://www.xda-developers.com/linux-apps-chrome-os/)

以上是关于在惠普蜻蜓专业版上运行 Linux 的所有信息。更直接的解决方案是在惠普蜻蜓专业版的 Windows 上虚拟化 Linux，或者使用 Linux 的 Windows 子系统。同时，你可以在 ChromeOS 上运行 Linux 应用程序。