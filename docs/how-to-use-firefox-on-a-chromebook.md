# 如何在 Chromebook 上安装和使用 Firefox

> 原文：<https://www.xda-developers.com/how-to-use-firefox-on-a-chromebook/>

Chromebooks 可能由谷歌 Chrome 驱动，但这并不意味着你*总是*必须使用 Chrome 网络浏览器。如果你的 Chromebook 或 [ChromeOS 平板](https://www.xda-developers.com/best-chrome-os-tablets/)足够强大，你实际上可以安装其他网络浏览器并扩展你的视野，就像你在 Windows 笔记本电脑上一样。

你可以在 ChromeOS 上使用的网络浏览器之一是 Firefox，它提供了增强跟踪保护等功能。Firefox 的 Linux 版本和 Android 版本都可以在大多数现代 Chromebooks 上使用。这就是为什么我们今天在这里向你解释如何开始在你的 Chromebook 上安装 Firefox。

## 你需要什么

 <picture>![The HP Elite Dragonfly Chromebook is great for businesses that deal with artists or creative types. It has an amazing display and specs](img/ad4f0e6f3a80c3fb18aced1860b89a9a.png)</picture> 

HP Elite Dragonfly Chromebook

*   **Chromebook 兼容谷歌 Play 商店和 Linux 应用:**本指南中的过程需要在 Chromebook 上启用 Linux 或运行 Android。大多数运行 ChromeOS 80 或更高版本的 x86 CPUs(英特尔或 AMD CPUs)的现代 Chromebooks 都可以很好地工作。如果你有联发科或高通的基于 Arm 的 SoC 的 Chromebook，你*不能正式*安装 x86 Linux 版本，而必须使用 Android 应用程序。您可以尝试安装 x86 版本，但它可能不是最好的。
*   **访问互联网**:自然，你需要访问互联网来下载 Firefox 所需的文件。
*   **管理员权限:**如果你的 Chromebook 由你的工作场所或学校管理，你将无法在 Chromebook 上安装 Firefox。你需要管理员权限才能安装 Linux 和 Android 应用程序。

## 选项 1(最简单)从谷歌 Play 商店安装移动版 Firefox

对于大多数人来说，在 Chromebook 上安装 Firefox 最简单的方法就是使用移动 Android 版本的浏览器。这个版本是从谷歌 Play 商店下载的。当然，如果你选择这种方式，你必须习惯火狐应用的移动布局。你的 Chromebook 还需要与 Android 应用程序兼容。大多数 Chromebooks 都能正常工作。

1.  点击 Chromebook 屏幕左下角的**启动器图标**。
2.  搜索 **Play 商店。**
3.  启动 Play Store 应用。
4.  在顶部的**搜索应用&游戏**框中输入术语 **Firefox。**
5.  点击绿色的**安装**按钮。
6.  完成后，Firefox 应该会添加到 ChromeOS 启动器中。
7.  单击屏幕左侧的启动器图标，搜索 **Firefox** ，然后单击启动它。

同样，在首次推出时，ChromeOS 会警告你，Firefox Android 应用程序是为移动设备设计的。它可能无法调整大小或很好地适应 Chromebook 屏幕，并且您可能会遇到网页提供移动版本而不是桌面版本的问题。

如果你想定制你的 Firefox 体验，点击窗口顶部显示 **Tablet** 的地方，选择向下箭头，并选择 **Resizable** 。点击**允许**，然后拖动 Firefox 窗口调整到你的屏幕大小。

## 选项 2(高级用户)安装 Firefox 的 Linux 桌面版本

更高级的 Chromebook 用户可以安装桌面 Linux 版本的 Firefox，获得类似于使用 Chrome 的经典网络浏览器体验。作为先决条件，我们建议查看我们的指南[在 ChromeOS](https://www.xda-developers.com/linux-apps-chrome-os/) 上安装 Linux 应用程序。一旦你熟悉了将要发生的事情，你就可以开始下面的步骤了。请记住，本指南的第一部分是针对采用英特尔或 AMD x86 CPU 的系统。对于基于 Arm 的 SoC 系统，步骤是不同的，您可以跳到这一小节下面的小节。

### 在采用 x86(英特尔/AMD) CPU 的 Chromebook 上安装 Linux 版本的 Firefox

1.  通过单击时间区域并选择设置目录来打开 ChromeOS 设置。
2.  点击**高级**选项卡，选择**开发者。**
3.  在显示 **Linux 开发环境**的地方，选择**打开**选项，并按照屏幕上的设置进行操作。
4.  在 ChromeOS 上打开终端应用程序，方法是单击屏幕左侧的启动器，搜索，然后选择**终端**。
5.  从列表中选择**企鹅**。
6.  键入以下命令，确认您拥有最新的 Linux 版本: **cat /etc/os-release**
7.  如果您看到版本 10 或更高版本，您就可以开始了。如果没有，键入以下脚本进行更新，然后按 enter:**sudo bash/opt/Google/cro-containers/bin/upgrade _ container**
8.  更新后，您必须通过键入以下代码并按下键盘上的 enter 键来启用并安装用于 Linux 的 Flatpak 包格式: **sudo 以安装 flatpak**
9.  按下键盘上的 **Y** 确认，然后点击**回车。允许安装完成。**
10.  键入以下命令:**sudo flat pak remote-add-if-not-exists flat hub https://flathub.org/repo/flathub.flatpakrepo**
11.  键入这个命令并按下键盘上的 enter 键:**sudo flat pak install flat hub org . Mozilla . Firefox**
12.  通过点击键盘上的 **Y** 并按下 **enter 键来接受。**让安装完成。
13.  再次按下 **Y** ，按下**进入**等待 Firefox 安装。
14.  从你的 ChromeOS 启动器启动 Firefox！它将位于 **Linux apps** 文件夹下。

官方上，Mozilla 没有列出在基于 Arm 的 CPU 设备上安装 Firefox 的文档。联想 Chromebook Duet 5 等设备配有联发科 Kompanio 或高通骁龙 7c 或 7c Gen 2 SoC。然而，你仍然可以按照下面的步骤安装 Linux 版本的 Firefox。请注意，您可能会遇到兼容性问题。

1.  按照上面看到的步骤 1-5 在 Chromebook 上启用 Linux。
2.  在终端中键入以下命令: **sudo apt update。**
3.  类型:**须藤 apt 升级。**
4.  点击键盘上的 **Y** 键，然后按**回车。**
5.  键入: **sudo 安装 firefox-esr** 并按**回车。**
6.  点击键盘上的 **Y** 键，然后按**回车。**
7.  从你的 ChromeOS 启动器启动 Firefox！它将位于 **Linux apps** 文件夹下。

这就是在 ChromeOS 上安装桌面版和谷歌 Play 商店版 Firefox 的全部内容。正如你所知，这可能需要很多步骤和耐心，但如果你不想在 Chromebook 上使用 Chrome，火狐是一个不错的选择。登录后，你甚至可以从电脑或手机上输入其他版本 Firefox 的数据。请记住，如果你是微软的粉丝，你甚至可以用同样的方式在 Chromebook 上安装 Linux 版本的新 Edge 浏览器！