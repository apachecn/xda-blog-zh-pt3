# Windows 10 内部版本 19044.1766 即将推出——以下是新内容

> 原文：<https://www.xda-developers.com/windows-10-build-19044-1766-rolling-out-whats-new/>

时光飞逝，一年已经过去了将近一半。6 月份已经过去了大约一半，今天是这个月的第二个星期二，这意味着是补丁星期二的时候了，届时微软将推出所有支持的 Windows 版本的更新。如果您拥有家庭版或专业版许可证，则仅包括 Windows 10 版本 21H1 和 21H2，这两个版本将分别更新为内部版本 19044.1766 和 19043.1766。

这个新版本通过一个标签为 [KB5014699](https://support.microsoft.com/en-us/help/5014699) 的更新而来，你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5014699)手动下载。按照过去几个月微软的惯例，这次更新没有太多的变更记录，但是在变更记录中有一项:

*   为[微软文件服务器卷影复制代理服务](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/jj612865(v=ws.11))解决了 [CVE-2022-30154](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2022-30154) 下的一个特权提升(EOP)漏洞。要受到保护并正常工作，您必须在应用程序服务器和文件服务器上安装 2022 年 6 月 14 日或更高版本的 Windows update。应用程序服务器运行卷影复制服务(VSS)感知应用程序，该应用程序将数据存储在文件服务器上的远程[服务器消息块](https://docs.microsoft.com/windows/win32/fileio/microsoft-smb-protocol-and-cifs-protocol-overview) 3.0(或更高版本)共享上。文件服务器托管文件共享。如果您不在两台计算机上都安装更新，以前正常工作的应用程序执行的备份操作可能会失败。对于这种故障情况，Microsoft 文件服务器卷影复制代理服务将在文件服务器上记录 FileShareShadowCopyAgent 事件 1013。更多信息见 [KB5015527](https://support.microsoft.com/help/5015527) 。

不过这次更新也包括了上个月推出的预览版更新( [KB5014023](https://support.microsoft.com/en-us/help/5014023) )的变化，确实有一个大的 changelog。其中包括大量修复，包括 Excel 或 Outlook 可能无法打开的某些情况，以及复制文件可能比预期慢的情况。

虽然 Windows 10 版本 21H2 和 21H1 是家庭版和专业版唯一支持的版本，但特定企业和教育环境中的用户仍会收到旧版本 Windows 10 的更新。这包括 Windows 10 版本 20H2，该版本于 5 月为家庭和专业用户提供了最后一次更新。不过，因为这个版本的 Windows 10 与上面的版本几乎相同，所以更新也完全相同，你可以在上面看到 changelog 和下载链接。

除此之外，一些旧版本的 Windows 10 仍然受支持，但仅限于长期服务渠道或长期服务分支。不再支持 Windows 10 版本 1909，因此本月可用的更新如下:

和往常一样，如果你不想手动下载这些更新，它们最终会自动安装。不过，手动安装它们有助于防止意外中断，因此，如果您不想在尝试工作时重启电脑，这可能是更好的选择。