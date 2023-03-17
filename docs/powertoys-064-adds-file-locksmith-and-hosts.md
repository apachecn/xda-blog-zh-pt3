# PowerToys 0.64 增加了文件锁匠和主机文件编辑器工具

> 原文：<https://www.xda-developers.com/powertoys-064-adds-file-locksmith-and-hosts/>

微软 PowerToys 工具套件的粉丝们今天有了一些好消息，因为该公司现在推出了该应用程序的 0.64 版本。最新的版本增加了几个主要的附件，文件锁匠和主机文件编辑器。

文件锁匠可能是两者中更有趣的一个，而且真的，它对任何人都有用。你可能遇到过这样的情况:你试图删除一个文件，但 Windows 向你显示一个错误，声称该文件不能被删除，因为它正被另一个应用程序使用。有了 File Locksmith，你就可以找出那个应用是什么了。这样，你可以很容易地终止进程，这样你就可以删除文件，所以这对很多人来说肯定是一个很大的帮助。

另一个补充是有点不言自明的。借助 Hosts 文件编辑器工具，您可以使用适当的编辑器 UI 在 [Windows 11](https://www.xda-developers.com/windows-11/) (或 10)中编辑 Hosts 文件，而不必使用记事本。例如，Hosts 文件允许您阻止某些域被访问，有了这个 UI，对它进行更改应该不会那么令人生畏。

然而，除了这两个新工具之外，这次更新还有一些好消息。PowerToys 设置现在包括一个新功能，允许您从文件中导出或导入当前设置，因此您可以根据需要更轻松地在设备之间迁移您的设置。

此外，微软还对 FancyZones 进行了改进，以便您可以设置水平和垂直屏幕的默认行为。这是因为，在某些情况下，显示器 id 可以重置，FancyZones 设置不再适用。有了这个修正，即使发生这种情况，你的布局仍然应该让*基于屏幕方向有一些*的感觉。

PowerToys 版本中有很多较小的修复和改进，所以如果你想要完整的列表，可以在下面查看。

**永远在顶端**

*   如果一个窗口不再在顶部，检测并把它放在顶部。

**颜色选择器**

**FancyZones**

*   增加了用户配置水平和垂直屏幕默认布局的方式。
*   用滑块替换了 FancyZones 编辑器中的剩余数字框，以提高屏幕阅读器的可访问性。
*   修正了一个打破窗口切换快捷键的问题。

**文件钳工**

*   增加了一个新的工具:文件锁匠。
*   感谢 [@niels9001](https://github.com/niels9001) 在 UI 上的设计！

**组策略对象**

*   强制禁用和启用 PowerToys 工具的组策略对象设置。
*   感谢 [@htcfreek](https://github.com/htcfreek) 帮助审查以确保发货的设置符合系统管理员的期望！

**主机文件编辑器**

*   增加了一个新的工具:主机文件编辑器。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   感谢 [@niels9001](https://github.com/niels9001) 对 UI 的设计帮助！
*   感谢 [@davidegiacometti](https://github.com/davidegiacometti) 修复发现的 bug 并在发布前增加功能！
*   感谢 [@AtariDreams](https://github.com/AtariDreams) 与项目的其他部分相比，合并了这些包！
*   感谢 [@htcfreek](https://github.com/htcfreek) 为条目编辑器添加了一个 scrollviewer！

**键盘管理器**

*   修正了一个没有被正确取消的延迟。感谢 [@AtariDreams](https://github.com/AtariDreams) ！

**鼠标实用程序**

**电动玩具运行**

*   更改图像加载以释放 PowerToys 运行主可执行文件中的图像。这是为了修复 PowerToys 更新后收到的“app.dark.png”缺失问题。
*   修正了默认动作失败后 PowerToys 运行隐藏的问题。感谢 [@hlaueriksson](https://github.com/hlaueriksson) ！
*   修复了 PowerToys 运行允许在上下文菜单动作成功后显示。感谢 [@hlaueriksson](https://github.com/hlaueriksson) ！

**快速口音**

*   将“荷兰语”更正为“德语”。感谢 [@damienleroy](https://github.com/damienleroy) ！
*   添加了葡萄牙语口音。感谢 [@pcanavar](https://github.com/pcanavar) ！
*   修正了工具栏在缩放桌面上的位置。

**屏幕尺**

*   改进了菜单中使用的丙烯笔刷。感谢 [@niels9001](https://github.com/niels9001) ！

**设置**

*   添加了将设置备份到文件或从文件恢复设置的功能。感谢 [@jefflord](https://github.com/jefflord) ！
*   修正了当窗口重新打开时，OOBE 显示的快捷方式不更新为新值的问题。
*   修复了备份/恢复功能中“文档”文件夹的用法。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！

**文本提取器**

*   添加了关于如何安装 OCR 识别语言的警告。
*   修正了第一次激活后覆盖不聚焦的问题。
*   增加了 CJK 语和非 CKJ 语单词之间的空格。感谢 [@maggch97](https://github.com/maggch97) ！

**视频会议静音**

*   添加了静音时隐藏视频会议静音覆盖的设置。感谢 [@akabhirav](https://github.com/akabhirav) ！
*   增加了一个关于以后不赞成视频会议静音的警告(v0.67)，详情请查看 [#21473](https://github.com/microsoft/PowerToys/issues/21473) 。

**安装者**

*   添加了一些丢失的文件，这些文件会导致设置和 PowerRename 在某些配置上无法正常工作。
*   更新了。净依赖于 6.0.10。

**开发**

*   整合了 nuget 包并删除了一些未使用的包。
*   更新了窗户。CppRT 到最新版本。感谢 [@AtariDreams](https://github.com/AtariDreams) ！
*   删除了不再使用的 cxxopts 依赖项。感谢 [@AtariDreams](https://github.com/AtariDreams) ！
*   将 cziplob 依赖项更新为 0.25。感谢 [@AtariDreams](https://github.com/AtariDreams) ！
*   更新了系统。IO .抽象依赖。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   打开 C++代码分析并增量修复警告。
*   在 GitHub 上的问题模板中添加了安装方法，因为有些问题似乎与特定的安装方法有关。
*   在发布配置项中自动创建安装程序哈希。
*   ImageResizer 上`.First()`的简化使用。感谢 [@AtariDreams](https://github.com/AtariDreams) ！
*   改进并澄清了问题模板。感谢 [@Jay-o-Way](https://github.com/Jay-o-Way) ！
*   修复了一个 PTRun 单元测试，使其与更加兼容。NET 6。感谢 [@AtariDreams](https://github.com/AtariDreams) ！

此版本中也有一些已知问题，包括文本提取器有时无法识别基于 Arm64 的设备上的文本，或者在非常特殊的情况下，一些用户无法打开 PowerToys 设置，这是因为与其他应用程序冲突。微软还警告说，安装 PowerToys 后，在重启电脑之前，PowerRename 和 Image Resizer 的上下文菜单条目可能不会显示。

如果这些问题对你来说不重要，你可以从 GitHub 下载 PowerToys 版本[。如果你已经安装了 PowerToys，你可以在应用程序的设置中检查更新，或者它最终会通知你更新。](https://github.com/microsoft/PowerToys/releases/tag/v0.64.0)