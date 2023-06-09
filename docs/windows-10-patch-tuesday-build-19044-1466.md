# 微软推出 Windows 10 build 19044.1466——以下是新内容

> 原文：<https://www.xda-developers.com/windows-10-patch-tuesday-build-19044-1466/>

我们正式在 2022 年的第二个星期二，这意味着它也是微软 2022 年的第一个补丁星期二。该公司正在为所有受支持的 Windows 版本推出安全更新，包括 Windows 10 版本 20H2、21H1 和 21H2。此次更新使 Windows 10 的内部版本号分别达到 19044.1466、19043.1466 和 19042.1466。

如果你错过了，版本 2004 [在上个月](https://www.xda-developers.com/windows-10-version-2004-no-longer-supported/)结束了支持，尽管与后续版本几乎相同，但它不会再有任何更新。你必须更新到较新版本的 Windows 10 才能继续接收安全更新，考虑到更新非常简单，我们强烈建议你这样做，这样你就可以保持安全。

Windows 10 build 19044.1466 及其相关版本通过一个标记为 [KB5009543](https://support.microsoft.com/en-us/help/5009543) 的更新而来，你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5009543)手动下载。至于这些更新的新内容，微软只提到了一些改进。具体来说，针对 Active Directory 的一个问题和日语 IME 可能无法正常工作的一个问题，有一些修复程序。以下是修复的完整描述:

*   解决了当您进行多个属性更改时，在轻型目录访问协议(LDAP)修改操作期间无法正确写入 Active Directory (AD)属性的问题。
*   解决了影响日语输入法编辑器(IME)的已知问题。当您使用日文 IME 输入文本时，在使用[多字节字符集(MBCS)](https://docs.microsoft.com/cpp/text/support-for-multibyte-character-sets-mbcss) 的应用程序中，文本可能会出现乱序或者文本光标可能会意外移动。此问题影响 Microsoft 日语 IME 和第三方日语 ime。

在过去的几个月里，微软的变更日志有些缺乏，特别是自从 Windows 11 发布以来。通常，更大的变更日志可以在内部人员的预览更新或可选更新中找到，但这次不是这样。这是我们所有的。

除了每个人都支持的 Windows 10 版本之外，还有少数版本只在特定 SKU 中受支持。今天这些也在更新，尽管目标受众要小得多。如果您仍然在运行这些版本中的一个，您可以在下面找到更新:

按照周二补丁更新的惯例，这些更新会随着时间的推移自动推出和安装，所以你不必急着自己去获取。手动安装可以帮助您做好准备，这样您就不会在意外的时候被提示重新启动。