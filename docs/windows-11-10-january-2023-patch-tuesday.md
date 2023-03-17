# 最新的 Windows 11 更新修复了一些设备启动时的蓝屏问题

> 原文：<https://www.xda-developers.com/windows-11-10-january-2023-patch-tuesday/>

以防你不知道，今天是星期二，事实上，这是今年的第一天。在每个月的第二个星期二，微软发布其所有支持的操作系统的新更新。今天，这包括 [Windows 11](https://www.xda-developers.com/windows-11/) ，Windows 10 和——有史以来最后一次——[Windows 7 和 Windows 8.1](https://www.xda-developers.com/windows-7-and-8-1-dead/) ，从今天起不再支持。

Windows 11 的原始版本和[版本 22H2](https://www.xda-developers.com/windows-11-22h2/) 都在更新，虽然它们有相似的变化，但它们并不完全相同。最初 Windows 版本的用户将获得 build 22000.1455，而运行 Windows 11 版本 22H2 的用户将获得 build 22621.1105。

我们先从后者说起。Windows 11 build 22621.1105 来自一个标记为 [KB5022303](https://support.microsoft.com/en-us/topic/january-10-2023-kb5022303-os-build-22621-1105-c45956c6-4ccb-4216-832c-2ec6309c7629) 的更新，你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5022303)手动下载。发行说明没有提到大量的变化，这可能是假期的结果。但是，它确实解决了几个问题:

> *   此更新解决了影响本地会话管理器(LSM)的问题。这些问题可能允许没有管理员权限的用户执行只有管理员才能执行的操作。
> *   此更新解决了一个已知问题，该问题会影响使用 Microsoft 开放式数据库连接(ODBC) SQL Server 驱动程序(**sqlsrv32.dll**)连接到数据库的应用程序。连接可能会失败。您也可能在应用程序中收到错误，或者从 SQL Server 收到错误。

如果你还在运行最初的 Windows 11 版本，build 22000.1455 将通过一个标签为 [KB5022287](https://support.microsoft.com/en-us/topic/january-10-2023-kb5022287-os-build-22000-1455-951898ec-2628-4d25-850e-9a44207bc139) 的更新发布，你可以[在这里手动下载](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5022287)。本次更新的变更日志包括了上面的两个项目，但是有一个额外的修复，用于一些设备在启动时可能会出现蓝屏。

这些更新中的已知问题也没有什么新的。最初的版本没有微软所知的问题，而 Windows 11 版本 22H2 在文件传输速度和供应方面存在一些问题，这些问题已经存在了几个月。微软表示，它仍在努力解决这些问题，尽管这两个问题都有解决办法。

如果你还在运行 Windows 10，本月发布的更新也和上面的一样。所有支持的 Windows 10 版本都获得了相同的更新， [KB5022282](https://support.microsoft.com/en-us/topic/january-10-2023-kb5022282-os-builds-19042-2486-19044-2486-and-19045-2486-9587e4e3-c2d7-48a6-86e2-8cd9146b47fd) ，与 Windows 11 初始版本的更新有相同的变化。你可以[在这里手动下载 Windows 10 更新](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5022282)。

按照周二补丁更新的惯例，这些是强制性的，它们迟早会自动安装。您可以使用上面的链接手动安装它们，或者如果您想在特定时间获取更新，请在 Windows Update 中检查更新。