# 新的 Windows 11 开发预览版增加了更多语言的实时字幕

> 原文：<https://www.xda-developers.com/windows-11-build-25300-live-captions/>

微软再次向 Dev 频道的内部人员发布了新版本的 Windows 11，其中包含了一些显著的变化。本周的构建是 25300，亮点是增加了对更多语言的直播字幕的支持。

## 七种新语言的实时字幕

直播字幕最初是在 [Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2/) 中添加的，但它们只支持美国英语。此功能为所有从您的电脑发出的音频创建字幕，因此如果您有听力障碍，它可以大大有助于使视频和音频更容易理解。

在这个版本中，微软增加了对其他英语方言的实时字幕支持，以及七种新语言，包括中文(简体或繁体)、法语、德语、意大利语、葡萄牙语(巴西)和西班牙语。

## 快照布局更新

这一版本中其他值得注意的变化与 Snap Layouts 有关，这是 Windows 11 首次引入的功能，尽管并非每个人都可以使用。微软正在减少您在“捕捉布局”弹出按钮出现之前将鼠标悬停在最大化/恢复图标上所需的时间，当您选择一个应用程序时，您还会在布局中看到当前应用程序的图标。

微软表示，它将继续尝试这一点，因此在未来的版本中可能会有其他变化。

## 其他改进

除了这些更大的变化，这个版本还有一些其他的改进。首先，微软已经完成了跨设备同步语音输入设置的功能，包括自动标点和语音输入启动器的设置。

此更新还使得在“设置”应用程序的启动页面中访问有关应用程序的更多信息变得更加容易。此外，当你在“开始”菜单中右键单击 Win32 应用程序来卸载它时，你现在会被带到“设置”应用程序，而不是旧的控制面板。最后，微软改进了新的 Linux Windows 子系统的行为，因此当您尝试运行它时，它会自动提示您安装新的商店版本。

当然，还有通常的修复列表，这是一个很长的列表。如果你有兴趣，可以看看下面的列表:

**【通用】**

*   我们修复了与 combase.dll 相关的底层问题，该问题在升级到 Build 25290 后导致使用 GetKnownFolder APIs 的多个应用程序崩溃，包括 IME 用户的记事本和 Windows 终端。这个问题也被认为是一些内部人员发现文件资源管理器中的某些操作在这些版本中需要几分钟才能完成的根本原因。
*   我们修复了导致渲染问题和使用 Windows 恢复环境(WinRE)困难的问题。
*   修复了一些用户在登录需要 windows 集成身份验证的企业网站时遇到问题的问题。

**【任务栏&系统托盘】**

*   在系统托盘上显示时钟秒数的功能，最初是由 [Build 25247](https://blogs.windows.com/windows-insider/2022/11/18/announcing-windows-11-insider-preview-build-25247/) 引入的，如果它在上周更新到 Build 25295 后消失了，应该会在更新到 Build 25300 后恢复。
*   修正了分辨率改变后任务栏被切断的问题。
*   我们修复了一个问题，当鼠标悬停在任务栏上的应用图标上时，可能会意外地切换窗口焦点。

**【小工具】**

*   由于修复了在多个 Windows 11 设备上使用 Microsoft 帐户登录时导致第三方 widgets 被解除锁定的问题，Dev Channel 中最新的 widgets 更新将解除锁定第三方 Widgets。内部人员将需要回到他们的插件板，并再次重新锁定这些插件。如果您仍然看到小工具被意外取消固定的问题，请提交反馈。
*   小部件选择器中“查找更多小部件”的链接现在不再断开，将指向商店收藏[这里](ms-windows-store://collection/?collectionid=MerchandiserContent/Apps/WidgetCollection/Widgetsforeverything)。

**【输入】**

*   我们开始解决 IME 候选窗口和 IME 工具栏有时无法显示或被裁剪的问题。

**【文件浏览器】**

*   跨选项卡拖放文件和文件夹应该可以再次工作。

**【任务管理器】**

*   在搜索框中输入的进程名称不再会被意外地进行拼写检查。
*   修正了讲述人在任务管理器中读出内容的几个问题。
*   修正了设置中的下拉列表可能与你当前选择的主题不匹配的问题。
*   当在应用历史页面使用搜索时，搜索结果不再会突然消失。
*   如果您在设置中打开默认的起始页下拉菜单，单击任务管理器窗口应该会使下拉菜单消失。
*   使用搜索框区域拖动窗口现在应该可以工作了(就像标题栏的其他区域一样)。
*   修正了一个在细节标签中结束进程不显示确认对话框的问题。
*   增加文本缩放比例不再会导致“查看更多”按钮没有内容出现。
*   如果您进行搜索，然后按下向下箭头，键盘焦点现在应该从搜索框移到结果中。
*   如果您启用了一个对比主题，并选择了 Processes 页面中的一行，该行现在应该显示它已被选中。
*   修复了一个问题，焦点可能不会正确设置为搜索，导致讲述人没有说焦点是在搜索框上。

**【其他】**

*   修正了在角色扮演页面中使用后退按钮时，讲述人的焦点不能正确返回快速设置窗口的问题。

尽管有很长的修复列表，仍然有一些已知的问题需要注意。这个列表相当长，如果你想在 Arm64 设备上使用新的实时字幕功能，你可能会遇到一些麻烦。您可以在下面找到更多信息:

**【常规】**

*   我们正在调查一个问题，一些用户在安装最近的版本时经历了比预期更长的更新时间。如果您遇到此问题，请在反馈中心提交一个新的带有日志的反馈项目。
*   一些加入了 AAD (Azure Active Directory)的用户现在在更新最新版本后登录 Windows 时会看到“为您做好准备”屏幕。我们正在调查这个问题。
*   启动组策略编辑器可能会显示找不到 displayName 属性的错误。
*   使用 Windows Hello 通过面部识别登录可能无法在 Arm64 PCs 上运行。解决这一问题的方法是使用 Hello PIN 路径。
*   我们正在调查有关 Windows Insider 程序设置页面显示 Windows Update 中有新版本可用的报告，即使它们是 Dev 频道中最新的可用版本。
*   [ **新** ]我们正在调查关于升级到 Build 25295 后，Snipping 工具中的新按钮对一些内部人员不起作用的报道。如果您受此影响，转到设置>应用程序>默认应用程序，并将屏幕截图设置为 ms-screenclip 的默认应用程序，应该可以解决问题。

**【小工具】**

*   我们正在调查一个问题，在某些情况下，第三方小工具可能无法按预期加载。

**【任务栏&系统托盘】**

*   对于一些拥有多台显示器的内部人员，任务栏上的应用程序图标可能会出现在错误的显示器上。

**【Windows 聚光灯】**

*以下已知问题仅适用于 Windows 内部人员，他们接受了 Windows Spotlight 的一种不同处理方式，该方式开始向内部人员推出* [*内部版本 25281*](https://blogs.windows.com/windows-insider/2023/01/19/announcing-windows-11-insider-preview-build-25281/) *:*

*   点击辅助显示器并不能消除全屏体验。

**【直播字幕】**

*   在 Arm64 设备上，增强的语音识别支持将无法通过语言和区域设置页面正确安装。Arm64 用户不支持带首选语言的实时字幕的语音识别，可以使用此解决方法: *(1)卸载设置>应用>已安装应用中的所有“语音包–”应用条目；(2)在设置>时间&语言>语言&区域将首选语言列表中的第一种语言临时设置为可接受的替代语言；(3)启动直播字幕。*
*   繁体中文实时字幕目前无法在 Arm64 设备上运行。
*   “语言和区域设置”页面上显示的某些语言将表示支持语音识别(如朝鲜语)，但尚不支持实时字幕。
*   通过“语言和区域设置”页面添加语言时，语言功能的安装进度可能会隐藏，并且您可能看不到“增强的语音识别”的安装完成(实时字幕要求)。(您可以使用该语言的“语言选项”来监控进度。)如果发生这种情况，在实时字幕设置体验检测到这种情况并允许您继续之前，可能会有意外的延迟。
*   首次登录后的一个小时内,“语言和区域设置”页面可能不会为实时字幕提供必要的语音识别语言支持。
*   非英语语言中的字幕性能可能会降低，并且在非英语(美国)语言中会丢失语言外过滤，这意味着非字幕语言的语音将显示不正确的字幕。

像往常一样，如果你在开发频道注册，这个新版本应该会自动下载，但你可以进入设置应用程序，访问 **Windows Update** 部分，立即获得最新版本。

* * *

**来源:** [微软](https://blogs.windows.com/windows-insider/2023/02/15/announcing-windows-11-insider-preview-build-25300/)