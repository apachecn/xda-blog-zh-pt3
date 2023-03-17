# 开发者现在可以开始制作和测试第三方 Windows 11 小工具了

> 原文：<https://www.xda-developers.com/windows-app-sdk-1-2-make-test-windows-11-widgets/>

我们离在 [Windows 11](https://www.xda-developers.com/windows-11/) 上提供第三方小工具又近了一步。微软今天发布了 Windows 应用 SDK 的 1.2 版本，这是第一个支持在 Windows 11 上为 widgets board 创建应用 Widgets 的版本。

第三方插件是微软在去年发布 Windows 11 时承诺的，但它花了很长时间才成为现实。目前，为了测试这些小工具，你需要是运行 [build 25217](https://www.xda-developers.com/windows-11-25217-dev-channel-third-party-widgets/) 或更高版本的 Windows Insider。事实上，虽然开发人员现在可以创建这些小部件，但它们仍然只能在内部机器上进行本地测试。你不能将一个带有插件的应用程序发布到微软商店让其他人试用，尽管这应该很快就会实现。微软特别提到你可以为“打包的 Win32 应用程序”创建窗口小部件，所以不是每个应用程序都支持窗口小部件，至少现在是这样。

考虑到所有现有的部件都是基于微软的网络内容，第三方部件即将发布的前景是非常乐观的。

然而，这并不是 Windows App SDK 这一版本的全部新功能。微软还增加了对动态刷新率显示器设备的支持，这意味着应用程序现在可以利用 Surface Laptop Studio 或 Surface Pro 9 等设备上的动态调整刷新率。反过来，这意味着您的应用现在可以在需要时使用更高的刷新率，并切换回更低的刷新率以节省电能。默认情况下，应用程序将使用更高的刷新率进行滚动和其他交互，而不需要对应用程序进行任何更改，只要用户拥有 [Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2/) 。

该版本的其他改进包括新的媒体播放控件，具有针对 Windows 11 的更新设计，以及使用 Azure 通信服务在应用程序中内置语音和视频通话的能力。还通过新的 DisplayInformation 类支持 HDR 和自动颜色管理，这是一个新的 AppNotificationBuilder，用于测试应用程序的通知，并支持修剪。网络应用。

如果你是一名开发人员，你可以从 Windows 应用软件开发工具包开始，你需要有 Visual Studio 2019 或 2022，你可以在这里[下载所需的工具](https://learn.microsoft.com/en-us/windows/apps/windows-app-sdk/)。

* * *

**来源:** [微软](https://blogs.windows.com/windowsdeveloper/2022/11/16/whats-new-in-windows-app-sdk-1-2/)