# 微软将 Windows Insider 测试版分成两条路

> 原文：<https://www.xda-developers.com/windows-11-beta-channel-split-build-22622-290/>

微软正在将 Windows Insider 程序的测试版分成两条独立的路径，作为一种有选择地测试新功能的方式，供内部测试人员测试 [Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2/) 。一组内部人员将会得到 22622.x 范围内的构建，这些构建将拥有默认启用的新特性。另一组内部人员将留在 build 22621.x 中，默认情况下这些支持包是关闭的。

据微软称，目标是测试在默认情况下关闭某些功能的情况下推出更新的可行性，以及衡量启用这些新功能的影响。这两个群体的存在，使微软可以比较数据，从他们两个之前，使功能更广泛可用。然而，那些最终获得没有启用新特性的版本的人可以再次检查更新以找到启用它们的版本。

为此，微软推出了 Windows 11 版本 22622.290 和 22621.290，带来了一些改进，特别是以前的版本。具体来说，Windows 11 build 22622.290 包括一些以前在开发频道推出的功能，如建议的操作。这样，当你选择并复制代表某个特定信息的文本时，比如一个电话号码，你会立即看到一个选项，例如在团队中呼叫那个号码。如果您选择了一个日期，您可以在 Outlook 中为它创建一个事件。这仅适用于美国和加拿大的用户。

另一项新功能是在“设置”的“帐户管理”页面中支持独立 OneDrive 订阅。以前，您只能看到有关正确的 Microsoft 365 订阅的信息。

除此之外，还有几个版本 22622.290 独有的修复。你可以在下面看到它们:

### Windows 11 内部版本 22622.290 中的修复

**【文件浏览器】**

*   在文件浏览器的主体中点击鼠标中键将会在一个新的标签中打开它。
*   当按 Tab 或 F6 时，这一行标签现在应该包含在键盘焦点循环中。一旦焦点位于选项卡行中，您可以使用左箭头键或右箭头键在它们之间导航。
*   修正了当你在文件浏览器中重新排列标签时，使用 CTRL + Tab 时标签顺序会出错的问题。
*   做了一些调整，当“在标题栏显示完整路径”被启用，以确保文件夹名称总是可见的。
*   修正了一个缩放问题，该问题可能会导致选项卡意外变大。
*   右键单击一个选项卡，然后在文件浏览器中单击其他地方，现在应该可以更可靠地关闭上下文菜单。

除此之外，一些修正适用于今天推出的两个版本。这些建议如下:

### Windows 11 中的修复版本为 22622.290 和 22621.290

*   ***新增！*** 我们增加了服务器消息块(SMB)重定向器(RDR)特定的公共文件系统控制(FSCTL)代码 fs CTL _ LMR _ 查询 _ 信息。
*   ***新！*** 我们在 Windows 客户端和服务器轻量级目录访问协议(LDAP)实现中增加了对传输层安全性(TLS) 1.3 的支持。
*   我们更新了 **Remove-Item** cmdlet，以正确地与 Microsoft OneDrive 文件夹交互
*   我们启用了**InternetExplorerModeEnableSavePageAs**组策略。有关更多信息，请参见[微软 Edge 浏览器政策文档](https://docs.microsoft.com/deployedge/microsoft-edge-policies#internetexplorermodeenablesavepageas)。
*   我们修复了一个问题，当你使用一个公共文件对话框打开相机时，拍照按钮会消失。
*   我们修复了一个问题，该问题会阻止设备从 Windows Update 接收相同扩展驱动程序的报价，因为该扩展驱动程序已安装，但没有基本驱动程序。
*   我们修复了导致 Active Directory 从媒体安装(IFM)创建失败的问题，并显示错误“2101 JET_errCallbackFailed”。
*   我们修复了 Active Directory 轻型目录服务(LDS)重置 userProxy 对象的密码时出现的问题。密码重置失败，并出现错误，如“00000005: SvcErr: DSID-03380C23，问题 5003 (WILL_NOT_PERFORM)，数据 0”。
*   我们启用了**InternetExplorerModeEnableSavePageAs**组策略。有关更多信息，请参见[微软 Edge 浏览器政策文档](https://docs.microsoft.com/deployedge/microsoft-edge-policies#internetexplorermodeenablesavepageas)。
*   我们修复了 Active Directory 轻型目录服务(AD LDS)重置 userProxy 对象的密码时出现的问题。当您尝试重置其他人的密码并且您使用简单绑定进行了身份验证时，密码重置会失败。错误类似于“00000005: SvcErr: DSID-03380C23，问题 5003 (WILL_NOT_PERFORM)，数据 0”。
*   我们修复了阻止 Microsoft Edge 在 Windows 沙盒中可用的问题。

当然，在这些构建中仍然有一些已知的问题，但是现在只有两个，这表明开发正在慢慢接近完成。以下是需要注意的问题:

### Windows 11 内部版本 22622.290 和 22621.290 中的已知问题

**【常规】**

*   我们正在修复一个问题，该问题导致测试版渠道中的少数内部人员在 Windows UI 组件(如 explorer.exe)中经历周期性崩溃，使屏幕看起来在闪烁。如果您受到影响，从提升的 PowerShell 窗口运行以下命令应该可以解决问题:Add-appx package-Register-Path C:\ Windows \ system apps \ Microsoft。UI . xaml . CBS _ 8 wekyb 3d 8 bbwe \ app xmanifest . XML-disabled development mode-ForceApplicationShutdown

**【文件浏览器】**

*   文件资源管理器选项卡中的向上箭头没有对齐。这将在未来的更新中得到解决。

如果您想要获取最新的更新，只需在 Windows Update 中检查更新即可。如上所述，如果您在开始时没有启用新功能，您可以在安装更新后再次检查更新，以找到 build 22622.290。