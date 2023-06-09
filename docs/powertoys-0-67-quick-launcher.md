# PowerToys update 为您最喜爱的工具添加了一个快速启动器

> 原文：<https://www.xda-developers.com/powertoys-0-67-quick-launcher/>

微软为 PowerToys 推出了新的更新，这是一套为 Windows 11 和 Windows 10 的超级用户提供的工具。最新的更新为我们带来了 0.67 版本，该版本的亮点是新的快速启动面板，它位于系统托盘中。

您可以打开此面板，查看 PowerToys 中最常用工具的快捷方式，如 Hosts 文件编辑器、文本提取器等。这意味着您无需在每次想要使用时创建复杂的键盘快捷键或打开 PowerToys 主窗口，因此可以节省您的宝贵时间。不同的工具可以被固定或从启动器中移除，你也可以随意重新排列它们。

除此之外，这个版本主要是关于代码质量的改进。微软在 PowerToys Run 中增加了一个新选项，允许你使用**标签**键来浏览搜索结果，而不是界面中的其他按钮。快速重音工具也已经更新，增加了更多语言的字符，如希伯来语，以及新的破折号字符。

这还不是最大的更新，但微软一直在为 PowerToys 添加新工具。最近，增加了 File Locksmith，让用户看到什么程序正在使用某个文件，文本提取工具也是最近才增加的，允许你从图像中提取文本。

有关此版本中较小的改进和修复的完整列表，您可以在下面找到:

**清醒**

*   禁用而不是隐藏“保持屏幕打开”选项。

**FancyZones**

*   重构并提高了代码质量。

**文件资源管理器附件**

*   修复了预览开发者文件时转义 HTML 敏感字符的问题。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！

**图像缩放器**

*   改进了向微软服务器报告的无声崩溃的代码质量。

**电动玩具运行**

*   仅在结果中添加选项卡选项。感谢 [@maws6502](https://github.com/maws6502) ！
*   系统插件-更新了回收站命令，允许打开回收站。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   系统插件-改进了回收站命令，在删除运行时不会阻止 PT 运行。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   系统插件-其他小的改变来提高回收站命令的可用性。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   WindowWalker 插件-用 action 关键字显示所有打开的窗口。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！

**快速重音**

**设置**

*   修正了“最新消息”屏幕上的 URL 点击崩溃问题。
*   增加了快速访问系统托盘启动器。感谢 [@niels9001](https://github.com/niels9001) ！

**文档**

**开发**

*   验证 notice.md 文件和使用的 NuGet 包是否同步。
*   打开 C++代码分析并增量修复警告。
*   自动添加列表。NET 运行时依赖于安装程序。感谢 [@snickler](https://github.com/snickler) ！
*   将所有安装程序注册表项移动到 HKCU。
*   重构安装程序——将与模块相关的内容从 Product.wxs 提取到每个模块。wxs 文件。
*   增强 ARM64 构建配置验证。感谢 [@snickler](https://github.com/snickler) ！
*   帮助确定了影响 PowerToys 文件资源管理器加载项的 WebView2 问题，该问题已在上游得到修复，并通过常用的 Windows 更新渠道作为更新发布。

如果你还没有，你可以从项目的官方 GitHub 页面下载 PowerToys，也可以通过微软商店下载 PowerToys。