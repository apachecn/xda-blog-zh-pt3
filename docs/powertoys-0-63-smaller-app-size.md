# 微软发布了 PowerToys 0.63，其应用程序的大小要小得多

> 原文：<https://www.xda-developers.com/powertoys-0-63-smaller-app-size/>

微软已经发布了 0.63 版本的 PowerToys 生产力工具套件，这是一个更完善的更新。虽然它没有增加很多新功能，但这个版本的 PowerToys 在效率方面确实有一些重大改进。该团队已经将 PowerToys 安装程序的大小从 125MB(在版本 0.62.1 中)减少到 83MB。而且，一旦安装，这个应用现在只占用 587MB，而不是 817MB。

微软表示，这是通过在不同工具之间共享 Windows 应用程序 SDK、VC++可再发行版和 PowerToys Interop 等文件来实现的。这也应该有助于在安装过程中消除对用户帐户控制(UAC)的需求，尽管在此之前还有很多工作要做。接下来，该公司还将推出一个独立版本的。NET 在不同的工具之间共享。

此版本的另一个亮点是 QuickAccent 工具，它可以让您快速找到字符的重音版本，现在可以让您选择一种语言，以减少您在键入时需要选择的字符数。

除此之外，这个版本主要集中在修复和微小的改进上，并且有很多是针对 PowerToys 中包含的各种实用程序的。你可以在下面找到完整的列表。

### PowerToys 0.63 变更日志

**已知问题**

**将军**

*   修复了导致错误报告生成失败的问题。(这是 0.62 的修补程序)
*   已将 Windows App SDK 运行时更新至 1.1.5。

**永远在顶端**

*   修复了在虚拟桌面之间移动窗口时导致边框逗留的问题。
*   现在，边框的最小厚度为 1。感谢 [@unuing](https://github.com/unuing) ！
*   边框显示在虚拟桌面的缩略图中。这些被移除了。
*   修正了边框视觉效果，使其更贴近应用程序的边框。

**清醒**

*   修复了实用程序退出逻辑，以关闭所有线程并避免崩溃。(这是 0.62 的修补程序)

**颜色选择器**

*   修复了实用程序退出逻辑，以关闭所有线程并避免崩溃。(这是 0.62 的修补程序)
*   修复了导致鼠标位置设置错误的初始化错误。

**FancyZones**

*   修复了 FancyZones 编辑器退出逻辑，以关闭所有线程并避免崩溃。(这是 0.62 的修补程序)

**文件浏览器附加组件**

*   将 WebView 2 依赖项更新为 1.0.1343.22。感谢[@亚伦-勇克](https://github.com/Aaron-Junker)！
*   的固定预览。注册文件。

**图像缩放器**

*   修正了在某些情况下访问上下文菜单时导致文件浏览器崩溃的错误。

**电动玩具跑**

*   增加了在地震模式下打开终端窗口的支持。感谢 [@FWest98](https://github.com/FWest98) ！
*   修复了实用程序退出逻辑，以关闭所有线程并避免崩溃。(这是 0.62 的修补程序)
*   改进应用程序执行别名的程序插件中显示的图标。感谢 [@MikeBarker-MSFT](https://github.com/MikeBarker-MSFT) ！
*   修复从微软商店安装 Firefox 时对默认浏览器的调用。
*   修正了附加到结果条目的控件没有被公布的可访问性问题。
*   搜索得到了改进，现在应该返回查询中的术语出现在结果末尾的结果。

**快速口音**

*   改进了键盘挂钩的性能。(这是 0.62 的修补程序)
*   修正了一个导致快速重音干扰键盘管理器的错误。(这是 0.62 的修补程序)
*   添加了正确的大写字母。感谢[@亚伦-勇克](https://github.com/Aaron-Junker)！
*   重音字符选择现在应该换行。感谢 [@wmentha](https://github.com/wmentha) ！
*   添加了语言选择设置，以减少显示的重音字符的数量。可用的语言有货币、捷克语、荷兰语、法语、匈牙利语、冰岛语、意大利语、毛利语、拼音、波兰语、罗马尼亚语、斯洛伐克语、西班牙语和土耳其语。感谢 [@damienleroy](https://github.com/damienleroy) ！

**屏幕标尺**

*   改进的用户界面/UX 和设置描述。
*   修复了实用程序退出逻辑，以关闭所有线程并避免崩溃。(这是 0.62 的修补程序)

**设置**

*   UI 图标已更新。感谢 [@Jay-o-Way](https://github.com/Jay-o-Way) ！
*   描述改进和歧义消除。感谢 [@Jay-o-Way](https://github.com/Jay-o-Way) ！
*   修正了复选框边距和其他设计调整。感谢 [@Jay-o-Way](https://github.com/Jay-o-Way) ！

**文本提取器**

*   删除了识别中文、日文或韩文时多余的空格。谢谢 [@TheJoeFin](https://github.com/TheJoeFin) ！
*   修复了实用程序退出逻辑，以关闭所有线程并避免崩溃。(这是 0.62 的修补程序)
*   修正了右键点击时选择开始的问题。

**安装人员**

*   添加了在尝试更新. NET 之前在升级时退出 PowerToys 的逻辑。
*   更新了。净依赖于 6.0.9。
*   为引导程序添加了更清晰的安装步骤名称。感谢 [@htcfreek](https://github.com/htcfreek) 和 [@Jay-o-Way](https://github.com/Jay-o-Way) ！
*   Windows App SDK、VC++可再发行版和 PowerToys Interop 运行时文件现在通过硬链接在实用程序之间共享，从而减小了安装大小。

**文档**

*   修复了键盘管理器文档中的拼写错误。感谢[@ elto clear](https://github.com/eltociear)！
*   用 learn.microsoft.com 取代了 docs.microsoft.com。感谢[@亚伦-勇克](https://github.com/Aaron-Junker)！

**发展**

*   修复了一个构建错误，该错误限制开发人员在没有首先清理本地构建文件的情况下在配置之间切换。
*   C++异常捕获被更正为通过引用来捕获，以避免不必要的复制操作。感谢 [@NN -](https://github.com/NN---) ！
*   一般的 C#代码清理、格式修复和删除未使用的代码分析抑制。
*   从 XAML 文件中删除了不必要的`muxc`前缀。感谢 [@Jay-o-Way](https://github.com/Jay-o-Way) ！
*   对依赖于 WebView2 的管道重新启用测试。
*   Windows 11 第 1 层上下文菜单包现在包含“Microsoft。PowerToys”前缀。

然而，有几个已知的工具正在开发中，而不是在这个版本中。微软工程师 Clint Rutkas 最近分享了一个[“文件锁匠”工具](https://github.com/microsoft/PowerToys/pull/20863)，它可以让你看到什么进程正在使用一个给定的文件，这可以防止该文件被删除。我们过去也看到过 [PowerToys Peek](https://www.xda-developers.com/powertoys-peek-windows-version-macos-quick-look/) 的演示，它的行为就像 macOS 中 Windows 版本的 Quick Look。这些工具还没有出现在 PowerToys 版本中，但希望它们很快就会出现。

* * *

**来源:** [GitHub](https://github.com/microsoft/PowerToys/releases/tag/v0.63.0)