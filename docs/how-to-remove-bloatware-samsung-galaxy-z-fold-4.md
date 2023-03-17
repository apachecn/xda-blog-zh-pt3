# 如何从三星 Galaxy Z Fold 4 中删除膨胀软件

> 原文：<https://www.xda-developers.com/how-to-remove-bloatware-samsung-galaxy-z-fold-4/>

许多现代 Android 旗舰手机都配有膨胀软件。这不仅仅是一两家制造商的专利，因为在我们的[最佳安卓手机](https://www.xda-developers.com/best-android-phones/)系列中提到的大多数流行设备都预装了一些你没有要求的应用程序。在你闪亮的 1000 美元新旗舰设备上看到臃肿的软件不是一种愉快的体验，在目前市场上最昂贵的旗舰手机之一 [Galaxy Z Fold 4](https://www.xda-developers.com/samsung-galaxy-z-fold-4-review/) 上也肯定是不可接受的。是的，这款手机自带了很多预装的应用程序。在本文中，我们将向您展示如何从三星 Galaxy Z Fold 4 中删除膨胀软件。

这些预装的应用程序不会妨碍你日常使用手机。然而，它们确实会占用你手机中的空间，占用存储空间，甚至在后台使用系统资源。如果你看不到自己在使用这些应用，最好把它们去掉。这里有几个简单的步骤，使用它们你可以清理你的新 Galaxy Z Fold 4，并删除“无法安装”的臃肿软件。

**注意:**你也可以按照本文提到的步骤清理你的其他安卓智能手机。

## 如何在没有 root 权限的情况下卸载三星 Galaxy Z Fold 4 的膨胀软件

在本教程中，我们将解释如何使用 ADB 和 ADB 应用程序删除 GUI(如“通用 Android 解包器”)从您的手机中删除膨胀软件。使用这些方法最好的一点是，它们不需要手机的 root 访问，这意味着你应该能够没有太多麻烦地做到这一点。

**注意:**卸载对手机正常工作至关重要的系统应用程序可能极其危险，可能会导致故障，甚至是智能手机死机。我们建议您仅删除那些您认为绝对不必要且不会影响设备功能的内容。

### 第一步:在三星 Galaxy Z Fold 4 上启用 USB 调试

*   你需要做的第一件事是打开你的 Galaxy Z Fold 4 上的*设置*应用，并一直向下滚动，找到关于手机的*部分。*
*   现在，寻找*软件信息*选项并选择它以显示您手机的所有软件细节，包括 Android 版本、一个 UI 版本等。
*   在该页面中查找*构建号*选项，并点击几次以启用*开发者选项*。
*   一旦完成，你现在可以在主*设置*页面的*关于手机*选项下面看到*开发者选项*。
*   进入开发者选项，向下滚动直到在*调试*部分找到 *USB 调试*选项。
*   当提示在您的三星 Galaxy Z Fold 4 上启用 USB 调试时，选择此选项并选择“确定”。

### 步骤 2:使用 ADB 删除已安装的软件包

*   您需要在您的计算机上安装 ADB 来完成这一特定步骤，因此在继续之前，请确保您已经对其进行了分类。您可以查看我们的'[如何安装 ADB '指南](https://www.xda-developers.com/install-adb-windows-macos-linux/)来轻松完成。
*   下一步是将 Galaxy Z Fold 4 插入您的计算机，并在出现提示时将 USB 设置从仅*充电手机*模式更改为*传输文件*模式。
*   使用 Windows 计算机执行此过程的用户可以浏览到 ADB 的安装目录，然后按 Shift +右键单击该目录的名称，并在此处打开命令/PowerShell 窗口。
*   Mac 用户将需要启动一个终端窗口，并使用 cd `<path to the directory>`导航到 ADB 目录。只是给你一个理解，在我的 Macbook 上是`cd /Users/karthiksmac/Desktop/platform-tool`。
*   一旦你连接上了，只需输入`adb devices`并按回车键就能看到你手机的序列号。在苹果电脑上，你必须输入`./adb devices`才能看到序列号。
*   该代码将在您的手机上触发一个提示，要求您授权继续。您可以点击*允许*进行下一步。
*   之后，重新运行`adb devices`或`./adb devices`代码以查看序列号。

### 步骤 3:移除膨胀件

*   这里你需要做的第一件事是键入`adb shell`或`./adb shell`并按回车键。
*   然后，您可以使用以下命令来填充手机上安装的 Samsung 应用程序列表:
*   你也可以只过滤掉三星应用程序包，但列表仍然会很长。相反，我们建议下载一个名为软件包名称查看器 2.0 的应用程序，以确定您要卸载的正确应用程序。
*   一旦你有了想要卸载的应用程序的正确包名，你就可以使用以下命令将其从 Galaxy Z Fold 4 中删除。

    pm uninstall-k-user 0 name of package

*   请注意，您必须将上面提到的命令中的“NameOfPackage”替换为您要卸载的应用程序的完整软件包名称，不带任何“或<>。

继续使用软件包名称查看器 2.0 应用程序找到膨胀软件的正确软件包名称，并卸载它们。就这样，你现在已经成功地从 Galaxy Z Fold 4 上卸载了臃肿软件。移除臃肿软件并不复杂，但你需要花一些时间浏览应用程序并手动输入软件包名称。

如果这太单调乏味，并且你不想逐个检查每个应用程序，你也可以使用一个应用程序删除 GUI 来一次性删除膨胀软件。你可以去我们的 [XDA 论坛的“通用 Android 解包器”](https://forum.xda-developers.com/t/2022-04-03-v0-5-universal-android-debloater.4069209/)线程下载并学习使用这个特定 GUI 的步骤。

使用 GUI 来删除臃肿的软件相对容易，因为你可以选择一堆软件包，然后简单地点击一个按钮就可以把它们从手机上删除。它还会给你一个恢复它们的选项，只需点击一个按钮，如果你最终误删除了一个包，这是非常方便的。

* * *

## 结束语

处理膨胀软件总是很烦人，但谢天谢地，这是一个相当简单的任务。您也可以使用本文中提到的相同方法来删除其他 Android 智能手机中的膨胀软件，因此可以随意开始清理您的 Android 手机。

 <picture>![The Galaxy Z Fold 4 has fewer compromises, is more durable and overall a much better smartphone than its predecessors.](img/376ad5acd59cec0c830475d60d556f9c.png)</picture> 

Samsung Galaxy Z Fold 4

Galaxy Z Fold 4 的妥协更少，更耐用，总体而言是一款比其前辈好得多的智能手机。

如果你刚刚为自己买了一台全新的 Galaxy Z Fold 4，那么你可能会有兴趣看看我们为它收集的[最佳案例](https://www.xda-developers.com/best-samsung-galaxy-z-fold-4-cases/)。这是一部昂贵的手机，所以如果你还没有保护它，为什么不用保护套保护它呢？如果你想为 Galaxy Z Fold 4 挑选一款新的快速充电器，我们还收集了一些[最佳充电器](https://www.xda-developers.com/best-samsung-galaxy-z-fold-4-chargers/)。