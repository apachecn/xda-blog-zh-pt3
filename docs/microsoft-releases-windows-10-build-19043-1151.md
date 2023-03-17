# 微软发布 Windows 10 build 19043.1151——以下是新内容

> 原文：<https://www.xda-developers.com/microsoft-releases-windows-10-build-19043-1151/>

今天，微软发布了 Windows 10 支持版本的最新预览版更新。这些更新也称为“C”周和“D”周更新，字母代表一个月中的第一周(该月的第二周，即修补程序星期二，是“B”周更新)。由于所有受支持的 Windows 10 版本都获得了相同的位，所以它们今天都获得了相同的更新。

具体来说，此次更新针对的是 Windows 10 版本 21H1、20H2 和 2004， [KB5004296](https://support.microsoft.com/en-us/topic/july-29-2021-kb5004296-os-builds-19041-1151-19042-1151-and-19043-1151-preview-6aba536a-6ed2-41cb-bc3d-3980e8693cc4) 将使内部版本号分别达到 19043.1151、19042.1151 和 19041.1151。这里可以[手动下载，以下是亮点:](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5004296)

*   更新了阻止游戏服务为桌面用户打开某些游戏的问题。
*   更新了阻止您使用输入法编辑器(IME)输入文本的问题。例如，如果您将电源选项设置为通过合上笔记本电脑的盖子来关机，则在启动后可能会出现这种情况。

*   更新了一个问题，当你按下游戏控制器上的触发按钮时，会大声播放选择游戏中某个东西的声音。
*   更新了一个阻止电源计划和游戏模式正常运行的问题。这导致游戏时帧速率和性能降低。
*   更新了连接到虚拟专用网络(VPN)后无法检测到您已连接到互联网的问题。
*   更新导致打印停止或打印错误输出的问题。当您在更新到 Windows 10、2004 版或更高版本后使用 USB 连接进行打印时，会出现此问题。

像往常一样，也有大量的修复。以下是完整列表:

实际上还有一些已知的问题:

### KB5004296 已知问题

| 

症状

 | 

工作区

 |
| --- | --- |
| 当使用 Microsoft 日文输入法编辑器(IME)在自动允许输入假名字符的应用程序中输入汉字字符时，您可能无法获得正确的假名字符。您可能需要手动输入汉字注音字符。**注意**受影响的应用程序正在使用**ImmGetCompositionString()**函数。 | 我们正在制定解决方案，并将在即将发布的版本中提供更新。 |
| 安装了从自定义离线介质或自定义 ISO 映像创建的 Windows 的设备可能会被此更新删除 [Microsoft Edge 旧版本](https://support.microsoft.com/en-us/microsoft-edge/what-is-microsoft-edge-legacy-3e779e55-4c55-08e6-ecc8-2333768c0fb0)，但不会被新的 Microsoft Edge 自动替换。只有在没有首先安装 2021 年 3 月 29 日或更高版本发布的独立服务堆栈更新(SSU)的情况下，通过将此更新组合到映像中创建自定义离线媒体或 ISO 映像时，才会遇到此问题。**注意**直接连接到 Windows Update 接收更新的设备不受影响。这包括使用 Windows Update for Business 的设备。任何连接到 Windows Update 的设备应该总是接收最新版本的 SSU 和最新的累积更新(LCU ),而无需任何额外的步骤。 | 为了避免这个问题，请确保首先将 2021 年 3 月 29 日或之后发布的 SSU 整合到自定义离线媒体或 ISO 映像中，然后再整合 LCU。要使用现在用于 Windows 10，版本 20H2 和 Windows 10，版本 2004 的 SSU 和 LCU 组合包来完成此操作，您需要从组合包中提取 SSU。使用以下步骤提取使用 SSU:

1.  通过这个命令行从 msu 中提取 cab(以 KB5000842 的包为例):**展开 windows 10.0-kb 5000842-x64 . MSU/f:windows 10.0-kb 5000842-x64 . cab<目的路径>**
2.  从之前提取的 cab 中提取 SSU，命令行如下:**展开窗口 10.0-KB5000842-x64.cab /f:* <目的路径>**
3.  然后您将拥有 SSU 出租车，在本例中命名为 **SSU-19041.903-x64.cab** 。首先将该文件整合到您的离线图像中，然后是 LCU。

如果您已经通过使用受影响的自定义介质安装操作系统遇到了此问题，您可以通过直接安装[新的 Microsoft Edge](https://www.microsoft.com/en-us/edge) 来缓解此问题。如果您需要广泛部署新的 Microsoft Edge for business，请参见[下载和部署 Microsoft Edge for business](https://www.microsoft.com/en-us/edge/business/download) |
| 在安装了 2021 年 6 月 21 日( [KB5003690](https://support.microsoft.com/en-us/topic/june-21-2021-kb5003690-os-builds-19041-1081-19042-1081-and-19043-1081-preview-expired-11a7581f-2a01-47d5-ba12-431709ee2248) )更新后，一些设备无法安装新的更新，例如 2021 年 7 月 6 日( [KB5004945](https://support.microsoft.com/en-us/topic/july-6-2021-kb5004945-os-builds-19041-1083-19042-1083-and-19043-1083-out-of-band-44b34928-0a71-4473-aa22-ecf3b83eed0e) )或更高版本的更新。您将收到错误消息“PSFX_E_MATCHING_BINARY_MISSING”。 | 有关更多信息和解决方法，请参见 [KB5005322。](https://support.microsoft.com/en-us/topic/kb5005322-some-devices-cannot-install-new-updates-after-installing-kb5003690-june-21-2021-66edf7cf-5d3c-401f-bd32-49865343144f) |

如上所述，这是一个可选的更新。显然，您可以从更新目录中下载并手动安装它。您也可以通过 Windows Update 获取它。如果您转到“设置”->“更新与安全”->“Windows Update”并检查更新，您会看到一个下载并安装此更新的选项。如果你愿意，你可以忽略它。如果你这样做了，这些修复将被捆绑到下个月 Windows 10 的周二补丁更新中，这将是强制性的。

如果你使用的是 [Windows 11](https://www.xda-developers.com/windows-11/) ，你不会收到常规的周二补丁或可选更新。预览版本按不同的时间表更新。