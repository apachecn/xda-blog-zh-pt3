# 微软发布 Windows 10 build 19043.1023——以下是新内容

> 原文：<https://www.xda-developers.com/microsoft-windows-10-build-19043-1013/>

又到了每月的这个时候。微软发布了新版 Windows 10 的可选累积更新。事实上，今天的更新适用于消费者支持的所有版本的操作系统，包括版本 2004、20H2 和 21H1。这也是自 [Windows 10 版本 21H1 发布](https://www.xda-developers.com/the-windows-10-may-2021-update-is-probably-coming-out-today/)以来的首次累积更新。

这是因为所有三个版本都获得了完全相同的更新。将它们彼此分开的唯一东西是一个实现包。这个包突出了一些特性，并提高了版本号。

如果你使用的是 Windows 10 版本 21H1、20H2 或 2004，你将会得到 [KB5003214](https://support.microsoft.com/en-us/topic/may-25-2021-kb5003214-os-builds-19041-1023-19042-1023-and-19043-1023-preview-8a58ac95-cf5e-4032-9272-23de9ee1d186) ，使版本号分别为 19043.1023、19042.1023 或 19041.1023。这里可以[手动下载，以下是亮点:](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5003214)

以下是修复的完整列表:

还有一些已知的问题需要注意:

| 

症状

 | 

工作区

 |
| --- | --- |
| 将设备从 Windows 10 版本 1809 或更高版本更新到更高版本的 Windows 10 时，系统和用户证书可能会丢失。如果设备已经安装了 2020 年 9 月 16 日或更晚发布的任何最新累积更新(LCU ),然后从没有集成 2020 年 10 月 13 日或更晚发布的 LCU 的媒体或安装源更新到更高版本的 Windows 10，则设备将受到影响。这主要发生在通过更新管理工具(如 Windows Server Update Services(WSUS)或 Microsoft Endpoint Configuration Manager)使用过时的捆绑包或介质更新受管设备时。当使用过时的物理介质或没有集成最新更新的 ISO 映像时，也可能发生这种情况。**注意**使用 Windows Update for Business 或直接连接到 Windows Update 的设备不受影响。任何连接到 Windows Update 的设备应该总是接收最新版本的功能更新，包括最新的 LCU，而无需任何额外的步骤。 | 如果您已经在您的设备上遇到了这个问题，您可以在卸载窗口中使用此处的说明[返回到您以前的 Windows 版本来缓解这个问题。卸载窗口可能是 10 天或 30 天，具体取决于您的环境配置和您要更新到的版本。在您的环境中解决该问题后，您需要更新到更高版本的 Windows 10。**注意**在卸载窗口中，你可以通过使用 DISM 命令/Set-OSUninstallWindow 来增加你必须回到你之前版本的 Windows 10 的天数。你必须在默认卸载窗口过期之前**做出这个改变。更多信息，请参见**](https://support.microsoft.com/windows/recovery-options-in-windows-10-31ce2444-7de3-818c-d626-e3b5a3024da5#bkmk_section6) **[DISM 操作系统卸载命令行选项](https://docs.microsoft.com/windows-hardware/manufacture/desktop/dism-uninstallos-command-line-options)。**我们正在制定解决方案，并将在未来几周内提供更新的捆绑包和更新的介质。 |
| 当使用 Microsoft 日文输入法编辑器(IME)在自动允许输入假名字符的应用程序中输入汉字字符时，您可能无法获得正确的假名字符。您可能需要手动输入汉字注音字符。**注意**受影响的应用程序正在使用**ImmGetCompositionString()**函数。 | 我们正在制定解决方案，并将在即将发布的版本中提供更新。 |
| 安装此更新后，一小部分用户报告游戏性能低于预期。受此问题影响的大多数用户都在全屏或无边框窗口模式下运行游戏，并使用两个或更多显示器。 | 使用[已知问题回滚(KIR)](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/known-issue-rollback-helping-you-keep-windows-devices-protected/ba-p/2176831) 解决此问题。请注意，解决方案可能需要 24 小时才能自动传播到消费者设备和非受管企业设备。重新启动您的设备可能有助于更快地将分辨率应用到您的设备。对于安装了受影响的更新并遇到此问题的企业管理设备，可以通过安装和配置特殊的[组策略](https://download.microsoft.com/download/e/e/e/eee62513-e95c-4d8a-99f8-2c1d62f15b0b/Windows%2010%20(2004%20&%2020H2)%20Known%20Issue%20Rollback%20042121%2001.msi)来解决。**注意**配置特殊组策略后，设备需要重启。如需帮助，请参见[如何使用组策略部署已知问题回滚](https://docs.microsoft.com/en-us/troubleshoot/windows-client/group-policy/use-group-policy-to-deploy-known-issue-rollback)。有关使用组策略的一般信息，请参见[组策略概述](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/hh831791(v=ws.11))。 |
| 安装此更新后，当使用某些音频设备和 Windows 设置时，5.1 Dolby Digital audio 可能会在某些应用程序中播放包含高音调噪音或吱吱声的声音。**注意**使用立体声时不会出现此问题。 | 要缓解此问题，您可以尝试以下一种或多种方法:

*   在网页浏览器或不同的应用程序中流式传输视频或音频，而不是受此问题影响的应用程序。
*   右击或长按**通知区**的**音量图标**，选择**空间声音(关)**，选择任意可用选项，启用**空间声音**设置。

我们正在制定解决方案，并将在即将发布的版本中提供更新。 |
| 安装了从自定义离线介质或自定义 ISO 映像创建的 Windows 的设备可能会被此更新删除 [Microsoft Edge 旧版本](https://support.microsoft.com/en-us/microsoft-edge/what-is-microsoft-edge-legacy-3e779e55-4c55-08e6-ecc8-2333768c0fb0)，但不会被新的 Microsoft Edge 自动替换。只有在没有首先安装 2021 年 3 月 29 日或更高版本发布的独立服务堆栈更新(SSU)的情况下，通过将此更新组合到映像中创建自定义离线媒体或 ISO 映像时，才会遇到此问题。**注意**直接连接到 Windows Update 以接收更新的设备不受影响。这包括使用 Windows Update for Business 的设备。任何连接到 Windows Update 的设备应该总是接收最新版本的 SSU 和最新的累积更新(LCU ),而无需任何额外的步骤。 | 为了避免这个问题，请确保首先将 2021 年 3 月 29 日或之后发布的 SSU 整合到自定义离线媒体或 ISO 映像中，然后再整合 LCU。要使用现在用于 Windows 10，版本 20H2 和 Windows 10，版本 2004 的 SSU 和 LCU 组合包来完成此操作，您需要从组合包中提取 SSU。使用以下步骤提取使用 SSU:

1.  通过这个命令行从 msu 中提取 cab(以 KB5000842 的包为例):**展开 windows 10.0-kb 5000842-x64 . MSU/f:windows 10.0-kb 5000842-x64 . cab<目的路径>**
2.  通过这个命令行从之前提取的 cab 中提取 SSU:**展开窗口 10.0-KB5000842-x64.cab /f:* <目的路径>**
3.  然后您将拥有 SSU 出租车，在本例中命名为 **SSU-19041.903-x64.cab** 。首先将该文件整合到您的离线图像中，然后是 LCU。

如果您已经通过使用受影响的自定义介质安装操作系统遇到了此问题，您可以通过直接安装[新的微软 Edge](https://www.microsoft.com/en-us/edge) 来缓解此问题。如果您需要广泛部署新的 Microsoft Edge for business，请参见[下载并部署 Microsoft Edge for business](https://www.microsoft.com/en-us/edge/business/download) |

由于这是一个 C/D 周更新，它是可选的。这意味着，如果你现在在 Windows Update 中检查更新，它将为 toy 提供选择加入的选项。如果你忽视它，你就不会得到它。相反，这些修复将被纳入下个月的补丁星期二更新，这是强制性的。