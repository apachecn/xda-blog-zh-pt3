# 微软发布 Windows 10 build 19043.1081——以下是新内容

> 原文：<https://www.xda-developers.com/microsoft-releases-windows-10-build-19043-1081-heres-whats-new/>

# 微软发布 Windows 10 build 19043.1081——以下是新内容

微软发布了另一个可选的 Windows 10 累积更新。它修复了模糊的新闻和兴趣图标和许多其他问题。

继本月的[补丁周二](https://www.xda-developers.com/microsoft-windows-10-build-19043-1052-changelog/)和上周的[Windows 10 版本 1909 和 1809 的可选更新](https://www.xda-developers.com/microsoft-releases-windows-10-build-18363-1645-heres-whats-new/)之后，微软今天发布了另一个可选的 Windows 10 累积更新。这一次，更新是针对较新版本的 Windows 10 - 2004、20H2 和 21H1。对于测试版和发布预览版渠道中的 Windows 内部人员来说，这个更新是上周发布的[。](https://www.xda-developers.com/microsoft-windows-10-cumulative-update-19043-1081-insiders/)

今天的更新将内部版本号提高到 19041.1081、19042.1081 和 19043.1081，这取决于您运行的版本。所有这些版本的 Windows 10 都获得了相同的更新，因为它们都有相同的文件。较新的版本只有启用特定功能的切换。更新本身是 [KB5003690](https://support.microsoft.com/en-us/topic/june-21-2021-kb5003690-os-builds-19041-1081-19042-1081-and-19043-1081-preview-11a7581f-2a01-47d5-ba12-431709ee2248) ，你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5003690)手动下载。它修复了许多主要问题，包括微软[已经承认的](https://www.xda-developers.com/microsoft-acknowledges-blurry-text-in-news-and-interests-in-windows-10/)模糊的新闻和兴趣图标。这个问题在上周 Windows 10 版本 1909 的累积更新中也得到了修复。以下是此次发布的亮点:

*   更新了一小部分用户在安装 [KB5000842](https://support.microsoft.com/en-us/topic/march-29-2021-kb5000842-os-builds-19041-906-and-19042-906-preview-1a58a276-6a0a-47a5-aa7d-97af2d10b16d) 或更高版本后游戏性能低于预期的问题。
*   更新了导致日语输入法编辑器(IME)在您键入时突然停止工作的问题。
*   更新了使用 PIN 登录失败的问题。错误消息是“发生了一些事情，您的 PIN 不可用。单击以再次设置您的 PIN。
*   更新了在某些情况下，当您按下控制器上的 Windows 按钮时，会将您带出独占虚拟现实(VR)应用程序并返回到 Windows 混合现实主页的问题。
*   更新了导致某些屏幕分辨率下 Windows 任务栏上的新闻和兴趣按钮上的文本模糊的问题。
*   更新当您右键单击任务栏并关闭“新闻和兴趣”时，Windows 任务栏上搜索框图形出现的问题。使用黑暗模式时，这个图形问题尤其明显。
*   更新了一个问题，该问题可能会阻止您在启动或唤醒设备后使用指纹登录。
*   更新了当您使用某些音频设备和 Windows 设置播放 5.1 杜比数字音频时，在某些应用程序中可能会导致高音调噪音或吱吱声的问题。

修复的完整列表很长，因为它往往在这些可选更新中。以下是此版本中已修复或更新的所有内容:

*   解决了在启用“AppMgmt_COM_SearchForCLSID”策略后导致应用程序之间的通信停止的问题。
*   解决了在非英语语言环境中使用 **MultiByteToWideChar()** 函数时出现的性能问题。
*   解决了在使用多种版本的国家语言支持(NLS)排序时，排序无法正常工作的问题。
*   解决了一小部分用户在安装 [KB5000842](https://support.microsoft.com/en-us/topic/march-29-2021-kb5000842-os-builds-19041-906-and-19042-906-preview-1a58a276-6a0a-47a5-aa7d-97af2d10b16d) 或更高版本后游戏性能低于预期的问题。
*   解决了在您键入时导致日语输入法编辑器(IME)突然停止工作的问题。
*   解决了当您尝试在离线模式下迁移时导致 WMIMigrationPlugin.dll**返回错误的问题。**
*   解决了**Set-rule option**PowerShell 命令无法为 Windows Defender 应用程序控制(WDAC)策略提供选项来将使用过期证书签名的文件视为未签名的问题。
*   解决了导致 Windows 在使用 AppLocker 验证具有多个签名的文件时停止工作的问题。错误是 0x3B。
*   解决了可能导致 BitLocker 在更新受信任的平台模块(TPM)固件后进入恢复模式的问题。当设置了“交互式登录:计算机帐户锁定阈值”策略并且有不正确的密码尝试时，会出现这种情况。
*   解决了导致 Windows 生成许多 AppLocker 或 SmartLocker 成功事件的问题。
*   解决了启用凭据保护和远程凭据保护时对域控制器进行身份验证的问题。
*   解决了在启用受虚拟机管理程序保护的代码完整性(HVCI)时，某些屏幕阅读器应用程序无法运行的问题。
*   解决了使用 PIN 登录失败的问题。错误消息是“发生了一些事情，您的 PIN 不可用。单击以再次设置您的 PIN。
*   为某些支持安全启动的处理器添加了对系统管理模式保护(固件保护 2.0 版)的 Windows 支持。
*   解决了在某些情况下，当您按下控制器上的 Windows 按钮时，会将您带出独占的虚拟现实(VR)应用程序并返回到 Windows 混合现实主页的问题。在此更新中，当您按下 Windows 按钮时，会出现 Windows 开始菜单。当你关闭开始菜单时，你会回到专属的 VR 应用程序。
*   提高 Microsoft 365 端点数据丢失防护(DLP)分类引擎中敏感数据分析的准确性和效率。
*   解决远程访问服务器(RAS)服务器上的 Internet 密钥交换(IKE) VPN 服务的问题。用户无法定期通过 IKE 协议将 VPN 连接到服务器。此问题可能在重新启动服务器或重新启动 IKEEXT 服务几个小时或几天后出现。一些用户可以连接，而许多其他用户无法连接，因为服务处于 DoS 保护模式，这限制了传入的连接尝试。
*   解决了在启用管理帧保护(MFP)的情况下，由于四向握手中的无效消息完整性检查(MIC)而导致 Wi-Fi 连接失败的问题。
*   解决了续订用户自动注册证书后可能导致 VPN 失败的问题。错误消息是“没有更多的文件”。
*   解决了隧道可扩展身份验证协议(TEAP)的一个问题，即使未选择或禁用身份隐私，该协议也会用“匿名”替换外部身份。
*   解决了在启用用户数据报协议(UDP)时导致远程桌面会话停止响应的问题。
*   增加了对 **USB 测试和测量类**的支持。
*   解决了 Adamsync.exe**的一个影响大型活动目录子树同步的问题。**
*   解决当轻型目录访问协议(LDAP)绑定缓存已满且 LDAP 客户端库收到引用时发生的错误。
*   解决当连接关闭时系统删除绑定对象时发生的争用情况所导致的重定向器停止错误。
*   解决了阻止用户在 C 驱动器上设置或查询磁盘配额的问题。
*   解决了在 NT 虚拟 DOS 机器(NTVDM)上运行的 16 位应用程序在打开时停止工作的问题。
*   解决了安装压缩字体格式版本 2 (CFF2)字体时导致 fontdrvhost.exe**停止工作的问题。**
*   解决了由于字体回退设置而可能导致最终用户定义的字符(EUDC)无法正确打印的问题。
*   解决了在某些显示配置下导致 Windows 任务栏上的新闻和兴趣按钮文本模糊的问题。
*   解决当您使用任务栏的上下文菜单关闭新闻和兴趣时，Windows 任务栏上搜索框图形出现的问题。使用黑暗模式时，这个图形问题尤其明显。
*   解决了系统启动或从睡眠状态恢复后可能导致指纹登录失败的问题。
*   解决了当您使用某些音频设备和 Windows 设置播放 5.1 杜比数字音频时，在某些应用程序中可能会导致高音调噪音或吱吱声的问题。

和往常一样，这个版本也有一些已知的问题。在安装此更新之前，您需要了解以下内容:

| 

**症状**

 | 

**解决方法**

 |
| --- | --- |
| 当使用 Microsoft 日文输入法编辑器(IME)在自动允许输入假名字符的应用程序中输入汉字字符时，您可能无法获得正确的假名字符。您可能需要手动输入汉字注音字符。**注意**受影响的应用程序正在使用**ImmGetCompositionString()**函数。 | 我们正在制定解决方案，并将在即将发布的版本中提供更新。 |
| 安装了从自定义离线介质或自定义 ISO 映像创建的 Windows 的设备可能会被此更新删除 [Microsoft Edge 旧版本](https://support.microsoft.com/en-us/microsoft-edge/what-is-microsoft-edge-legacy-3e779e55-4c55-08e6-ecc8-2333768c0fb0)，但不会被新的 Microsoft Edge 自动替换。只有在没有首先安装 2021 年 3 月 29 日或更高版本发布的独立服务堆栈更新(SSU)的情况下，通过将此更新组合到映像中创建自定义离线媒体或 ISO 映像时，才会遇到此问题。**注意**直接连接到 Windows Update 以接收更新的设备不受影响。这包括使用 Windows Update for Business 的设备。任何连接到 Windows Update 的设备应该总是接收最新版本的 SSU 和最新的累积更新(LCU ),而无需任何额外的步骤。 | 为了避免这个问题，请确保首先将 2021 年 3 月 29 日或之后发布的 SSU 整合到自定义离线媒体或 ISO 映像中，然后再整合 LCU。要使用现在用于 Windows 10，版本 20H2 和 Windows 10，版本 2004 的 SSU 和 LCU 组合包来完成此操作，您需要从组合包中提取 SSU。使用以下步骤提取使用 SSU:通过该命令行从 msu 提取 cab(以 KB5000842 的包为例):**展开 windows 10.0-kb 5000842-x64 . MSU/f:windows 10.0-kb 5000842-x64 . cab<目的路径>** 通过该命令行从之前提取的 cab 中提取 SSU:**展开 Windows10.0-KB5000842-x6 首先将该文件整合到您的离线图像中，然后是 LCU。如果您已经通过使用受影响的自定义介质安装操作系统遇到了此问题，您可以通过直接安装[新的 Microsoft Edge](https://www.microsoft.com/en-us/edge) 来缓解此问题。如果您需要广泛部署新的 Microsoft Edge for business，请参见[下载和部署 Microsoft Edge for business](https://www.microsoft.com/en-us/edge/business/download) 。** |

除了顶部链接的手动下载之外，您还可以通过 Windows Update 的可选更新下获得此更新。你可以一直等待这些变化被包含在下个月的补丁星期二，这将是强制性的。Windows 10 累积更新包括所有以前的修复程序，因此如果您还没有它们，您将获得它们。