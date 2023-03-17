# Windows App SDK 1.1 增加了对高级应用和云母材料的支持

> 原文：<https://www.xda-developers.com/windows-app-sdk-1-1-elevated-apps-mica/>

微软发布了 Windows App SDK 的 1.1 版本，这是一套开发工具，可以让你为 Windows 10 和 11 开发应用。Windows 应用 SDK 的最初版本是在 [Windows 11](https://www.xda-developers.com/windows-11/) 推出后不久发布的，它是一种将现代视觉和功能以及传统 Win32 功能整合在同一应用中的方式。这个新版本带来了一些显著的改进，使体验更好。

云母是微软在 Windows 11 中推出的一种新的表面材料，它允许你的桌面背景通过应用程序柔和地发光，为用户界面增添一点色彩。虽然 Windows 应用 SDK 的最初版本是在 Windows 11 已经推出之后发布的，但你不能以这种方式构建使用新云母材料的应用。与此同时，Windows 应用程序 SDK 中的 WinUI 3 gallery 具有新的示例、新的控件和刷新的界面，以更加符合 Windows 11 的设计原则。

另一个主要改进是能够制作需要提升权限的应用程序(意味着它们需要以管理员身份运行)，这是最初版本的一个限制。此外，使用 MSIX 格式打包的应用程序、稀疏打包的应用程序和未打包的应用程序现在也可以发送 Windows toast 通知，包括在应用程序未运行时。这意味着即使应用程序没有被使用，它也有办法提醒用户。

由于 WinRT 互操作层的更新，微软还对使用 C#的应用程序进行了性能改进。微软表示，一个简单的“Hello World”应用程序的启动时间可以加快 9%，当在 WinUI 3 应用程序中使用依赖属性时，你也应该会看到很大的改进。

在开发者方面，现在可以设置一个应用程序在由于更新或崩溃而关闭时自动重启。此外，您可以设置恢复选项，以便应用程序可以将用户带回到应用程序意外关闭之前的状态。

其他变化包括改进的引导程序 API、对自包含应用程序的支持(即，包含使用它们所需的 Windows 应用程序 SDK 依赖项的应用程序)，以及无需直接使用注册表 API 即可更改环境变量的能力。微软还推出了一种新的窗口 API，可以设置应用程序窗口的 z 顺序。最后，微软宣布 WinUI 模板工作室(C#)现在可以在 Visual Studio 市场中[使用。这个扩展使得使用基于向导的体验创建 WinUI 应用程序变得更加容易，产生“格式良好、可读的代码”，这是开始 WinUI 开发的好方法。](https://marketplace.visualstudio.com/items?itemName=TemplateStudio.TemplateStudioForWinUICs)

要安装 Windows App SDK 开发工具，您需要使用 Visual Studio 2022 或 2019，并且[根据您想要构建的应用类型，遵循本页](https://docs.microsoft.com/en-us/windows/apps/windows-app-sdk/set-up-your-development-environment?tabs=vs-2022-17-1-a%2Cvs-2022-17-1-b)上的说明。通过这种方式，您应该可以自动获得最新版本的工具。您也可以在这里找到完整的发行说明。

* * *

来源:[微软](https://blogs.windows.com/windowsdeveloper/2022/06/03/whats-new-in-windows-app-sdk-1-1/)