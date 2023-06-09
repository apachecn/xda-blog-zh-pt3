# Windows 11 build 25206 为外部显示器带来动态刷新率

> 原文：<https://www.xda-developers.com/windows-11-build-25206-dev-channel/>

紧随昨天向公众发布的 [Windows 11 2022 更新](https://www.xda-developers.com/windows-11-22h2/)之后，开发频道的 Windows 内部人士今天将获得他们每周的 Windows 11 版本。微软正在开发频道推出 Windows 11 build 25206，它带来了一些显著的改进，包括在外部显示器上使用动态刷新率(DDR)的能力。

事实上，你可能还记得微软在 Surface Pro 8 和 Surface Laptop Studio 旁边首次宣布支持 Windows 中的动态刷新率，这是首批支持动态刷新率的设备。但是，它仅适用于笔记本电脑上的内置显示器，其他支持的笔记本电脑也有同样的限制。然而，使用这种版本，只要您有支持 WDDM 3.1 的驱动程序和刷新率为 120Hz 或更高的显示器，您就可以利用动态刷新率来节能。

此版本还对 SMB 身份验证速率限制器进行了更改，这是一项限制 SMB 服务器错误身份验证尝试次数的功能。例如，如果一个强力攻击试图在 5 分钟内每秒提交 300 次身份验证尝试，它将在这段时间内提交 90，000 个密码，但使用这个限制，相同的过程需要 50 多个小时。这项功能已经可用，但现在它默认启用，并设置为每次失败的身份验证尝试延迟 2 秒，这使得 WIndows 机器不太容易成为这种暴力攻击的目标。

这个版本中的其他变化包括具有现代化设计的“打开方式”对话框的完全可用性。此外，当在文件浏览器主页中执行搜索时，您现在可以看到云中文件的最近文件活动。最后，微软开始推出一项改变，允许你在密码字段中使用剪贴板历史。

除了这些新增内容，还有一个典型的缺陷修复列表，尽管这次相对来说比较短。您可以在下面查看:

### Windows 11 内部版本 25206 中的已知问题

**【通用】**

*   OneDrive 安装程序不应再在每次电脑重新启动时意外请求设置权限。
*   修正了影响一些内部人士的高击球 explorer.exe。

**【设置】**

*   修复了在搜索和选择某些与讲述人相关的设置时可能发生的设置崩溃。

**【搜索】**

*   修正了一个高命中率的搜索崩溃，这个崩溃在过去的几个航班中影响了一些内部人员。

**【其他】**

*   如果您将 Windows 沙盒窗口靠到屏幕的一侧，它现在应该可以正确调整大小。
*   修复了一个问题，该问题可能会导致在某些崩溃后 Windows 错误报告中出现内存泄漏。
*   如果焦点在桌面上，那么按 ALT + F4 和 Enter 键应该会关闭你的电脑，而不是必须先移动键盘焦点(就像在最后几次飞行中需要的那样)。
*   计算机图标现在再次显示在关闭窗口对话框中。

同样典型的是已知问题列表，这是任何预发布软件都可能遇到的问题。这包括最近添加的平板电脑优化任务栏的一些问题，它仍然有一些问题需要解决。以下是完整列表:

### Windows 11 内部版本 25206 中的已知问题

**【常规】**

*   **【新】**我们正在调查一个问题，即“日期、时间和时区设置不正确”消息显示不正确，并阻止安装继续进行。
*   我们正在调查一些内部人员在升级到最新航班后音频停止工作的报道。
*   我们正在调查一些不同的应用程序在最近的版本中开始崩溃的报告。

**【文件浏览器】**

*   我们正在解决一个问题，即命令栏项目，如复制、粘贴和清空回收站，可能会意外地在应该启用时未启用。

**【设置】**

*   我们正在调查使用“设置”>“应用”>“已安装的应用”卸载某些应用时无法正常工作的一些问题。

**【平板电脑优化任务栏】**

*   在桌面姿势和平板电脑姿势之间转换时，任务栏有时会闪烁。
*   在桌面姿势和平板电脑姿势之间切换时，任务栏转换到触摸优化版本所需的时间比预期的长。
*   使用左边缘或右边缘手势会导致窗口小部件或通知中心(分别)与任务栏重叠或看起来被任务栏截断。
*   当使用右下角手势查看快速设置时，任务栏有时会停留在展开状态，而不是消失在折叠状态。
*   当桌面上没有正在运行的窗口时，任务栏有时会折叠，而此时它应该是展开的。

**【微件】**

*   在像阿拉伯语这样的从右向左显示的语言中，当点击窗口小部件板的扩展视图时，在窗口小部件板调整大小之前，内容在视图之外动画显示。
*   任务栏上的通知徽章编号可能会出现错位。

很难说这些变化何时会对公众开放，特别是现在[微软已经表示计划在全年发布较小的功能更新](https://www.xda-developers.com/microsoft-windows-11-update-cadence-denies-windows-12/)，而不是像本周早些时候发布的那样将新功能集中在年度更新中。他们可能会在明年左右的任何时候出现。

* * *

**来源:** [微软](https://blogs.windows.com/windows-insider/2022/09/21/announcing-windows-11-insider-preview-build-25206/)