# 如何使用 ViveTool 强制启用 Windows 11 中的新功能

> 原文：<https://www.xda-developers.com/how-use-vivetool-enable-features-windows-11/>

似乎过了漫长的时间，[文件浏览器标签终于对每个人可用了](https://www.xda-developers.com/windows-11-22h2-file-explorer-tabs-available/)随着第一个功能下降为 [Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2/) ，也就是 2022 年的更新。准确地说，微软不久前在 Windows 代码库[中添加了标签界面功能](https://www.xda-developers.com/microsoft-bringing-tabs-file-explorer-windows-11/)，但实际的可用性取决于几个因素，如更新渠道和服务器端 A/B 测试。事实上，就像选项卡式文件浏览器一样，大多数实验性功能现在都通过一个名为 Windows 功能商店的核心操作系统组件推送到 Windows，该组件控制着逐步推出。

由于 Windows 功能存储受到 Windows 内核的严格保护，您不能使用典型的二进制补丁技术来强制启用此类功能。这就是 ViVeTool 发挥作用的地方。即使您不是开发人员并且正在阅读这篇文章，您也很有可能已经使用过一两次 ViVeTool，以便在公开推出之前获得一些功能。但这并不是 Windows 功能商店可以改变的全部。下面是如何激活 ViveTool。

## 什么是 Windows 功能商店？

在微软的术语中，现代 Windows 操作系统中的“功能”是 UI 和/或 UX 的变化——从用菜单打开[到任务栏上下文菜单](https://www.xda-developers.com/windows-11-build-22622-440-open-with-taskbar-flow/)中的[任务管理器条目。如前所述，Windows 10 及更新版本中的 A/B 功能实验机制由 Windows 功能商店控制。这个存储(内部称为“Velocity”)是大多数未记录的](https://www.xda-developers.com/windows-11-build-22621755-task-manager-taskbar-menu/) [Windows 通知工具](https://www.youtube.com/watch?v=MybmgE95weo) (WNF)的一部分，它是一个内核组件，用于在整个系统中分发通知，包括其他内核组件、系统服务和用户空间应用程序。

现在，大多数实验性功能都通过一个名为 Windows 功能商店的核心操作系统组件推向 Windows，该组件控制着逐步推出。

构建各种功能的模块化基础设施本质上是设计受控部署模型的一种方式。例如，Windows Insider 计划用于为早期更新提供正在进行的功能，这些功能随后会进行增量修补，并在达到稳定性里程碑后为每个用户启用。如果某个特定的特性包含灾难性的错误或有安全缺陷，它可以被内核无缝禁用。

## 我们可以绕过服务器端的 A/B 测试吗？

请记住，内部和稳定渠道版本通常都附带了过多的“特性”,这些特性对应于处于休眠状态的新功能。抛开受控的首次展示方面，远程编排的 A/B 测试(也称为分割测试)可以确保跨多个配置的持续改进和快速反馈循环。Windows 功能存储通过保护功能切换状态来保护随机实验过程。

幸运的是，**可以操作存储在 Windows 功能库**中的数据。许多有才华的开发人员已经成功地对 Windows 的内部功能控制 API 进行了逆向工程。要访问 Windows 功能商店，你可以使用拉斐尔·里维拉的 [Mach2 或卢卡斯的](https://github.com/riverar/mach2) [ViVeTool(又名 the book disclosed](https://github.com/thebookisclosed/ViVe))等应用程序，并完全绕过服务器端的 A/B 测试。

在某些情况下，您可能能够修改注册表——`HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FeatureManagement\Overrides\`部分，以更改特性存储变量。然而，我们建议坚持特定于 ID 的特性状态修改，以避免不可预见的情况。

## 功能 id

Windows 功能商店中的每个功能都有一个唯一的 ID，比如 26008830 对应[平板优化任务栏](https://www.xda-developers.com/microsoft-tablet-optimized-taskbar-windows-11-beta-channel/)。每个特征 ID 有三种状态:

*   默认值(0):这是特定功能的正常行为。
*   Disabled (1):这将完全禁用该功能。
*   Enabled (2):这将强制启用该功能。

Mach2 [的开发者为每个内部版本维护一个特性 id](https://github.com/riverar/mach2/tree/master/features)列表。repo 还包含构建之间的变更，这对于识别新的隐藏特性很有用。您还可以使用名为 [ViVeTool GUI](https://www.xda-developers.com/vivetool-gui-enable-hidden-windows-11-features/) 的 ViVeTool 图形分支来搜索任何 Windows 版本的可用特性 id。

修改特性 id 会导致不稳定或崩溃。由于相互依赖，有些可能会破坏核心操作系统模块，使 Windows 完全不可用。您还可能遇到一些特性 id，它们做出了无法恢复的永久更改。继续进行，风险自负。

由于 Windows Update 机制和 Windows 功能存储的关联方式，更改某些功能可能足以将您的设备置于不受支持的状态。强烈建议您在选择试用 Windows 功能商店之前进行映像备份。或者，在虚拟机中进行评估。

下面你可以找到一些流行的 Windows 功能和相应的功能 id 列表。

| 

功能描述

 | 

功能 ID

 | 

最低 Windows 版本

 |
| --- | --- | --- |
| 文件浏览器中的选项卡 | 37634385 | 21536 |
| 平板电脑优化的任务栏 | 26008830 | 25197 |
| 改进的小部件用户界面 | 40772499 | 25227, 22623.746 |
| 新系统托盘 | 38764045 | 25211 |
| 小组件设置菜单 | 38652916 | 25217 |
| 任务管理器中的搜索栏 | 39420424 | 25231 |
| 桌面上的搜索栏 | 37969115 | 25120 |
| 设置中的动画导航面板图标 | 34878152 | 25197 |
| 现代“打开方式”菜单 | 36302090 | 25151, 22622.290 |

ViVeTool 是一个用于功能操作的开源 CLI 工具。在引擎盖下，它由一个名为 ViVe 的 C#库提供支持。如果您想在 Windows 11 实例上尝试任何新功能，您应该遵循以下步骤:

1.  从其 [GitHub 库](http://github.com/thebookisclosed/ViVe/releases/latest)下载**最新版本的 ViVeTool** 。
2.  **将档案文件**提取到方便的地方。
3.  按下键盘上的 **Windows 键+ X** 并选择**终端(管理)**以启动提升的 shell 窗口。如果您愿意的话，您也可以使用 PowerShellif，或者使用普通的旧命令提示符并提升权限。
4.  将目录更改为**提取的 ViVeTool 目录**。比如你把 ViveTool 提取到 D:\ViveTool，输入`cd D:\ViveTool`。
5.  从上表中找到与您要启用的功能相对应的功能 ID。然后，执行命令:`vivetool /enable /id:xxx`
6.  如果一切正常，您应该在控制台中看到“成功设置特性配置”。
7.  关闭控制台窗口并重新启动计算机，以使更改生效。

如果您改变主意，想要恢复更改，重复上述步骤，将第 5 步命令中的`/enable`替换为`/disable`。

说到 Windows 功能控制 API，ViVeTool 简直就是“瑞士军刀”。除了切换 WIndows 功能的状态之外，它还可以查询底层 Windows 版本的现有功能配置，导入/导出/重置自定义配置，甚至帮助识别最后一次已知的良好回滚系统状态。

要了解更多信息，请打开终端窗口，不带任何参数地运行 ViveTool 可执行文件。该应用程序将列出所有的命令及其用法。这包括启用或禁用功能，以及列出现有的功能配置。

* * *

你对 Windows 11 中新的 UI/UX 增强功能满意吗，或者你打算降级到以前的版本？请在评论中告诉我们你的想法。