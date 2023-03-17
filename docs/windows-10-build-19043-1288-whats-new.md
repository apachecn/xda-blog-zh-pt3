# 微软发布 Windows 10 build 19043.1288——以下是新内容

> 原文：<https://www.xda-developers.com/windows-10-build-19043-1288-whats-new/>

今天是 10 月的第二个星期二，这意味着微软是时候在一个被称为补丁星期二的场合发布它通常的累积更新了。这是自上周推出 Windows 11 以来的第一个补丁，新的操作系统 T3 有很多 T2 补丁。但 Windows 10 仍然生机勃勃，今天，所有支持的版本也在获得更新。Windows 10 build 19043.1288 正在向运行 21H1 版本操作系统的用户推出，但旧版本也在获得更新。

这实际上比以前简单得多，因为 Windows 10 版本 21H1、20H2 和 2004 都使用相同的基本版本，并且它们都获得了相同的更新。事实上，即使是部分用户可用的 Windows 10 版本 21H2 也获得了相同的更新。实际上，根据您的 Windows 10 版本，您将看到 Windows 10 内部版本号 19043.1288、19042.1288 或 19041.1288。

更新本身的标签是 [KB5006670](https://support.microsoft.com/en-us/help/5006670) ，你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5006670)手动下载。不管你现在用的是什么版本，这个更新的变更日志都是一样的，而且是一个非常通用的版本。变更日志中的一个亮点如下:

微软随后更详细地解释道:

至于已知的问题，没有太多新的东西，只有一些你在之前的更新中可能已经注意到的东西。如果您感兴趣，可以查看以下内容:

### Windows 10 内部版本 19043.1288 中的已知问题

| 

症状

 | 

工作区

 |
| --- | --- |
| 安装了从自定义离线介质或自定义 ISO 映像创建的 Windows 的设备可能会被此更新删除 [Microsoft Edge 旧版本](https://support.microsoft.com/microsoft-edge/what-is-microsoft-edge-legacy-3e779e55-4c55-08e6-ecc8-2333768c0fb0)，但不会被新的 Microsoft Edge 自动替换。只有在没有首先安装 2021 年 3 月 29 日或更高版本发布的独立服务堆栈更新(SSU)的情况下，通过将此更新组合到映像中创建自定义离线媒体或 ISO 映像时，才会遇到此问题。**注意**直接连接到 Windows Update 以接收更新的设备不受影响。这包括使用 Windows Update for Business 的设备。任何连接到 Windows Update 的设备应该总是接收最新版本的 SSU 和最新的累积更新(LCU ),而无需任何额外的步骤。 | 为了避免这个问题，请确保首先将 2021 年 3 月 29 日或之后发布的 SSU 整合到自定义离线媒体或 ISO 映像中，然后再整合 LCU。要使用现在用于 Windows 10，版本 20H2 和 Windows 10，版本 2004 的 SSU 和 LCU 组合包来完成此操作，您需要从组合包中提取 SSU。使用以下步骤提取使用 SSU:

1.  通过这个命令行从 msu 中提取 cab(以 KB5000842 的包为例):**展开 windows 10.0-kb 5000842-x64 . MSU/f:windows 10.0-kb 5000842-x64 . cab<目的路径>**
2.  通过这个命令行从之前提取的 cab 中提取 SSU:**展开窗口 10.0-KB5000842-x64.cab /f:* <目的路径>**
3.  然后您将拥有 SSU 出租车，在本例中命名为 **SSU-19041.903-x64.cab** 。首先将该文件整合到您的离线图像中，然后是 LCU。

如果您已经通过使用受影响的自定义介质安装操作系统遇到了此问题，您可以通过直接安装[新的 Microsoft Edge](https://www.microsoft.com/edge) 来缓解此问题。如果您需要广泛部署新的 Microsoft Edge for business，请参见[下载和部署 Microsoft Edge for business](https://track.flexlinkspro.com/g.ashx?foid=1.24542&trid=1198401.711&foc=17&fot=9999&fos=1&fobs=d72ea3ca-c089-4863-814a-23823fc6072e&urllink=https://www.microsoft.com/edge/business/download) 。 |
| 在安装了 2021 年 6 月 21 日( [KB5003690](https://support.microsoft.com/en-us/topic/june-21-2021-kb5003690-os-builds-19041-1081-19042-1081-and-19043-1081-preview-expired-11a7581f-2a01-47d5-ba12-431709ee2248) )更新后，一些设备无法安装新的更新，例如 2021 年 7 月 6 日( [KB5004945](https://support.microsoft.com/en-us/topic/july-6-2021-kb5004945-os-builds-19041-1083-19042-1083-and-19043-1083-out-of-band-44b34928-0a71-4473-aa22-ecf3b83eed0e) )或更高版本的更新。您将收到错误消息“PSFX_E_MATCHING_BINARY_MISSING”。 | 有关更多信息和解决方法，请参见 [KB5005322。](https://support.microsoft.com/en-us/topic/kb5005322-some-devices-cannot-install-new-updates-after-installing-kb5003214-may-25-2021-and-kb5003690-june-21-2021-66edf7cf-5d3c-401f-bd32-49865343144f) |

虽然 Windows 10 版本 21H1、20H2 和 2004 是大多数用户唯一支持的版本，但在特定情况下，Windows 10 的旧版本也仍然受支持。因此，所有这些版本今天都得到了更新。您可以查看下表，找到今天发布的每个更新的更新日志和下载链接。

像往常一样，这些更新是强制性的，它们迟早会自动安装到你的电脑上。您可能需要进行规划，以便能够更好地控制更新的时间。值得注意的是，Windows 10 version 2004 将在今年年底前结束支持，其最后一次更新计划在 12 月进行。在那之后，如果你还没有，你会想要升级到一个较新的版本或 Windows 11，以保持获得安全更新。