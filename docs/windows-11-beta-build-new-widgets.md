# Windows 11 测试版为 Spotify、Game Pass、Phone Link 和 Messenger 提供了插件

> 原文：<https://www.xda-developers.com/windows-11-beta-build-new-widgets/>

微软在测试频道为 Windows 内部人士提供了一个最新的待遇。有两个新的 [Windows 11](https://www.xda-developers.com/windows-11/) 版本可供下载。Build 22623.1325 是为那些推出新功能的人准备的，build 22621.1325 是为那些默认关闭新功能的人准备的。在这两个版本中，您可以享受 Spotify、Game Pass、Phone Link 和 Messenger 的一些新插件。这是在解决 Windows 内部人士报告的问题的常规 bug 调整之上的。

### 两个版本中的新功能

正如我们刚才所说的，这两个版本中**的亮点是新的部件。你可以去微软商店的 [widgets collection](http://ms-windows-store://collection/?collectionid=MerchandiserContent/Apps/WidgetCollection/Widgetsforeverything) 获取最新版本的 Spotify、Game Pass、Phone Link 和 Messenger 应用来抓取这些 widgets。然后，您应该可以看到面板上的小部件，方法是单击右上角的“+”按钮，将它们固定在您喜欢的位置。这一切之所以成为可能，是因为 Windows App SDK 1.2 允许开发人员为他们的应用程序创建小部件。以前，这个功能只在不太稳定的 Windows 11 开发频道中可用，所以很高兴看到这里的扩展。**

请注意，此版本还带来了一项新策略，使商业客户能够启用通过服务(年度功能更新之外)引入的功能，这些功能对于其 Windows 更新受管理的设备来说是默认关闭的。如果你是一名 IT 管理员，你可以通过微软了解更多关于这个[的信息。](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/commercial-control-for-continuous-innovation/ba-p/3737575)

### 两种版本的修复

在这两个版本中，微软推出了一系列的变化。这些会影响打印机、任务视图、蓝牙键盘等等。我们已经把你需要知道的一切都包括在下面了。

*   我们修复了影响某些打印机的兼容性问题。这些打印机使用 Windows 图形设备接口(GDI)打印机驱动程序。那些驱动程序没有完全遵守 GDI 规范。
*   我们修复了使用任务视图时出现的可靠性问题。
*   我们修复了一个影响从网络复制到本地驱动器的问题。对于某些用户来说，复制速度比预期的要慢。
*   我们为墨西哥合众国 2023 年夏令时变更令提供了支持。
*   我们修复了日期信息问题。它影响了 Windows 和某些版本的 Heimdal Kerberos 库之间发送的日期格式。
*   我们修复了一个影响配置包的问题。当需要提升时，它们在某些情况下不适用。
*   我们修复了一个问题，该问题会影响哪些文件夹出现在浏览文件夹选择器中。
*   我们修复了一个影响文件浏览器的问题。当您使用 Shift + Tab 或 Shift + F6 时，输入焦点不会移动。
*   我们修复了一个影响用户界面(UI)的问题。蓝牙键盘上的调高音量和调低音量命令未显示。
*   在您安装更新后，我们提高了 Windows 的可靠性。
*   我们修复了一个可能影响到 lsass.exe 的问题。当它向具有非常大的 LDAP 筛选器的域控制器发送轻型目录访问协议(LDAP)查询时，它可能已经停止响应。
*   我们修复了一个影响 Azure Active Directory (Azure AD)的问题。使用预配包进行批量预配失败。
*   我们修复了一个影响软件键盘的问题。在[按钮复位](https://learn.microsoft.com/windows-hardware/manufacture/desktop/how-push-button-reset-features-work?view=windows-11)(工厂复位)后，它没有出现在开箱即用体验(OOBE)中。这种类型的重置需要连接外部键盘来提供凭据。
*   我们修复了一个影响 AppV 的问题。它阻止文件名具有正确的字母大小写(大写或小写)。
*   我们修复了一个影响通用打印的配置服务提供商(CSP)的问题。安装打印机时会出现一个命令提示符窗口。
*   我们修复了一个可能影响触摸键盘和 PIN 输入键盘的问题。当您登录到设备时，可能无法使用它们来输入文本。
*   我们修复了视频播放时显示蓝屏的问题。这发生在您在显示器上设定高动态范围(HDR)之后。
*   我们修复了一个影响奇偶校验虚拟磁盘的问题。使用服务器管理器创建它们失败
*   我们修复了一个影响 IE 模式的问题。状态栏上的文本并不总是可见的。
*   我们修复了一个影响滤色器设置的问题。当您选择反转时，系统会将其设置为灰度。
*   我们修复了一个影响 Microsoft Edge 的问题。该问题删除了 Microsoft Edge 的冲突策略。当您在 Microsoft Intune 租户中设置 **MDMWinsOverGPFlag** 并且 Intune 检测到策略冲突时，会发生这种情况。
*   我们修复了一个影响 Appx 状态库的问题。删除用户配置文件时，清理未完成。正因为如此，它的数据库增长了久而久之。这种增长可能会导致用户登录 FSLogix 等多用户环境时出现延迟。

### 内部版本 22623.1325 中的其他更改和修复

随着 **just build 22623.1325** ，微软增加了在 Azure Active Directory 加入设备的开始菜单中查看人工智能推荐内容的能力。你会看到普通 Windows 11 用户熟悉的内容，比如建议文件，以及你之前可能评论过或打开过的其他内容。这是对导致任务栏在分辨率改变后被切断的修复的补充。

本周 Beta 频道的行动到此结束。提醒一下，如果你也在运行 Windows 11 的 Dev channel 版本，你会在周三得到一个新版本。开发者增加了对更多语言的实时字幕支持，并对微软商店进行了改造，在商店的主页上为特色产品提供了更简洁的用户界面，更简洁的搜索结果页面，以及更简洁的应用程序产品卡设计。

**来源:** [微软](https://blogs.windows.com/windows-insider/2023/02/16/announcing-windows-11-insider-preview-build-22621-1325-and-22623-1325/)