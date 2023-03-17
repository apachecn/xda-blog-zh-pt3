# Windows 11 补丁周二更新修复了睡眠和任务栏搜索的问题

> 原文：<https://www.xda-developers.com/windows-11-10-patch-tuesday-february-2023/>

今天可能是情人节，但也是这个月的第二个星期二，这意味着是修补星期二的时候了。微软正在推出所有支持的 Windows 版本的更新，包括 Windows 11(原始版本和版本 22H2)以及 Windows 10。这些更新包括对整体体验的修复和改进，但它们会根据您运行的版本而有所不同。

## Windows 11 版本 22H2(内部版本号 22621.1265)

如果你运行的是最新版本的 Windows 11，今天向你推出的更新被标记为 [KB5022845](https://support.microsoft.com/en-us/topic/february-14-2023-kb5022845-os-build-22621-1265-90a807f4-d2e8-486e-8a43-d09e66319f38) ，它的内部版本号达到了 22621.1265。和往常一样，官方的变更日志没有太多的信息，但是有一些亮点。其中包括对任务栏搜索问题的修复，在任务栏中，您可能无法使用您喜欢的照片应用程序打开图像。另一个搜索问题使您无法根据文件内容搜索文件(例如，Word 文档)，此更新也解决了该问题。

此外，Windows 11 build 22621.1265 还包括一个针对带控制器的游戏玩家的修复程序，即使连接了控制器，计算机也可能会进入睡眠状态。最后，输入法编辑器的一些问题也得到了解决，性能和可靠性应该得到改善。

除了今天的更新日志中提到的内容之外，这次更新还包括了上个月可选更新( [KB5022360](https://support.microsoft.com/en-us/topic/january-26-2023-kb5022360-os-build-22621-1194-preview-f6973dbe-bcc4-402a-8b9a-0541b0959403) )的变化，同时还有许多小的修复。这些修复现在是第一次强制更新，所以如果你想知道有什么改进，你可以看看下面:

*   **新！**此次更新改变了预览体验。NET 框架更新。安装此更新后，所有未来预览(可选)。NET Framework 更新将显示在**设置> Windows 更新>高级选项>可选更新**页面上。在该页面上，您可以控制要安装哪些可选更新。
*   本次更新解决了影响**searchindexer.exe 的一个问题。它随机阻止你登录或退出。**
*   此更新解决了两个或多个线程之间的资源冲突问题(称为死锁)。这个死锁会影响 COM+应用程序。
*   本次更新解决了一个影响**conhost.exe 的问题。**停止响应。
*   此更新解决了一个可能影响域名系统(DNS)后缀搜索列表的问题。配置时，父域可能会丢失。
*   此更新解决了一个可能影响 **FindWindow()** 或 **FindWindowEx()** 的问题。他们可能会返回错误的窗口句柄。
*   此更新解决了一个影响某些具有固件可信平台模块的系统的问题。(TPM)。这个问题阻止你使用自动驾驶仪来设置这些系统。
*   这次更新解决了一个影响 mstsc.exe 的**的问题。它在连接到 RemoteApp 和桌面连接时停止响应。**
*   此更新解决了导致 Windows Server 2022 域控制器(DC)停止响应的问题。当它们处理轻量级目录访问协议(LDAP)请求时，会出现这种情况。
*   此更新解决了影响弹性文件系统(ReFS) MSba 标记的问题。该问题导致非分页池泄漏。
*   此更新解决了一个影响参考的问题。该问题会导致大量非分页池的使用，从而耗尽系统内存。
*   此更新解决了一个影响受[微软漏洞保护导出地址过滤(EAF)](https://learn.microsoft.com/microsoft-365/security/defender-endpoint/exploit-protection-reference?view=o365-worldwide) 约束的设备的问题。一些应用程序停止响应或无法打开。其中包括微软 Office 和 Adobe Reader。
*   此更新解决了一个可能会影响使用 Microsoft Edge [WebView2](https://developer.microsoft.com/microsoft-edge/webview2/) 显示内容的应用程序的问题。使用 WebView2 的应用包括微软 Office 和 [Widgets 应用](https://learn.microsoft.com/windows/apps/design/widgets/)。内容可能会显示为空白或灰色。
*   此更新解决了一个影响扩展祝酒词组策略的问题。
*   此更新更改了您启用 Windows 诊断数据处理器配置的方式，为 [EU 数据边界](https://learn.microsoft.com/privacy/eudb/eu-data-boundary-learn#eu-data-boundary-countries-and-datacenter-locations)支持做准备。要了解更多信息，请参见[启用 Windows 诊断数据处理器配置](https://learn.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization#enable-windows-diagnostic-data-processor-configuration)。

虽然更新会很快自动下载，但您也可以在这里手动下载。

## Windows 11 版本 21H2(内部版本号 22000.1574)

对于那些仍然运行 Windows 11 原始版本的人来说，更新有点不同。您将获得一个标签为 [KB5022836](https://support.microsoft.com/en-us/topic/february-14-2023-kb5022836-os-build-22000-1574-dfe0c801-e2e0-45dd-bb47-2c2cbea505ed) 的更新，并且构建号将被更新为 22000.1574。这个版本的变更日志中没有任何内容，但你必须再次查看一月份的可选更新— [KB5019274](https://support.microsoft.com/en-us/topic/january-19-2023-kb5019274-os-build-22000-1516-preview-ace2511d-586e-41b0-b213-3a89d97565a4) —看看有什么新内容。

这个版本中有几个亮点。首先，现在在设置应用的个性化页面中有一个 Windows Spotlight 主题选项，这意味着你不再需要进入背景图像设置来启用 Windows Spotlight。

帐户部分也有更新，包括一个新的 OneDrive 存储使用指示器，显示您的 OneDrive 订阅的可用总存储，以及新的警报和管理 OneDrive 订阅设置的功能。Xbox 订阅的详细信息现在也可以在这个页面上看到。

除了这些更改之外，此版本中还修复了大量问题，包括修复了使用 IME 时的某些性能问题(与上面提到的问题相同)，等等。以下是完整列表:

*   此更新解决了影响一些现代应用程序的问题。这个问题阻止他们打开。
*   此更新解决了输入法编辑器(IME)处于活动状态时可能出现的问题。当您同时使用鼠标和键盘时，应用程序可能会停止响应。
*   此更新解决了触摸键盘无法打开的问题。
*   此更新解决了阻止您根据文件内容搜索文件的问题。
*   这次更新解决了一个影响 searchindexer.exe**的问题。**它随机阻止您登录或退出。
*   此更新解决了两个或多个线程之间的资源冲突问题(称为死锁)。这个死锁会影响 COM+应用程序。
*   本次更新解决了一个影响**conhost.exe 的问题。**停止响应。
*   此更新解决了影响域名系统(DNS)后缀搜索列表的问题。配置时，父域可能会丢失。
*   此更新增加了对长达 8196 个字符的长 URL 的支持。
*   此更新解决了一个可能影响 **FindWindow()** 或 **FindWindowEx()** 的问题。他们可能会返回错误的窗口句柄。
*   此更新解决了降低内存位置的问题。使用某些高清音频控制器硬件时出现问题。
*   此更新解决了一个影响某些具有固件可信平台模块的系统的问题。(TPM)。这个问题阻止你使用自动驾驶仪来设置这些系统。
*   此更新解决了影响 Microsoft Edge 中横向模式打印的问题。打印输出不正确。使用 Microsoft Defender Application Guard 时会出现此问题。
*   本次更新解决了一个使**explorer.exe**停止响应的问题。当您在某些设备上使用键盘上的播放和暂停按钮时，会出现此问题。
*   此更新解决了一个影响 Windows Server 2022 域控制器的问题。它们在管理轻量级目录访问协议(LDAP)请求时停止响应。
*   此更新解决了影响弹性文件系统(ReFS) MSba 标记的问题。该问题导致非页面池泄漏。
*   此更新解决了一个影响引用的问题。该问题会导致大量非分页池的使用，从而耗尽系统内存。
*   此更新更改了您启用 Windows 诊断数据处理器配置的方式，为[欧盟数据边界](https://learn.microsoft.com/privacy/eudb/eu-data-boundary-learn#eu-data-boundary-countries-and-datacenter-locations)支持做准备。要了解更多信息，请参见[启用 Windows 诊断数据处理器配置](https://learn.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization#enable-windows-diagnostic-data-processor-configuration)。

如果你不想等它自动安装，你可以在这里手动下载这个更新。

## Windows 10

仍然持有受支持版本的 Windows 10 的用户也在获得更新，他们将在更长时间内继续获得更新。对于大多数用户来说，唯一支持的版本是 Windows 10 版本 22H2、21H2 和 20H2，它们都获得了相同的更新。该更新被标记为 [KB5022834](https://support.microsoft.com/en-us/topic/february-14-2023-kb5022834-os-builds-19042-2604-19044-2604-and-19045-2604-ffb56254-3fee-44f1-9574-b8a0c19bde77) ，并且根据您拥有的版本，它将内部版本号变为 19045.2604、19044.2604 或 19042.2604。

这个版本有一个亮点，它修复了一些物联网设备可能停止播放音频的问题。然而，查看 1 月份的可选更新(KB5019275)，我们可以发现，当您接近存储限制时，此更新还为 OneDrive 添加了存储警报。否则，此更新包括以下修复程序:

*   ***新增！*** 此更新解决了影响缓存的 Fast Identity Online 2.0 (FIDO2)身份验证数据的问题。第一次登录尝试失败。第二次登录尝试成功。
*   本次更新解决了影响**searchindexer.exe 的一个问题。**它随机阻止你登录或退出。
*   本次更新解决了一个影响**conhost.exe 的问题。**停止响应。
*   此更新解决了影响域名系统(DNS)后缀搜索列表的问题。配置时，父域可能会丢失。
*   此更新增加了对长达 8196 个字符的长 URL 的支持。
*   此更新解决了输入法编辑器(IME)处于活动状态时可能出现的问题。当您同时使用鼠标和键盘时，应用程序可能会停止响应。
*   此更新解决了打开任务视图时出现的问题。它会导致桌面停止响应。
*   此更新解决了降低内存位置的问题。使用某些高清音频控制器硬件时出现问题。
*   本次更新解决了一个影响**MSInfo.exe**的问题。它报告了 Windows Defender 应用程序控制(WDAC)用户模式策略的错误实施状态。
*   此更新解决了一个影响某些具有固件可信平台模块的系统的问题。(TPM)。这个问题阻止你使用自动驾驶仪来设置这些系统。
*   此更新解决了影响 Microsoft Edge 中横向模式打印的问题。打印输出不正确。使用 Microsoft Defender Application Guard 时会出现此问题。
*   此更新解决了影响弹性文件系统(ReFS) MSba 标记的问题。该问题导致非分页池泄漏。
*   此更新解决了一个影响弹性文件系统(ReFS)的问题。该问题会导致大量非分页池的使用，从而耗尽系统内存。
*   此更新更改了您启用 Windows 诊断数据处理器配置的方式，为[欧盟数据边界](https://learn.microsoft.com/privacy/eudb/eu-data-boundary-learn#eu-data-boundary-countries-and-datacenter-locations)支持做准备。要了解更多信息，请参见[启用 Windows 诊断数据处理器配置](https://learn.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization#enable-windows-diagnostic-data-processor-configuration)。

你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5019275)手动下载这个更新。

对于运行旧版本的企业用户，如 LTSB 和 LTSC 版本，现在还有一些更新推出。您可以了解有关这些更新的更多信息，并使用下面的链接下载它们。

只要你的操作系统支持，这些更新应该都是自动下载的，不用你自己动手。但是，您可以通过尽快下载它们来防止意外。