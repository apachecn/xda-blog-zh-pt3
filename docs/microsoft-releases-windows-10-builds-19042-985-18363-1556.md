# 微软发布 Windows 10 内部版本 19042.985，18363.1556

> 原文：<https://www.xda-developers.com/microsoft-releases-windows-10-builds-19042-985-18363-1556/>

今天是这个月的第二个星期二，所以是补丁星期二。今天，Windows 10 的每个受支持版本都将获得新的累积更新。这包括版本 1507、1607、1803、1809、1909、2004 和 20H2。然而，在今天之后， [Windows 10 版本 1803 和 1809 将从列表中消失](https://www.xda-developers.com/windows-10-version-1909-no-longer-supported-after-today/)。

如果你使用的是 Windows 10 版本 20H2 或 2004，你将会得到 [KB5003173](https://support.microsoft.com/en-us/help/5003173) ，使版本号分别达到 19042.985 或 19041.985。这里可以[手动下载，以下是亮点:](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5003173)

以下是修复的完整列表:

> *   Windows 应用平台和框架、Windows 内核、Windows Media、Microsoft 脚本引擎和 Windows 芯片平台的安全更新。

请注意，这些更新都是累积的，因此它们也有在本月的可选更新中找到的修复清单。

如果你还在使用 Windows 10 版本 1909，本月的补丁周二更新是 [KB5003169](https://support.microsoft.com/en-us/topic/may-11-2021-kb5003169-os-build-18363-1556-13896704-b003-4d24-bf45-b6e1ff506d64) ，使内部版本号达到 18363.1556。请注意，这是您将收到的最后一个更新，除非您使用的是 Windows 10 企业版或教育版。你可以[手动下载这里的更新](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5003169)，以下是亮点:

以下是修复的完整列表:

> *   解决了可能导致滚动条控件在屏幕上显示为空白并且不起作用的问题。此问题影响运行在 64 位 Windows 10 (WOW64)上的 32 位应用程序，这些应用程序使用**USER32.DLL 滚动条**窗口类的[超类](https://docs.microsoft.com/en-us/windows/win32/winmsg/about-window-procedures#window-procedure-superclassing)创建滚动条。这个问题也会影响 **HScrollBar** 和 **VScrollBar** 控件和从**系统派生的类。windows . forms . scroll bar**。当您创建滚动条控件时，在 64 位应用程序中可能会出现高达 4 GB 的内存使用增加。
> *   安全更新 Windows 应用平台和框架、Windows 内核、微软脚本引擎和 Windows 芯片平台。

最后，Windows 10 版本上有几个更新不支持家庭和专业 SKU。这些更新适用于企业和教育 SKU 或长期服务选项。

由于这些是周二补丁更新，它们是强制性的。如果你不选择安装它们，它们会在某个时候自动安装。

还要注意的是，由于 Windows 10 版本 1909 的消费者在今天之后不会获得更新，这意味着只有两个版本的操作系统将受到支持，2004 和 20H2。然而，本月晚些时候，Windows 10 版本 21H1 将推出，尽管所有三个支持的版本都将获得相同的累积更新。