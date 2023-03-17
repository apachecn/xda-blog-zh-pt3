# 微软发布 Windows 10 补丁周二更新——以下是新内容

> 原文：<https://www.xda-developers.com/microsoft-windows-10-patch-tuesday-build-19043-1110-19042-1110/>

# 微软发布 Windows 10 build 19043.1110，19042 . 1110——以下是新内容

今天是补丁星期二，这意味着是时候对所有支持的操作系统版本进行新的 Windows 10 累积更新了。

今天是这个月的第二个星期二，是补丁星期二。这意味着今天所有受支持的 Windows 版本都将得到更新。对于消费者来说，这包括 Windows 10 版本 21H1、20H2 和 2004。为了方便起见，它们都获得相同的更新。

尽管微软使用累积更新方法进行服务，但 Windows 11 预览版没有更新。据推测，这将在本周晚些时候到达。

对于 Windows 10 版本 21H1、20H2 或 2004 的消费者，你将获得 [KB5004237](https://support.microsoft.com/en-us/help/5004237) ，使内部版本号分别达到 19043.1110、19042.1110 或 19041.1110。这里可以[手动下载，以下是亮点:](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5004237)

以下是修复的完整列表:

*   解决了可能使某些打印机难以打印的问题。此问题影响各种品牌和型号，但主要是使用 USB 端口连接的收据或标签打印机。
*   删除对 PerformTicketSignature 设置的支持，并永久启用 CVE 的强制模式-2020-17049。有关在域控制器服务器上启用完全保护的更多信息和步骤，请参见[管理 CVE Kerberos S4U 更改的部署-2020-17049](https://support.microsoft.com/en-us/topic/kb4598347-managing-deployment-of-kerberos-s4u-changes-for-cve-2020-17049-569d60b7-3267-e2b0-7d9b-e46d770332ab) 。
*   为 [CVE-2021-33757](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-33757) 增加了高级加密标准(AES)加密保护。更多信息见 [KB5004605](https://support.microsoft.com/en-us/topic/kb5004605-update-adds-aes-encryption-protections-to-the-ms-samr-protocol-for-cve-2021-33757-e4daa133-54aa-4a5d-a921-04bb50868fc2) 。
*   解决了主刷新令牌未进行高度加密的漏洞。此问题可能会允许令牌被重复使用，直到令牌过期或被续订。有关此问题的更多信息，请参见 [CVE-2021-33779](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-33779) 。
*   Windows 应用程序、Windows 管理、Windows 基础、Windows 身份验证、Windows 用户帐户控制(UAC)、操作系统安全性、Windows 虚拟化、Windows Linux、Windows 内核、Microsoft 脚本引擎、Windows HTML 平台、Windows MSHTML 平台和 Windows 图形的安全更新。

也有一些版本的 Windows 10 仍然支持商业应用。

像往常一样，在周二补丁日，这些更新是强制性的，它们会在提示你重启电脑之前的某个时候在后台安装。