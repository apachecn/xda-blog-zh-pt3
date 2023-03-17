# Windows 11 Beta 版在截图工具中添加屏幕录制

> 原文：<https://www.xda-developers.com/windows-11-beta-screen-recording-snipping-tool/>

微软正在向注册了该计划测试版的 Windows 内部人员推出一些重大更新。不仅有一对新的 [Windows 11](https://www.xda-developers.com/windows-11/) 版本——22621.1245 和 22623.125——而且更大的新闻实际上是 Snipping 工具的最新更新。在这个版本中，微软在应用程序中添加了对屏幕录制的支持，使在没有第三方应用程序的情况下录制部分屏幕变得比以往任何时候都更容易。

之前，Windows 11 内置的唯一屏幕录制功能是 Xbox game bar，但那只允许录制特定的应用程序，所以你无法捕捉像桌面这样的东西。新的 Snipping 工具去年在 Dev 频道向内部人员提供，但它也在 Beta 频道中，这意味着它将在不太遥远的将来向公众开放。要获得未来的屏幕录制，您需要安装版本为 11.2212.24.0 或更高版本的截图工具。

这主要是指本周测试频道中的新内容。本周的版本主要集中在修复上，包括一些运行 Windows 11 版本 22623.1245 的任务管理器中的错误。以下是完整列表:

**【任务栏&系统托盘】**

*   修复了与快速设置交互相关的高命中率 ShellExperienceHost 崩溃。

**【任务经理】**

*   修正了一些导致任务管理器崩溃的问题。
*   现在，在导航窗格出现之前，您不必让任务管理器变得同样宽。
*   如果文本缩放已经增加，搜索框不应该再与标题栏文本重叠。
*   做了一些调整，以解决当文本缩放增加时对话框中的文本被切断的情况。
*   修正了标题栏的某些部分不能用于拖动窗口的问题。

一些修正也适用于今天发布的两个版本，如下所示:

*   **新！**本次更新改变了预览版的体验。NET 框架更新。安装此更新后，所有未来预览(可选)。NET Framework 更新将显示在**设置> Windows 更新>高级选项>可选更新**页面上，您可以控制要安装哪些可选更新。
*   我们修复了一个影响裁判的问题。该问题导致大量非分页池的使用，耗尽了系统内存。
*   我们修复了一个影响从网络复制到本地驱动器的问题。对于某些用户来说，复制速度比预期的要慢。
*   我们修复了导致 Windows Server 2022 域控制器(DC)停止响应的问题。这发生在他们处理轻型目录访问协议(LDAP)请求时。
*   我们修复了一个影响扩展祝酒的组策略的问题。
*   我们修复了输入法编辑器(IME)处于活动状态时可能发生的问题。当您同时使用鼠标和键盘时，应用程序可能已经停止响应。
*   我们修复了一个影响 conhost.exe 的问题。它停止了反应。
*   我们修复了两个或多个线程之间的资源冲突问题(称为死锁)。这个死锁影响了 COM+应用程序。
*   我们修复了一个影响受[微软漏洞保护出口地址过滤(EAF)](https://learn.microsoft.com/microsoft-365/security/defender-endpoint/exploit-protection-reference?view=o365-worldwide) 的设备的问题。一些应用程序停止响应或无法打开。其中包括微软办公软件和 Adobe Reader。
*   我们修复了阻止您根据文件内容搜索文件的问题。
*   我们修复了一个影响 searchindexer.exe 的**的问题。它随机阻止您登录或退出。**
*   我们修复了使用多字节字符集(MBCS)应用程序转换或重新转换日语汉字时可能出现的问题。当您键入时，光标可能移动到了错误的位置。
*   我们更改了您启用 Windows 诊断数据处理器配置的方式，为 [EU 数据边界](https://learn.microsoft.com/privacy/eudb/eu-data-boundary-learn#eu-data-boundary-countries-and-datacenter-locations)做准备。要了解更多信息，请参见[启用 Windows 诊断数据处理器配置](https://learn.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization#enable-windows-diagnostic-data-processor-configuration)。
*   我们修复了一个影响 mstsc.exe 的问题。它在连接到 RemoteApp 和桌面连接时停止响应。
*   我们修复了一个可能影响 **FindWindow()** 或 **FindWindowEx()** 的问题。他们可能返回了错误的窗口句柄。
*   我们修复了影响您使用任务栏上的搜索找到的图片文件的问题。此问题阻止您打开这些图片。
*   我们修复了一个可能会影响使用 Microsoft Edge [WebView2](https://developer.microsoft.com/microsoft-edge/webview2/) 显示内容的应用程序的问题。使用 WebView2 的应用包括微软 Office 和 [Widgets 应用](https://learn.microsoft.com/windows/apps/design/widgets/)。内容可能显示为空白或灰色。

有趣的是，微软没有列出这个版本的任何已知问题，这表明我们正在接近下一个“时刻”更新向普通 Windows 11 用户推出之前的最后测试阶段。这只是我们的一点猜测，但是很少看到新的内部版本没有任何已知的问题。

如果你注册了测试版频道，你可以通过在设置应用程序中检查更新来获取最新版本的 Windows 11。若要获取最新版本的 Snipping 工具，您需要在 Microsoft Store 中检查更新。如果你想了解更多关于未来 Windows 更新的信息，你也可以在预览版中查看所有可用的 [Windows 11 功能。](https://www.xda-developers.com/windows-11-features-in-preview/)

* * *

**来源:** [微软](https://blogs.windows.com/windows-insider/2023/01/26/announcing-windows-11-insider-preview-build-22621-1245-and-22623-1245/)