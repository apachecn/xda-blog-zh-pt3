# PowerToys 0.59 可以在基于 ARM64 的 Windows 电脑上运行

> 原文：<https://www.xda-developers.com/powertoys-0-59-native-arm-support/>

# 微软 PowerToys 套件采用最新更新的原生 ARM

微软发布了 PowerToys 软件套件的重大更新，为 ARM 处理器提供了本机支持。继续阅读，了解更多信息！

微软发布了 PowerToys 软件套件的新稳定版本。0.59 版本标志着 PowerToys 的第一个官方版本，设计为在 ARM 计算机上运行。PowerToys 软件包的每个模块，包括安装程序，都针对 ARM64 架构进行了重新编译，在使用更少内存的同时，带来了更好的性能和更高的效率。

值得注意的是，微软在 0.58 发布周期中开始为 ARM 打基础[。然而，PowerToys 的前一版本没有提供编译后的 ARM64 二进制文件。因此，](https://www.xda-developers.com/powertoys-0-58-preps-arm64-version/) [ARM 设备](https://www.xda-developers.com/best-windows-on-arm/)上的性能不如原生 ARM64 应用。现在，PowerToys 的原生 ARM 版本可以通过稳定的渠道获得，与通过仿真运行的旧版本相比，它将显著改善 Surface Pro X 等设备的整体用户体验。

还有另一个值得注意的增加，那就是在键盘管理器中支持多达 4 个快捷键。该团队还完成了 Power Rename 向 WinUI 3 的过渡。

除此之外，0.59 版本还对 PowerToys 中包含的大量应用程序进行了修复、调整和其他改进。你可以在下面看到完整的变更日志:

### PowerToys 0.59 的新功能

**通用**

**ARM64**

*   现在完全增加了 ARM64 支持！
*   修复了在 ARM64 上工作的 PowerRename。
*   修复了在 ARM64 上工作的文件浏览器工具。
*   对安装程序项目进行了更改，以构建 ARM64 安装程序。
*   为 ARM64 配置 CI 和发布管道。
*   在自述文件中添加了 ARM64 版本状态。

**永远在顶端**

*   修正了 Win+D 最小化窗口时边框粘滞的问题。

**FancyZones**

*   修正了一个在设置默认布局时消耗 CPU 周期的错误。
*   修复了由于虚拟桌面 ID 更改而导致应用程序无法在最近已知的区域中打开的错误。
*   修正了一个程序打开弹出菜单的错误。
*   修正了一个在某些配置下导致窗口不被抓取的错误。

**图像缩放器**

*   不再尝试更改未实际调整大小的文件的元数据。感谢[@亚当儿童](https://github.com/adamchilders)！

**文件浏览器附加组件**

*   修正了依赖 WebView2 的模块只能打开小于 2 MB 的文件的错误。现在，产生的 html 在呈现之前被生成到一个临时文件中。
*   为没有 viewBox 属性的 svg 文件添加一个 view box 属性，以便预览尝试显示整个图像。
*   移除渲染 svg 缩略图时显示的滚动条。

**键盘管理器**

*   现在快捷键中最多可以使用四个修饰键。例如，这将允许您使用 Office 键(发送 Win+Ctrl+Shift+Alt)。
*   修正了同时按下两个快捷键映射时锁定键盘管理器的错误。
*   删除了某些遥测事件的垃圾事件。

**电源重命名**

*   移植到使用 WinUI 3 而不是 WinUI 2。

**PowerToys 运行**

*   服务插件能够搜索部分名称、显示名称或服务类型或状态。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   服务插件现在支持启动类型“自动(延迟自动启动)”。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   服务插件现在有大服务名称的工具提示和其他 UI 改进。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   TimeDate 插件在全局查询中给出只包含数字的查询结果。这个问题已经解决了。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   我们在执行查询之前引入了一个节流器，以确保执行输入来提高性能。感谢 [@shandsj](https://github.com/shandsj) ！
*   修正了当系统默认浏览器有一个空模式设置时网络搜索崩溃的问题。
*   修复了 VSCodeWorkspaces 找不到 VSCode 的可移植安装的错误。感谢 [@harvastum](https://github.com/harvastum) ！
*   计算器插件对无效输入和内部错误反应更好。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   计算器插件现在可以配置为使用美国数字格式，而不是系统格式。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   文件夹插件支持包含“/”的路径。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！

**设置**

*   现在，当模块被禁用时，用于为 FindMyMouse 添加排除的应用程序的 UI 也被禁用。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   文件浏览器的设置界面中的文本得到了改进。感谢 [@Jay-o-Way](https://github.com/Jay-o-Way) ！
*   如果机器中的一切都以提升的方式运行，设置将不会尝试启动，而是显示一条警告消息。
*   一些小的 UI 修复。感谢 [@niels9001](https://github.com/niels9001) ！
*   如果首先打开 OOBE 屏幕，设置屏幕现在应该正确打开。
*   FancyZones 的圆角设置现在只在 Windows 11 上显示。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   修正了当使用干净的设置进入键盘管理器页面时界面冻结的问题。
*   修正了当使用搜索功能时，显示所有 PowerToys 运行插件被禁用的信息。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   将 Windows App SDK 运行时升级到 1.1.0，修复了 UAC 关闭时设置无法启动的问题，并提高了性能。

**跑步者**

*   自动更新会考虑它是否在 x64 或 arm64 上运行，以下载正确的安装程序。

**安装工**

*   更新了。净依赖于 6.0.5。
*   安装程序现在是使用 Wix 3.14 的 beta 版构建的，支持 arm64。
*   根据需要添加了 VC++可再发行二进制文件。
*   PowerToys 随附了 Windows App SDK 运行时二进制文件，而不是运行其安装程序。这应该可以修复 0.58 的大部分安装问题。

**发展**

*   GitHub 增加了向 PowerToys 发布 winget 包的新动作。
*   GitHub 增加了新的动作，可以发布到微软商店。感谢 [azchohfi](https://github.com/azchohfi) ！
*   安装 Windows App SDK 依赖项和构建安装程序的文档已更新。
*   FxCop 已从 PowerToys Run TimeZone 插件中移除，并被 NetAnalyzers 所取代。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！

### PowerToys 0.59 中的已知问题

**已知问题**

*   有用户报告称[无法打开设置窗口](https://github.com/microsoft/PowerToys/issues/18015)。这是由于与一些应用程序不兼容造成的(RTSS RivaTuner 统计服务器和 MSI AfterBurner 就是已知的例子)。如果您受此影响，请检查链接的问题，以验证所提供的任何解决方案是否适合您。

如果你还没有，你可以从 GitHub 仓库下载最新版本的 PowerToys，或者在微软商店搜索。如果您已经安装了 PowerToys，系统会提示您自动下载 0.59 版。

**下载 PowerToys:[GitHub](https://github.com/microsoft/PowerToys/releases/latest)| |[微软商店](https://apps.microsoft.com/store/detail/XP89DCGQ3K6VLD)**

* * *

**来源:** [PowerToys Github](https://github.com/microsoft/PowerToys/releases/tag/v0.59.0)