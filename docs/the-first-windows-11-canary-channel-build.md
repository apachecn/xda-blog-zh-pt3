# 第一个 Windows 11 金丝雀频道版本为操作系统带来了轻微的调整和变化

> 原文：<https://www.xda-developers.com/the-first-windows-11-canary-channel-build/>

对于运行 Windows 11 的 Windows 内部人员来说，这将是忙碌的一天。除了重新启动的开发频道 T1 的新版本，微软还向金丝雀频道发布了第一个 T2 Windows 11 T3 版本。它的内部版本号是 25314。

这一次，该公司已经选择发布一个版本的变更日志，但这里没有太多的新内容。在今天的 Dev Channel 版本中，对文件资源管理器做了一些调整。这是此版本独有的与 LSA 保护启用相关的变更的补充。

同样，Canary Channel 构建通常不会为每个版本获取文档。但是今天，微软选择突出一些东西，我们在这里为你做了浓缩。现在，您应该可以在文件浏览器的 XAML 上下文菜单中看到访问键快捷方式。这是一个快捷方式，可以让您在上下文菜单中执行命令，并使菜单更易于访问。

至于文件资源管理器中的文件建议，这是为那些使用 Azure Active Directory 帐户的人准备的。你会在新的**推荐**栏目下看到你拥有或分享的文件。然而，这些功能还不能为所有人所用，将会慢慢推出。下面是两者的预览。

此版本的另一项变化是升级时启用 LSA 保护。这是一项安全功能，通过防止未经授权的代码在 LSA 进程中运行，有助于防止用于登录的机密和凭据被盗。它还可以防止进程内存的转储。微软在另一篇博客文章中深入探讨了这一变化[。这个版本中的其他一些变化如下。](https://learn.microsoft.com/en-us/windows-server/security/credentials-protection-and-management/configuring-additional-lsa-protection#after-opting-in-how-to-identify-plug-ins-and-drivers-loaded-by-the-lsassexe)

**-** “讲述人”现在将在“讲述人”启动时检索对其 [Outlook 支持](https://support.microsoft.com/en-us/windows/chapter-5-navigation-68941680-3245-6ef5-5012-0674b8b6fc59#WindowsVersion=Windows_11)的更新。您可以在讲述人用户指南的第 5 章[中了解我们为 Outlook 所做工作的更多信息。我们没有向 Outlook 支持添加任何额外的功能。](https://support.microsoft.com/en-us/windows/chapter-5-navigation-68941680-3245-6ef5-5012-0674b8b6fc59#WindowsVersion=Windows_11)

**-** 为了提高 Windows 11 的安全性，从这个版本开始，我们默认禁用[远程邮件槽协议](https://learn.microsoft.com/openspecs/windows_protocols/ms-mail/47ac910f-1dec-4791-8486-9b3e8fd542da)。传统的远程邮件槽协议是客户端和服务器之间的一种简单、不可靠、不安全的单向进程间通信协议，它是在 Windows NT 3.1 中引入的，在未来的 Windows 版本中将被弃用。

这就是本周金丝雀频道的全部内容，但仅仅因为微软选择突出这些功能，并不意味着就是这样。金丝雀频道带来了比任何其他 Windows Insider 版本更多的新功能。您可能会注意到也可能不会注意到这些特性，因为所有 Canary Channel 版本都是在微软构建完成后立即发布的，几乎没有任何文档。

**来源:** [微软](https://blogs.windows.com/windows-insider/2023/03/08/announcing-windows-11-insider-preview-build-25314/)