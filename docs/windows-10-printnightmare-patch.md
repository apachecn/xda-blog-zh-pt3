# Windows 10 获得打印噩梦漏洞的带外补丁

> 原文：<https://www.xda-developers.com/windows-10-printnightmare-patch/>

[星期二补丁](https://www.xda-developers.com/microsoft-windows-10-build-19043-1052-changelog/)要到下一个星期二*才发布，但是 Windows 已经在本周获得了累积更新。微软正在解决各种 Windows 10 版本中的一个关键漏洞，包括最新版本 21H1，但也可以追溯到最初的 Windows 10 版本。此次更新旨在解决上周披露的一个名为 PrintNightmare 的 Windows 10 漏洞。此漏洞使得攻击者能够利用 Windows 打印后台处理程序服务接管组织的域来传播恶意软件。*

漏洞[的技术细节和概念验证被意外披露](https://www.bleepingcomputer.com/news/security/public-windows-printnightmare-0-day-exploit-allows-domain-takeover/)，因为研究人员将该漏洞与上周修补的另一个问题混为一谈，该问题被标记为 CVE-2021-1675。后一个问题在 Windows 10 月的周二补丁更新中得到了解决，但 PrintNightmare 漏洞没有解决。然后，他们在漏洞被修补之前公布了利用漏洞的技术细节，使服务器容易受到攻击。这促使网络安全&基础设施安全局[鼓励](https://us-cert.cisa.gov/ncas/current-activity/2021/06/30/printnightmare-critical-windows-print-spooler-vulnerability)服务器管理员禁用 Windows 打印假脱机服务。

该漏洞的严重性和意外泄露促使微软迅速发布了一个补丁。该漏洞现已被确定为 CVE-2021-34527，并已在今天的带外更新中得到修补。如果你使用的是 Windows 10 版本 21H1、20H2 或 2004，修复该问题的更新将被标记为 [KB5004945](https://support.microsoft.com/en-us/help/55004945) ，它会为这些版本分别带来内部版本号 19043.1083、19042.1083 或 19041.83。你可以在这里[手动下载更新](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5004945)。该修复几乎是全新的，微软已经分享了该漏洞的一些细节。变更日志是这样说的:

*   解决了 Windows 打印后台处理程序服务中的远程代码执行漏洞，称为“打印噩梦”，如 [CVE-2021-34527](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-34527) 中所述。安装此更新和更高版本的 Windows 更新后，非管理员用户只能将签名的打印驱动程序安装到打印服务器。默认情况下，管理员可以将已签名和未签名的打印机驱动程序安装到打印服务器。系统的受信任根证书颁发机构中安装的根证书信任签名的驱动程序。Microsoft 建议您立即在所有支持的 Windows 客户端和服务器操作系统上安装此更新，从当前承载打印服务器角色的设备开始。您还可以选择配置**restrictdriverinstallationtoadministrator s**注册表设置，以防止非管理员在打印服务器上安装签名的打印机驱动程序。更多信息见 [KB5005010](https://support.microsoft.com/en-us/topic/kb5005010-restricting-installation-of-new-printer-drivers-after-applying-the-july-6-2021-updates-31b91c02-05bc-4ada-a7ea-183b129578a7) 。

对于其他版本，您可以在下面找到知识库文章的链接和下载链接:

此更新是强制性的，因此可以通过 Windows Update 获得，它将自动安装。不过，您可以使用下载链接更快地获得它。当然，这不会改变下周 Windows 更新的时间表。这些应该包括更多的修复，而且它们也将是强制性的。