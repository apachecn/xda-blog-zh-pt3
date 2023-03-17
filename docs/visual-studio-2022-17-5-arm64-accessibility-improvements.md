# Visual Studio 2022 17.5 改进了对 Arm64 的支持，并添加了辅助功能检查器

> 原文：<https://www.xda-developers.com/visual-studio-2022-17-5-arm64-accessibility-improvements/>

微软发布了 Visual Studio 2022 的重大更新，将 IDE 带到了 17.5 版本。此更新改进了体验的多个方面，包括新的辅助功能检查器功能和对 Arm64 设备的改进支持。

事实上，可访问性检查器是这个版本的众多亮点之一。这是一个可以检测基于 XAML 的桌面应用程序中潜在的可访问性问题的工具，它支持 WPF、WinForms、WinUI 和 MAUI，所以你可以在很多项目中使用它。Visual Studio 不仅会强调这些问题，还会解释如何修复它们。关于建议的话题，Visual Studio 2022 17.5 现在也支持人工智能支持的“基于意图的”建议，这意味着它可以根据你在项目的其他部分所做的其他编辑，自动建议对你的代码进行编辑。

另一个值得注意的改进是针对 LLVM 的本机 Clang Arm64 工具集，它支持 Arm64 设备上的本机编译，从而提高了性能。这是继版本 17.4 的[原生 Arm64 支持正式亮相之后。关于性能改进的话题，微软也说你可以期待更快的构建时间。NET 应用程序，这样就只构建收到更新的项目，而跳过未更改的项目。此外，微软改进了调试器的性能，特别是线程窗口的响应时间，微软表示现在应该快两倍。](https://www.xda-developers.com/visual-studio-17-4-native-windows-arm/)

还有很多全面的改进，一些与 Azure、Blazor 等相关。一些生活质量的改进还包括一个新的更新设置，它允许您在关闭 Visual Studio 时自动更新它，以便在您不使用它时立即安装更新。另外，微软还通过 Windows 包管理器(winget)提供了 Visual Studio，所以你现在可以通过这种方式安装它。

在 macOS 上，有一些其他的改进，从状态栏中的一个新的 Git 分支选择器开始，这样你就可以很容易地看到你正在做的品牌，并打开你的 Git 更改窗口。还有一个新的热退出功能，即使您有未保存的更改，也可以让您立即关闭 Visual Studio。当您关闭 Visual Studio 时，您对项目所做的所有更改现在都存储为未保存的更改，因此您不必处理确认提示。

随着 Visual Studio 新版本的发布，微软也宣布并发布了。NET 8，以及 ASP.NET 核心和 EF 核心的匹配更新。新版本包括对原生 AOT 功能的改进支持，允许减少内存占用和加快应用程序的启动时间。还包括许多其他改进，其中一些专门针对 Arm64 设备。

你可以在这里下载 [Visual Studio for Windows](https://visualstudio.microsoft.com/downloads/) ，而 [Visual Studio for Mac 可以在这里](https://visualstudio.microsoft.com/vs/mac/)下载。如果你想试试最新的。NET 预览版，可以[下载。网 8 这里](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)。

* * *

**来源:微软** ( [1](https://devblogs.microsoft.com/visualstudio/visual-studio-2022-17-5-released) 、 [2](https://devblogs.microsoft.com/visualstudio/visual-studio-for-mac-17-5-is-now-available/) 、 [3](https://devblogs.microsoft.com/dotnet/announcing-dotnet-8-preview-1/) )