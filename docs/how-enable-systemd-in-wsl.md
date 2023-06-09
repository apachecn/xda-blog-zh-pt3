# 如何在 Linux (WSL)的 Windows 子系统中启用 systemd

> 原文：<https://www.xda-developers.com/how-enable-systemd-in-wsl/>

Linux 中的 systemd 是好是坏将取决于你与谁交谈，但它非常重要，以至于一些用于 Linux 的 Windows 子系统(WSL)社区已经建立了他们自己的方法来实现它。[微软已经完成了这项工作](https://www.xda-developers.com/the-windows-subsystem-for-linux-now-supports-systemd/)，通过与 Canonical 的合作，在 WSL 中正式实现 systemd。

不过，最初，它实际上并不是每个人都可以使用的，也不是默认启用的。一旦启用，您还可以随时禁用它。以下是你需要知道的。

## 什么是 systemd？

\ r \ nht TPS://www . YouTube . com/watch？v=Ja3qikzd-as\r\n

systemd 的简短官方描述是:

> Systemd 是 Linux 系统的一套基本构建块。它提供了一个系统和服务管理器，作为 PID 1 运行，并启动系统的其余部分。

一些最流行的 Linux 发行版已经在裸机安装中默认使用 systemd。其中一些，比如 Ubuntu 和 Debian，也可以在 WSL 上获得。

WSL 中包含 systemd 使该工具更接近于本机运行 Linux 的体验。现在在 WSL 上很容易使用的一些工具也需要它，比如 snap、microk8s 和 systemctl。

## 在 WSL 中获得 systemd 需要什么

如果您使用的是 Windows 中的 WSL 版本，也就是说，您通过 PowerShell 启用的版本，而不是从商店下载的版本，那么您最初不会有 systemd。只有那些使用 Windows 11 内部版本的用户，或者那些使用从微软商店下载的 WSL 的用户才会拥有它。你需要的版本号是 0.67.6 及以上。

要检查您是否有正确的版本，只需打开 PowerShell 窗口，输入 **wsl - version** 并检查响应。如果低于 0.67.6，去微软商店[下载 WSL](https://apps.microsoft.com/store/detail/windows-subsystem-for-linux-preview/9P9TQF7MRM4R) 。或者，您可以从 [WSL GitHub repo](https://github.com/microsoft/WSL/releases) 获取最新版本。

将来，所有用户都将获得 systemd 支持，您可以通过在 PowerShell 中输入 **wsl - update** 来检查 WSL 的任何更新。

或者，如果你在 WSL 上使用 Ubuntu Preview，systemd 会被自动添加。

## 如何启用 systemd

要启用 systemd，至少现在，您必须向您的 **wsl.conf** 文件添加一条指令。这是一个可以在任何 WSL Linux 发行版中找到的配置文件，它允许您在每个发行版的基础上进行配置，而不是修改全局 WSL 设置。

这是一个简单的文本文件，所以你只需要在文本编辑器中打开它。在本例中，我们使用的是 Nano。通过输入以下命令打开您选择的 Linux 发行版中的 wsl.conf:

```
 sudo nano /etc/wsl.conf 
```

除非您之前已经构建了自己的配置文件，否则您现在很可能会看到一个空白文档。

要启用 systemd，只需在 wsl.conf 文件中输入以下内容:

```
 [boot] 
```

```
 systemd=true 
```

现在您可以简单地保存并退出文件(CTRL+O 保存，CTRL+X 退出)。从这里开始，您需要完全关闭 WSL 会话。关闭 Linux，返回 PowerShell 窗口，输入:

```
 wsl.exe --shutdown 
```

这将完全关闭您机器上的 WSL。现在只需重新打开您的 Linux 发行版。第一次启动可能需要几秒钟的时间，但是当它启动时，您将运行 systemd。您可以使用 systemctl 来检查它是否工作，system CTL 是依赖于 systemd:

```
 systemctl list-unit-files --type=service 
```

现在，您应该会看到正在运行的服务的列表。这就是启用 systemd 的全部内容。当然，通过在 wsl.conf 中更改为 false，您可以随时关闭它。

### 在 WSL 上的 Ubuntu 上使用 snap

在 WSL 上的 Ubuntu 上使用 systemd 的额外好处之一是 snap 现在可以正常工作了。不是每个人都会跑去使用它，但这是 WSL 用户可以使用的另一个特性。并且有一些有用的 snap 包你可能想试试。

例如，Nextcloud 是微软 365 和谷歌云应用和存储的开源替代产品。Nextcloud snap 是在 Linux 上安装它的最佳方式之一，现在已经在 WSL 上开放了。安装快照与使用 apt(或任何其他软件包管理器)就地替换快照是一样的:

```
 sudo snap install nextcloud 
```

您可以通过查看 [snapcraft.io](https://snapcraft.io/) 快速找到可用的快照。