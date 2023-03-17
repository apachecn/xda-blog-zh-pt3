# 微软在 Dev 频道发布了 Windows 11 build 25140，并附有修复程序

> 原文：<https://www.xda-developers.com/windows-11-build-25140-fixes/>

微软正在为在 Dev 频道注册的内部人员推出 Windows 11 的新版本，使版本号达到 25140。在上周的版本在文件浏览器中引入了标签之后，这次的更新更加温和了，集中在对各种问题的修复上。

有一个更明显的改进，它与 Euphemia 字体有关，其中包括一些使用加拿大音节文字的语言，如 Inuktitut。升级后的字体使 200 多个字符更加易读，并改善了它们的屏幕呈现，此外它还支持 Unicode 14 标准中的新字符。

除此之外，都是修复，包括一些集中在文件浏览器标签。奇怪的是，这一功能仍然没有在 Dev 频道的内部人员中完全推出，尽管 Beta 频道的一些用户[也已经可以尝试它了](https://www.xda-developers.com/windows-11-22h2-gets-its-first-update-since-rtm-in-the-beta-channel/)。这符合微软对 Insider 计划的指导，但仍然奇怪的是，专门注册尝试最新功能的用户仍然需要等待它们被启用，而其他用户已经可以尝试它们了。

这个版本也有一些已知的问题，包括一个可能导致使用 Easy 反作弊技术的游戏崩溃的问题。像这样的问题在开发通道中是一个常数，因为它几乎总是被用于在开发的非常早期阶段测试构建。在这个时候，大多数人真的没有理由加入这个频道，因为他们会在不稳定的版本中停留一段时间，并且没有很多值得注意的开发频道独有的功能。您可以在下面看到修复和已知问题的完整列表。

### Windows 11 构建 25140 个修复程序

### **【文件浏览器】**

*   修复了一个导致一些人在从网络驱动器复制文件时意外看到错误 0x80070026 的问题。
*   修正了一个问题，即活动选项卡的颜色与它下面的命令栏不匹配。
*   修正了拖动标签重新排列有时不起作用的问题。
*   修复了一个问题，如果文件资源管理器被最大化，而你使用 WIN + M 最小化它，可能会导致任务栏中的 windows 缩略图预览出现瑕疵。

### **【设置】**

*   如果您在系统>存储>磁盘和卷中重命名驱动器标签，当前的驱动器名称现在会预填充在对话框中。

### **【输入】**

*   修正了在 OOBE 选择英语(纽西兰)会意外导致阿拉伯语(101)键盘被选择的问题。
*   设置语言栏热键直接将输入切换到特定的非 IME 输入法现在应该可以工作了。
*   某些语言不支持文本到语音转换。当管理员用户试图使用[新的安装语言 CopyToSettings 命令](https://blogs.windows.com/windows-insider/2022/02/16/announcing-windows-11-insider-preview-build-22557/)安装其中一种语言时，一些设置如新用户帐户区域设置、输入(键盘)和 UPLL(用户首选语言列表)没有得到更新。此问题现已修复。
*   修复了在使用 Office online 应用程序时，当这些字体不在您的 PC 上时，导致 Batang、BatangChe、Gungsuh 和 GungsuhChe 字体无法正确呈现朝鲜语的问题。

### **【任务经理】**

*   修复了在进程页面之外的页面中切换模式时可能发生的崩溃。
*   我们对流程页面上热图中使用的颜色强度做了一点小小的调整。

### **【其他】**

*   修复了一个问题，如果 LPACCEL 参数是 ACCEL 结构数组中奇数编号的索引的地址，则调用 [CopyAcceleratorTable](https://docs.microsoft.com/windows/win32/api/winuser/nf-winuser-copyacceleratortablea) 和 [CreateAcceleratorTable](https://docs.microsoft.com/windows/win32/api/winuser/nf-winuser-createacceleratortablea) 会失败。
*   修复了 ARM64 上 x64 仿真的一个问题，该问题可能导致某些应用程序在启动时崩溃，错误代码为 0xc0000409。
*   修复了导致音频在一分钟后在某些应用程序中停止播放的问题。

### Windows 11 内部版本 25140 已知问题

### **【常规】**

*   Surface Pro X 设备上的 Windows Insiders 在尝试从休眠状态恢复时会出现黑屏。您需要重启电源(长时间关闭电源按钮)才能回到设备中。建议这些设备上的内部人员暂停飞行，直到我们发布带有此修复的版本。
*   我们正在调查关于[云母材料](https://docs.microsoft.com/en-us/windows/apps/design/style/mica)和[丙烯酸](https://docs.microsoft.com/en-us/windows/apps/design/style/acrylic)模糊效果在操作系统表面(如开始菜单、通知中心和其他区域)呈现不正确的报告。
*   我们正在调查关于通过开始菜单关机对一些内部人员不起作用，而是意外重启的报道。
*   一些使用 Easy Anti-check 的游戏可能会崩溃或导致您的电脑进行错误检查。

### **【文件浏览器】**

*   文件资源管理器选项卡中的向上箭头没有对齐。这将在未来的更新中得到解决。
*   **【新功能】**我们正在调查关于在使用黑暗模式时以特定方式(例如，从命令行)启动文件资源管理器会在明亮模式下意外显示文件资源管理器主体的报告。

*   **【新】**我们正在修复一个导致控件偏好设置(温度单位和固定控件)意外重置为默认值的问题。

### **【直播字幕】**

*   全屏模式下的某些应用程序(如视频播放器)会阻止显示实时字幕。
*   位于屏幕顶部附近并在运行实时字幕前关闭的某些应用程序将在位于顶部的实时字幕窗口后重新启动。当应用程序有焦点时，使用系统菜单(ALT +空格键)将应用程序的窗口进一步下移。

如果你期待 Windows 11 的下一步，测试版和发布预览版频道[目前正在测试 Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2-available-release-preview-channel/) ，测试版频道还可以访问文件资源管理器标签。目前还不完全清楚这项功能是否会在正式发布时成为 Windows 11 版本 22H2 的一部分，但似乎很可能是这样的。

* * *

来源:[微软](https://blogs.windows.com/windows-insider/2022/06/15/announcing-windows-11-insider-preview-build-25140/)