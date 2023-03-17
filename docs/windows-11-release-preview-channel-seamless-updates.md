# 新的 Windows 11 预览版使升级体验更加无缝

> 原文：<https://www.xda-developers.com/windows-11-release-preview-channel-seamless-updates/>

# 新的 Windows 11 预览版使升级体验更加无缝

最新的 Windows 11 Release Preview Channel build 减少了您在升级电脑时经历的重新启动次数。

微软以全新的 Windows 11 版本开始了新的一周。发布预览版 Windows 内部人士现在可以下载[Windows 11](https://www.xda-developers.com/windows-11/)build 22621.1192(kb 5022360)。这是一个相当小的版本，但它带来了一个变化，可以帮助减少您在升级 PC 时经历的重新启动次数。

更具体地说，微软已经做出了一项改变，一旦你将 Windows 11 的发布预览版升级到 22H2 版，你将获得 1 月份的可选更新和. NET 更新。这是安全修补程序。NET 更新，不需要重新启动两次。除此之外，在他的版本中还有对搜索索引、自动驾驶、组策略和游戏控制器的修复。请查看下面的更改日志。请注意，在**设置> Windows 更新>高级选项>可选更新**下还有一个新的设置页面，以查看未来。NET 预览更新。

*   我们修复了一个影响 searchindexer.exe**的问题。**它随机阻止您登录或退出。
*   我们修复了阻止您根据文件内容搜索文件的问题。
*   我们修复了两个或多个线程之间的资源冲突问题(称为死锁)。这个死锁影响了 COM+应用程序。
*   我们修复了一个影响 conhost.exe 的问题。它停止了响应。
*   我们修复了一个可能影响域名系统(DNS)后缀搜索列表的问题。当您配置它时，父域可能已经丢失。
*   我们修复了输入法编辑器(IME)处于活动状态时可能发生的问题。当您同时使用鼠标和键盘时，应用程序可能已经停止响应。
*   我们修复了一个可能影响 **FindWindow()** 或 **FindWindowEx()** 的问题。他们可能返回了错误的窗口句柄。
*   我们修复了使用多字节字符集(MBCS)应用程序转换或重新转换日语汉字时可能出现的问题。当您键入时，光标可能移动到了错误的位置。
*   我们修复了一个可能会影响使用 Microsoft Edge [WebView2](https://developer.microsoft.com/microsoft-edge/webview2/) 显示内容的应用程序的问题。使用 WebView2 的应用包括微软 Office 和 [Widgets 应用](https://learn.microsoft.com/windows/apps/design/widgets/)。内容可能显示为空白或灰色。
*   我们修复了一个问题，该问题会影响某些具有固件可信平台模块的系统。(TPM)。此问题阻止您使用 AutoPilot 来设置这些系统。
*   我们修复了影响您使用任务栏上的搜索找到的图片文件的问题。此问题阻止您打开这些图片。
*   我们修复了一个影响 mstsc.exe 的问题。它在连接到 RemoteApp 和桌面连接时停止响应。
*   我们修复了一个影响扩展祝酒的组策略的问题。
*   我们修复了导致 Windows Server 2022 域控制器(DC)停止响应的问题。这发生在他们处理轻型目录访问协议(LDAP)请求时。
*   我们修复了影响弹性文件系统(ReFS) MSba 标签的问题。该问题导致了非页面池泄漏。
*   我们修复了一个影响裁判的问题。该问题导致大量非分页池的使用，耗尽了系统内存。
*   我们修复了一个影响受[微软漏洞保护出口地址过滤(EAF)](https://learn.microsoft.com/microsoft-365/security/defender-endpoint/exploit-protection-reference?view=o365-worldwide) 的设备的问题。一些应用程序停止响应或无法打开。其中包括微软办公软件和 Adobe Reader。
*   我们修复了一个影响一些游戏控制器的问题。当游戏控制器连接到电脑时，电脑可能没有进入睡眠模式。

到目前为止，这就是微软本周的全部内容。我们还没有得到一个开发频道或测试频道建设。如果你错过了，上周的[开发者频道发布](https://www.xda-developers.com/windows-11-25276-dev-channel/)是关于设置应用的，包括更多关于云存储的信息。与往常一样，您将通过 Windows Update 自动获得新版本。

**来源:** [微软](https://blogs.windows.com/windows-insider/2023/01/17/releasing-windows-11-build-22621-1192-to-the-release-preview-channel/)