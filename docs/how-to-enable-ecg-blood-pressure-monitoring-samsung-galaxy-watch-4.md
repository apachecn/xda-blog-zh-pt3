# 如何在三星 Galaxy Watch 4 上启用心电图和血压功能

> 原文：<https://www.xda-developers.com/how-to-enable-ecg-blood-pressure-monitoring-samsung-galaxy-watch-4/>

[三星 Galaxy Watch 4](https://www.xda-developers.com/samsung-galaxy-watch-4-classic-review/) 支持广泛的健康跟踪和健身功能。但是，这些功能中的一些并不适用于所有用户。例如，心电图和血压特征被限制在某些区域。此外，当手表与非三星手机配对时，即使在支持的地区也不能使用这些功能。幸运的是，有一个变通办法可以在所有地区获得这些功能，甚至在非三星设备上。如果你使用的是非三星手机的 Galaxy Watch 4，或者由于地区限制而无法使用这些功能，这里介绍了如何在 Galaxy Watch 4 上启用心电图和血压功能。

## 如何在三星 Galaxy Watch 4 上启用心电图和血压功能

要在不受支持的地方或使用非三星手机在三星 Galaxy Watch 4 上启用心电图和血压监测，您需要安装 XDA 高级会员 [Dante63](https://forum.xda-developers.com/m/dante63.7047928/) 的改装三星健康监测应用程序。你必须在你的手机和 Galaxy Watch 4 上安装这款应用。

然而，这个过程并不像听起来那么简单。为了使事情更容易，我们已经详细地概述了指令。但是，在继续之前，请从下面的链接下载所有需要的文件。

[**下载改装的三星健康监测 app**](https://drive.google.com/drive/folders/138thPYPMbZIp2Us0Unx_h-SqJQEDxZ-0)

上面链接的 Google Drive 文件夹包含了在 Galaxy Watch 4 上实现心电图和血压监测所需的所有文件。它还包括几个指南来帮助你，以防你在这个过程中遇到麻烦。

***注:**确保你的手机上安装了 [Galaxy 可穿戴设备应用](https://play.google.com/store/apps/details?id=com.samsung.android.app.watchmanager2)并与 Galaxy Watch 4 配对。另外，一定要从 Play Store 安装 [Galaxy Watch 4 插件](https://play.google.com/store/apps/details?id=com.samsung.android.waterplugin)。*

### 在您的手机上安装修改后的三星健康监测应用程序

在手机上安装修改后的三星健康监测应用程序是一个非常简单的过程。你所需要做的就是在上面链接的驱动器文件夹中找到修改后的应用程序。we aros . shm . mod . x . x . x . XXX . Dante 63 . apk)并转移到手机根目录。

在您的手机上，使用文件浏览器导航到根目录，并找到修改后的 APK。

***注意:**在这篇文章中，我使用的是[一加 10 Pro](https://www.xda-developers.com/oneplus-10-pro-review/) 和股票 OxygenOS MyFiles 应用程序。如果你的手机上没有文件浏览器，你可以下载我们收集的[安卓](https://www.xda-developers.com/best-file-manager-android/)最佳文件管理应用中列出的任何选项。*

点击改装的三星健康监测 APK 安装它。您现在应该会看到一个权限弹出窗口，允许您安装来自未知来源的应用程序。按照提示前往设备设置，并允许从文件管理器安装应用程序。

您应该立即看到另一个带有*安装*按钮的弹出窗口。点击它来安装应用程序，然后点击下面弹出的*完成*来完成安装。

这就完成了简单的部分。现在，让我们继续复杂的部分，即使用 ADB 在 Galaxy Watch 4 上安装修改后的三星健康监测应用程序。

### 在您的 Galaxy Watch 4 上安装修改后的三星健康监测应用程序

在 Galaxy Watch 4 上安装修改后的三星健康监视器应用程序需要 ADB。如果你不熟悉在你的电脑上安装 ADB，你会很高兴知道 Dante63 提供了一个简单的解决方案。

打开上面链接的 Google Drive 文件夹中的 **Watch SHM MOD WearOS 文件夹**。然后，打开**READ ME-ADB Manual instructions**文件夹，将文件夹中 ZIP 文件的内容解压到桌面。双击 ZIP 文件中的最小 ADB 快速启动可执行文件，并按照安装向导中提供的说明设置 ADB。

完成安装后，会立即弹出一个命令提示符窗口。如果没有，只需导航到您安装最小 ADB Fastboot 时的目录，并双击标记为**cmd-here**的文件。

在继续之前，请在手表上启用 **ADB 调试和 Wi-Fi 调试**设置。若要启用这些选项，您必须首先打开开发人员选项。为此，前往手表上的设备设置，一路向下滚动到**关于手表**选项并点击它。

在下一页上，选择**软件** 选项，然后点击下一页上的**软件版本** 几次，以启用开发者模式。

跳回设备设置，选择**开发者选项** *。*然后，点击 **ADB 调试和通过 Wi-Fi 调试**设置旁边的开关，启用它们。

***注:**如果您的手表配置为连接 Wi-Fi 网络，它现在应该会自动连接到保存的网络，并向您显示通过 Wi-Fi 调试* *选项下的 IP。如果您没有连接到 Wi-Fi，请前往主设置页面上的连接* *选项，连接到 Wi-Fi 网络。确保您的电脑已连接到同一个 Wi-Fi 网络。为此，您也可以使用手机的移动热点。*

连接到 Wi-Fi 后，点击活动连接并记下下页提到的 IP 地址。

回到 PC 上的最小 ADB 和快速启动命令提示符窗口，键入“adb connect ”,然后键入上一步中的 IP 地址。

您应该立即在手表上看到一个提示，询问您是否允许调试。如果您只想允许调试一次，请选择 **OK** ，如果您不想再次重复该过程，请选择**Always allow from this computer**

现在，将您的手表放在一边，键入以下 ADB 命令，然后按 Enter 键在手表上安装修改后的三星健康监测应用程序。为了使该命令按预期工作，**您需要将修改后的三星健康监测器 APK 放在与标签为*cmd-此处为*** 的文件相同的目录中，即您安装 ADB 的文件夹。另外，将下面提到的命令中的 X 替换为 APK 的当前版本号。

```
 adb -s "IP address" install Watch.SHM.MOD.X.X.X.XXX.dante63.apk 
```

应用程序成功安装后，您应该会在命令提示符窗口中看到“成功”。现在，使用以下命令断开与 ADB 的连接。

```
 adb disconnect 
```

现在，您应该能够在手表的应用程序抽屉中看到修改后的三星健康监测应用程序。当你打开手机上的 modded 应用程序时，你的 Galaxy Watch 4 应该会自动连接，你应该可以看到血压和心电图标签。你可以按照应用程序中提供的说明来设置这些功能。完成后，将心电图和血压贴在你的手表上，你就可以开始了。

在开始使用这些功能之前，请确保在 Galaxy Watch 4 上禁用 ADB 调试，否则会影响其电池寿命。为此，返回到开发人员选项，点击 ADB 调试选项旁边的开关。

值得一提的是，由于这种方法使用了修改过的三星健康监测应用程序，您可能会遇到一些预期的问题。此外，你将无法在手表和手机上的三星健康应用程序之间同步血压数据。然而，我们有一个简单的解决方法，也可以在 Galaxy Watch 4 上启用 BP 同步。你可以通过下面给定的链接来尝试，如果你仍然面临任何问题，你可以在下面链接的 XDA 论坛帖子中提出你的担忧。

**[三星健康监视器 mod XDA 论坛线程](https://forum.xda-developers.com/t/restrictions-removed-samsung-health-monitor-wearos-1-1-1-191-root-age-country-device-restriction-removed-28th-may-2022.4322527/)**