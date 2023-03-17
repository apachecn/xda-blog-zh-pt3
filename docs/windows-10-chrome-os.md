# 如何在 Chromebook 上运行 Windows 10

> 原文：<https://www.xda-developers.com/windows-10-chrome-os/>

如果你最近从 Windows 10 PC 转向 Chromebook，你可能会错过一些你最喜欢的应用程序。一些 Windows 应用无法在 Chrome OS 上原生运行，这已经不是什么秘密了。用户在进行切换时，经常会错过他们最喜欢的生产力应用程序、创作工具和游戏。幸运的是，如果你需要在 Chromebook 上运行 Windows 10，还有一些选项。

最有效的方法之一就是安装[Parallels Desktop for Chrome OS](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU3295/https://www.parallels.com/products/desktop/chrome/)。请注意，尽管该软件目前面向企业用户，因此个人许可证尚不可用。如果你是目标受众的一部分，这可能是你的 Chrome OS 工作流程的一个惊人的补充。

## 什么是 Parallels Desktop for Chrome OS？

[Parallels Desktop](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU3295/https://www.parallels.com/products/desktop/chrome/?utm_source=google&utm_medium=cpc&creative=474284210573&keyword=parallels+desktop+chrome&matchtype=e&network=g&device=c&gclid=Cj0KCQjw5auGBhDEARIsAFyNm9Gj-6BHVMW13Co32nbONHgpMYwfmCwskWBthIjP60S22K0P89GygCAaAiIDEALw_wcB) 是一个全功能的 Windows 容器，原生运行在 Chrome OS 上。这个软件允许你运行完整版的 Windows，但是有一些重要的事情需要注意。

Parallels Desktop 软件目前仅面向企业客户，因此目前个人用户很少使用该选项。借助 Parallels Desktop for Chrome OS，IT 部门可以在线或离线在 Chrome OS 设备上启用专有的全功能 Windows 应用程序-包括原生 Microsoft Office。您需要升级 Chrome Enterprise 才能运行 Parallels(见上面的截图)。

Parallels Desktop for Chrome OS 的主要功能包括:

### 对关键业务 Windows 应用的不间断访问

*   在 Chrome 操作系统和 Windows 之间轻松切换，无需重启。
*   暂停和恢复 Windows 以立即恢复运行。
*   使用 Windows 应用程序在 Chrome OS 上打开文件。
*   额外奖励:使用附带的 Parallels Toolbox 访问 30 多个一键工具。

### 随时随地准备就绪的工作

*   利用桌面应用程序的全部功能，包括 Word、Excel、PowerPoint 等。
*   从 Chrome OS 文件访问 Windows 桌面、文档、下载和自定义文件夹。
*   没有网络？没问题！无论在线还是离线，文件和应用程序都是完全可访问的。

### 完全集成 Chrome 操作系统，带来熟悉友好的体验

*   通过共享剪贴板在 Chrome 操作系统和 Windows 之间轻松移动内容。
*   从 Windows 打印到支持的打印机。
*   借助无缝鼠标、摄像头、麦克风、音频和坞站以及 USB 智能卡读卡器支持，与时俱进。
*   享受动态分辨率和全屏支持带来的视觉享受。

## 运行 Parallels Desktop 的要求

在 Chromebook 上运行 Parallels 有最低系统要求。您至少需要 Chrome OS 版本 85 或更高版本。此外，如果您希望分发到组织中的多台机器，您需要 Google 管理控制台、Chrome 企业升级/Chrome 教育升级、Microsoft Windows ISO、Windows 许可证和存储服务器。在硬件方面，支持的处理器包括英特尔酷睿 i5 或 i7 以及 AMD 锐龙 5 或 7。您的设备上还需要至少 8 GB 的 RAM 和 128 GB 的 SSD 本地存储。

虽然这些规范中的一些似乎是限制性的，但请记住，该软件目前是针对企业客户的。有很多宏碁、惠普、联想的企业级 Chromebooks 符合要求。如果你的 Chromebook 或 Chrome OS 平板电脑满足最低要求，你可能也会喜欢购买一个 T2 坞站，将你的 Chromebook 变成一个完整的工作站。

从技术上来说，如果你是个人，你可以在支持的 Chromebook 上升级到 Chrome Enterprise。你需要做的就是从 Squarespace 这样的提供商那里购买一个网站域名，然后将它链接到一个 Google Workspace 账户。Google Workspace、Chrome Enterprise 和你的域名都有相关的成本，所以如果你没有真正的业务，这可能是一个非常昂贵的方法。

## 安装 Parallels Desktop for Chrome OS

开始之前，Parallels Desktop for Chrome OS 的安装过程需要一些关键的东西。

*   您需要确保您是 Google Workspace 帐户的超级管理员，该帐户与您计划安装的域相关联。
*   在开始之前，请确保您还拥有 Windows 10 ISO、Chrome Enterprise Upgrade 有效的 Windows 10 许可证以及 Parallels Desktop for Chrome OS 许可证密钥。
*   你需要首先在你的管理员 Chromebook 上安装一份 Windows，然后你可以创建一个 zip 文件上传到公司服务器或 Google Drive，供其他人安装在受管设备上。

在用户可以登录到贵组织的 Chromebook 之前，该设备必须注册到管理中。这也适用于管理员的 Chromebook，它将用于创建 Parallels Desktop Windows 映像。

接下来，您需要激活您的 Parallels Desktop 许可证。这可以通过访问您购买许可证时 Parallels 支持提供的链接来完成。点击链接后，您将访问您的 Google 管理控制台为您的组织启用 Parallels Desktop。确保您选中允许用户访问 Parallels Desktop 的选项，否则您将无法继续安装 Windows 10。

最后，您可以在管理机器上运行 Windows 虚拟机，但是首先您需要创建它。为此，在 Chrome 浏览器中按下 *Ctrl+Alt+t* 访问 crosh (Chrome 开发者外壳)终端。在 crosh 终端中运行命令:

**VMC create-p PVM default<windows . iso>**

这里的<windows.iso>应该替换为 Chromebook 下载文件夹中存储的 Windows 映像文件的名称。这个过程需要几分钟来完成，最后会将您的虚拟机命名为 PvmDefault。然后，您可以通过执行以下命令来运行虚拟机:</windows.iso>

**vmc 启动 PVM 默认**

这将打开 Windows 10 安装菜单，您可以照常安装 Windows。请记住，您需要有效的 Windows 许可证来完成此过程。请确保您也安装了 Parallels Tools 以充分利用所有功能。

在虚拟机上安装 Windows 10 后，您需要将图像导出为 zip 文件，以便其他用户(包括您自己)从 Chrome OS 启动器运行 Parallels Desktop。为此，请运行以下命令:

**vmc 导出-d PVM 默认窗口 s10.zip**

您可以用任何您想要的文件名来替换“Windows10.zip”。这个过程需要相当长的时间来完成，压缩文件将会非常大。在这个过程的最后，你必须上传文件到公司服务器或谷歌驱动器，然后输入相关的网址和 SHA-256 散列到谷歌管理控制台。

在此之后，您应该能够点击 Chrome 启动器中的 Parallels Desktop 图标并启动安装程序来下载并在您的机器上安装 zip 文件。从这一点来看，Windows 10 应该会自然打开，你可以开始了。贵组织的其他用户可以重复此过程，在其 Chrome 设备上使用 Windows 10。

## 解决纷争

在 Chromebook 上通过 Parallels 安装 Windows 10 时，我遇到了几个关键问题。第一个问题似乎是 Chrome OS 集成问题。当我第一次尝试在我的管理员设备上创建 Windows 虚拟机时，我收到了一个错误，即安装无法完成，需要 Chrome OS 更新。我检查了更新，但在稳定的 Chrome OS 频道上没有适用于我的设备的更新。

为了看看我是否可以强制更新，我将我的设备切换到 Chrome OS Beta 频道。这对我很有效，我能够更新。回到 crosh 命令行，我就可以运行 create 命令并生成一个 Windows 10 虚拟机了。从那里开始，管理员端的安装过程相对顺利。请记住，为了切换到测试频道，你需要在谷歌管理控制台允许这一点。即使是管理员也需要手动启用此权限才能移动到备用更新通道。

在我的管理员 Chromebook 上创建了虚拟机并安装了并行工具后，我还注意到我的 Windows 文件系统没有与 Chrome OS 共享。这并不理想，因为你不能在 Windows 和 Chrome 操作系统之间移动文件，这是 Parallels 宣传的一个关键功能。这实际上是正常的行为，只是在文档中没有明确说明您需要一个额外的步骤来为管理员启用它。

管理员需要从公司服务器或 Google Drive 下载 Windows zip 文件，以便在自己的机器上完整安装 Parallels。如果不这样做，您将无法共享文件。要在管理员笔记本电脑上安装 Parallels，只需点击 Chrome OS 启动器中的 Parallels 图标，下载就会自动开始。现在，你可以在 Windows 和 Chrome 操作系统之间完全共享了。

## 哪些 Windows 应用可以通过 Parallels 在 Chromebook 上运行？

使用 Parallels Desktop for Chrome OS，您可以运行大多数流行的 Windows 应用程序。也许您想运行 Microsoft Office 的完整 Windows 版本？这是 Parallels Desktop for Chrome OS 最引人注目的使用案例之一。在 Chrome OS 设备上安装完整版本的 Windows，您可以轻松下载并运行每个 Office 应用程序的完整桌面版本。

这种方法有一些主要优点。最重要的是，您保留了微软应用程序的所有功能。一些专业功能，如 Excel 中的数据分析工具库，在 web 应用程序和 Android 应用程序中缺失。在 Chromebook 上运行 Parallels 可以使用桌面应用程序中的所有功能。

大多数 PC 游戏使用 Parallels 也应该运行良好，但请记住游戏质量将取决于您的 Chromebook 的规格。好消息是 Parallels 需要相当大的规格来安装，所以你应该也能玩一些游戏。

然而，并非所有的功能都与真正的 Windows 机器完全一样。例如，你可以使用 Parallels 更流畅地运行 iTunes 的 Windows 版本。但是，您将无法同步 iPhone 或 iPod。这是一个需要记住的重要警告。尽管你可以用 Parallels 在 Chromebook 上运行 Windows，但该设备并不总是像 PC 一样运行。

## 结论

事实证明，你确实可以在任何一款[顶级 Chromebooks、](https://www.xda-developers.com/best-chromebooks/)上运行 Windows 10，前提是你是企业或教育客户，或者愿意支付谷歌 Workspace 和企业升级的费用，并连接到你个人拥有的网站域名。如果你愿意购买[Parallels Desktop for Chrome OS](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU3295/https://www.parallels.com/products/desktop/chrome/)，你的 Chromebook 将拥有 Windows 的全部功能。对于那些想开始尝试 Parallels 的人，点击下面框中的链接。如果您在 Chromebook 上试用了 Parallels 软件，请在评论区告诉我们效果如何。

**注意:**我们预计 Parallels Desktop for Chrome OS 也将在不久的将来支持 Windows 11。Windows 11 是最近才发布的，所以在本文发布时还没有官方支持的详细信息。当 Windows 11 支持 Chromebooks 时，我们将更新本文或创建新的教程。

 <picture>![Parallels Desktop is a full-featured Windows container that runs natively on Chrome OS. This software allows you to run the full version of Windows on your Chromebook.](img/f794f234e438998262bd2b838876d1db.png)</picture> 

Parallels Desktop for Chrome OS

##### Parallels Desktop for ChromeOS

Parallels Desktop 是一个全功能的 Windows 容器，在 Chrome OS 上运行。这款软件可以让你在 Chromebook 上运行完整版的 Windows。

 <picture>![Windows 10 is the most popular operating system in the world. Used on PCs from numerous manufacturers. You need a copy of Windows to use Parallels.](img/8763d4d975be29058ac89876d7cbc2c4.png)</picture> 

Windows 10

##### Windows 10 主页

Windows 10 是世界上最流行的操作系统。用于众多制造商的电脑。您需要一份 Windows 才能使用 Parallels。

 <picture>![The most popular productivity suite out there, Office has everything you need for school or work, with Word, Excel, Powerpoint, and OneNote all included. Make sure you have a copy of Office to use with Parallels.](img/a78bff6b9b629e98e0a7a9dd04474c50.png)</picture> 

Microsoft Office

##### 微软办公

Office 是最受欢迎的办公套件，拥有您在学校或工作中所需的一切，包括 Word、Excel、Powerpoint 和 OneNote。请确保您有一个 Office 副本可用于 Parallels。