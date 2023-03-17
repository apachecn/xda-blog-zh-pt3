# 微软推出 Windows 10 build 19044.1586——以下是新内容

> 原文：<https://www.xda-developers.com/windows-10-build-19044-1586/>

我们又一次来到了新的一个月的第二个星期二，这意味着今天是补丁星期二。微软正在为所有受支持的 Windows 版本推出累积更新，包括 Windows 11 和 Windows 10。虽然 Windows 10 不再有任何大的新功能，但这些更新应该会提高整体的稳定性和可靠性。提醒一下，只有 Windows 10 版本 21H2、21H1 和 20H2 受到官方支持，它们将分别更新到内部版本号 19044.1586、19043.1586 和 19042.1586。

不过，这些都是相同的更新，这是因为这三个版本的 Windows 10 本质上是相同的，只是新版本启用了一些额外的功能。更新的标签是 [KB5011487](https://support.microsoft.com/en-us/help/5011487) ，你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5011487)手动下载，如果你喜欢走那条路的话。至于新功能，微软已经解决了 [OneDrive 数据在重置后可能会保留在你的 PC 上的问题](https://www.xda-developers.com/windows-11-reset-bug-onedrive-files/)。以下是该修复的完整描述:

*   *   解决当您尝试重置 Windows 设备及其应用程序包含包含[重解析数据](https://docs.microsoft.com/windows/win32/fileio/reparse-points)的文件夹时发生的已知问题，例如 Microsoft OneDrive 或 Microsoft OneDrive for Business。当您选择**删除所有内容**时，从 Microsoft OneDrive 本地下载或同步的文件可能不会被删除。某些设备在安装此更新后可能需要七(7)天才能完全解决问题，并防止文件在重置后持续存在。为了立即生效，您可以使用 [Windows Update 故障诊断程序](https://support.microsoft.com/windows/windows-update-troubleshooter-19bc41ca-ad72-ae67-af3c-89ce169755dd)中的说明手动触发 Windows Update 故障诊断程序。

这就是此次更新的全部内容，这是因为微软喜欢在前一个月将大部分重大变化放在可选更新中——在本例中是 [KB5010415](https://support.microsoft.com/en-us/topic/february-15-2022-kb5010415-os-builds-19042-1566-19043-1566-and-19044-1566-preview-5a644b82-83f4-4cc2-a0e7-85f643252386) 。所有这些变化都已纳入 Windows 10 内部版本 19044.1586，现在它们是强制性的。以下是从可选更新中继承下来的所有内容:

### Windows 10 版本 21H2、21H1 和 20H2 的修复程序

*   ***新增！*** 提供在 Microsoft Edge Internet Explorer 模式和 Microsoft Edge 之间共享 cookies 的能力。
*   ***新增！*** 增加了对热添加和移除非易失性内存(NVMe)命名空间的支持。
*   解决了当 Windows Server 2016 作为使用特定云计算虚拟桌面基础架构(VDI)的终端服务器运行时出现的问题。因此，服务器在运行一段时间后会随机停止响应。这也解决了一个回归问题，该回归主动检查以确保**rpcss.exe**中的 CSharedLock 被正确设置以避免死锁。
*   解决影响 Windows search 服务并在使用近似运算符进行查询时出现的问题。
*   解决 wmipicmp.dll 模块**中的内存泄漏问题，该问题导致系统中心运营管理器(SCOM)数据中心监控系统出现大量错误警报。**
*   解决了当登录用户数超过 100 时导致远程桌面服务(RDS)服务器变得不稳定的问题。这将阻止您在 Windows Server 2019 上使用 RDS 访问已发布的应用程序。
*   解决了当您浏览域或组织单位(ou)时返回错误消息的问题。出现此问题的原因是内存清零不正确。
*   解决了导致组策略管理控制台在您关闭后停止工作的问题。系统记录应用程序错误事件 ID 1000 和错误 0xc 0000005(STATUS _ ACCESS _ VIOLATION)。故障模块是 GPOAdmin.dll 的**。**
***   解决了无法在任务管理器中显示启动影响值的问题。*   解决了在间接显示场景中影响 OpenGL 和 GPU 重绘制的问题。*   解决了当**iexplore.exe**在 Microsoft Edge Internet Explorer 模式上下文中运行时，阻止 **ShellWindows()** 返回 **InternetExplorer** 对象的问题。*   解决了在 Microsoft Edge Internet Explorer 模式下影响对话框的问题。*   解决了当您按 F1 键时导致 Microsoft Edge Internet Explorer 模式停止工作的问题。*   解决导致动态数据交换(DDE)对象不正确清理的问题。这可以防止会话断开并导致会话停止响应。*   解决了当您使用超过 50 个窗口树时可能导致设备停止工作的问题。*   解决了阻止某些低完整性流程应用程序正常打印的问题。*   解决了导致证书注册失败并出现错误消息“0x800700a0 (ERROR _BAD_ARGUMENTS)”的问题。*   解决了影响只与 Azure Active Directory (AAD)集成的应用程序的问题。这些应用程序将无法在加入 Active Directory 联合身份验证服务(ADFS)的计算机上运行。*****   解决了在虚拟机脱机时扩展 BitLocker 分区可能导致 BitLocker 损坏虚拟机(VM)系统文件的问题。*   解决了一个遗留问题，该问题可能会导致 **Get-TPM** PowerShell 命令在尝试报告受信任的平台模块(TPM)信息时失败。该命令失败，并显示错误“0x80090011 Microsoft。Tpm.Commands.TpmWmiException，Microsoft。Tpm.Commands.GetTpmCommand "。*   解决了当驱动程序受虚拟机监控程序保护的代码完整性(HVCI)保护时，阻止您卸载和重新加载驱动程序的问题。*   解决了影响使用远程桌面应用将客户端的本地驱动器装载到终端服务器会话的可靠性问题。*   解决了导致登录时远程桌面会话的键盘和远程桌面协议(RDP)客户端不匹配的问题。*   解决了有时会导致简体中文输入法编辑器(IME)完全不可用的问题。*   解决了导致屏幕阅读器将后退按钮描述为“按钮”而不是“后退按钮”的问题。*   解决了当您尝试写入服务主体名称(SPN)别名(如 www/FOO)而 HOST/FOO 已存在于另一个对象上时出现的问题。如果 **RIGHT_DS_WRITE_PROPERTY** 在碰撞对象的 SPN 属性上，您会收到一个“拒绝访问”错误。*   解决了阻止管理员和内容所有者打开过期的 Active Directory Rights Management Services(AD RMS)内容的问题。*   解决了在您重新启动操作系统并登录后断开网络驱动器上的脱机文件的问题。如果分布式文件系统(DFS)路径被映射到网络驱动器，就会出现此问题。*   解决了由于 **vhdmp.sys** 接收同一文件的不同文件控制块(FCB)对象指针而导致虚拟机实时迁移失败的问题。*   解决了在安装网络驱动器时显示两次身份验证对话框的问题。*   解决重定向驱动器缓冲子系统(RDBSS)和 **mrxsmb.sys** 驱动程序中的内存泄漏问题。*   解决导致 WebDav 重定向器死锁的问题。当您尝试从本地 TfsStore 读取文件时，会发生此问题，这会导致系统停止响应。*   解决了阻止工作文件夹同步从客户端上的错误代码 0x80c80003“服务器当前正忙”中恢复的问题。即使服务器上的 HTTP 请求队列没有指示负载，也会出现此问题。*   解决了在页面错误路径中调用上下文函数而导致 7F 错误的问题。​​​​​​**

 **除了 Windows 10 版本 21H2、21H1 和 20H2，还有其他版本的操作系统仅支持商业和教育客户。这些今天也收到更新，但你必须在一个支持的版本或分支才能获得这些更新。您可以在下表中查看并手动下载它们:

你可以手动下载 Windows 10 build 19044.1586 或当今的任何更新，但如果你花的时间太长，它们最终会自动安装。这些都是强制更新，最好在方便的时候尽早安装，这样在你忙的时候就不会打扰你了。

现在也是提醒用户对某些版本的支持即将下降的好时机。从 5 月 10 日开始，Windows 10 版本 20H2 将不再支持家庭版和专业版，而版本 1909 将完全失去支持。现在是开始准备升级以便继续接收安全更新的好时机。**