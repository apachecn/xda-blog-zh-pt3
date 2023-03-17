# 最新的 Windows 11 更新修复了损坏的任务管理器颜色，并添加了 OneDrive 存储警报

> 原文：<https://www.xda-developers.com/latest-windows-11-update-fixes-broken-task-manager-colors/>

我们现在是 12 月的第二个星期二，这意味着 2022 年的最后一个星期二。事实上，今天，微软发布了今年最后一次 Windows 11 累积更新，因为可选的 C 和 D 更新在假期暂停。Windows 11 的两个支持版本都在更新，包括初始版本和 [Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2/) 。

## Windows 11 版本 22H2 -内部版本号 22621.963

从 Windows 11 版本 22H2 的用户开始，今天推出的更新被标记为 [KB5021255](https://support.microsoft.com/en-us/topic/december-13-2022-kb5021255-os-build-22621-963-8286ffb4-d1a6-4510-b637-5414e64d7da3) ，它的内部版本号达到了 22621.963。如果你有兴趣这样安装的话，你可以在这里手动下载更新。

此次更新的亮点是修复了任务管理器中颜色显示不正确的[问题，这是 11 月底](https://www.xda-developers.com/windows-11-november-optional-update-task-manager-issue/)发布的[可选更新突然出现的问题。还有一个影响数据保护应用程序编程接口(DPAPI)解密的问题的修复，该问题可能会导致某些 VPN 连接无法正常工作。](https://www.xda-developers.com/windows-11-optional-update-kb5020044-windows-spotlight/)

否则，这个更新将包括 11 月可选更新的所有修复和更改，但这一次它们是强制性的。这包括 OneDrive 云存储的新存储提醒，这将显示在设置应用程序中，以及查看您订阅的所有 OneDrive 存储的能力。

微软还将 Windows Spotlight 与设置应用的个性化页面中的通用主题设置进行了合并。这意味着你现在可以选择 Windows Spotlight 主题来获得每天旋转的桌面背景，而不必专门进入背景设置(尽管你仍然有这个选项)。可选的 11 月更新还有更多的内容，比如对组织消息的支持。

## Windows 11(初始版本)-内部版本号 22000.1335

与此同时，仍在 Windows 11 初始版本上的用户正在获得一个标签为 [KB5019157](https://support.microsoft.com/en-us/topic/december-13-2022-kb5021234-os-build-22000-1335-56a94ce4-7122-447d-98d8-360e95fc0cf9) 的更新，这使得内部版本号达到了 22000.1335。你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5021234)手动下载更新。

此更新本身并不包括太多内容，尽管它对上面提到的 DPAPI 解密问题进行了相同的修复，因此它应该可以解决您可能遇到的一些 VPN 连接问题。

否则，所有更新都来自于 11 月中旬发布的可选更新。这包括一个更新的 Quick Assist 应用程序，用于远程帮助其他用户，以及各种其他修复和改进，包括对 Microsoft Store 可能经常无法安装更新的问题的修复。你可以在下面找到完整的变更日志。

*   ***新！*** 它为您的客户端设备提供快速辅助应用程序。
*   ***新！*** 它提供了一种验证 Azure Active Directory 加入设备的方法，以确定它们是否在受信任的网络上。这有助于 Windows Defender 防火墙应用由您的组织配置的正确策略。该功能仅适用于企业客户。IT 管理员必须使用移动设备管理(MDM)策略来配置此功能。有关如何配置配置服务提供商(CSP)的更多信息，请参见[策略 CSP–网络列表管理器](https://learn.microsoft.com/windows/client-management/mdm/policy-csp-networklistmanager#networklistmanager-allowedtlsauthenticationendpoints)。
*   它解决了 Microsoft Store 的一些持续更新故障。
*   它解决了斐济共和国今年暂停夏令时(DST)的问题。
*   它解决了影响企业管理的某些设备的问题。这提高了他们安装应用程序的可靠性。
*   它解决了一个影响统一更新平台(UUP)内部客户的问题。它消除了阻止他们获取离线语言包的障碍。
*   它解决了影响群集名称对象(CNO)或虚拟计算机对象(VCO)的问题。密码重置失败。错误消息是，“重置 AD 密码时出错...// 0x80070005”。
*   它解决了一个影响 Microsoft Direct3D 9 (D3D9)的问题。当您使用 Microsoft 远程桌面时，它会导致 D3D9 停止工作。
*   它解决了影响 Windows 防火墙服务的一个问题。当您打开“覆盖块规则”选项时，它不会启动。
*   它解决了一个可能影响在 Windows 锁定策略(WLDP)下运行的应用程序的问题。他们可能会停止工作。
*   它解决了一个影响 Microsoft Defender for Endpoint 的问题。自动调查阻止实时响应调查。
*   它解决了一个影响 TextInputHost.exe 的问题。它停止响应。
*   它解决了影响“开始”菜单上固定应用程序的问题。当您在已锁定的应用程序页面之间移动时,“开始”菜单停止工作。当语言是从右向左(RTL)语言时，会出现此问题。

* * *

由于这些是强制更新，如果您的计算机已打开并连接到互联网，它们将自动安装。如果您想防止意外的重新启动，您可以手动安装它们，但是它们会尽快安装。同样，这些应该是今年的最后一次更新，除非可能出现任何紧急的带外更新。