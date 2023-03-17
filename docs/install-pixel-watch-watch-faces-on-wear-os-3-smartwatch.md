# 以下是如何在 Wear OS 3 智能手表上从 Pixel Watch 获得新的手表表盘

> 原文：<https://www.xda-developers.com/install-pixel-watch-watch-faces-on-wear-os-3-smartwatch/>

谷歌的第一款 Wear OS 智能手表 [Pixel Watch](https://www.xda-developers.com/google-pixel-watch-review/) ，可能不是[最好的智能手表](https://www.xda-developers.com/best-smartwatches/)。但它提供了一些独特的功能，这些功能是其他原始设备制造商的智能手表所没有的。例如，它配备了许多新的表盘，赋予它独特的美感，但不幸的是，其他 Wear OS 智能手表上没有。如果你想在你的 Wear OS 3 智能手表上安装它们，你会很高兴知道有一个简单的解决方法。

Pixel 手表有 18 个独特的表盘，从只显示时间的最小表盘到提供许多健康和健身跟踪指标的更复杂的表盘。以下图库展示了 Galaxy Watch 4 上运行的 Pixel Watch 的所有新手表外观。

如果你想在 Wear OS 3 智能手表上获得这些手表外观，如 [Galaxy Watch 5](https://www.xda-developers.com/samsung-galaxy-watch-5-review/) 或 [Galaxy Watch 4](https://www.xda-developers.com/samsung-galaxy-watch-4-classic-review/) ，你会很高兴知道 APK 现在可以下载了。点击下面的链接下载谷歌手表面部 APK，并将其加载到你的智能手表上。如果你不熟悉这个过程，这里有一个快速概述。

## Wear OS 3 智能手表的侧面像素手表表盘

你必须使用 ADB 在你的 Wear OS 3 智能手表上安装 Pixel Watch 的表盘。但首先，您必须从 APKMirror 下载 APK，并将其保存在与您 PC 上的 ADB 平台工具相同的目录中。完成后，按照下面提供的步骤为智能手表准备 ADB 调试:

1.  打开 Wear OS 3 智能手表上的**设置应用**，导航至**软件信息**页面。
2.  轻按几次**软件版本**以启用**开发者选项**。
3.  一旦你看到一个提示**开发者模式开启**的提示，回到主设置菜单，选择**开发者选项**按钮。
4.  在接下来的页面中，点击ADB 调试旁边的**开关将其启用，然后启用**通过 Wi-Fi 调试**选项。**
5.  确保您的手表已连接到 Wi-Fi，并记下“通过 Wi-Fi 调试”选项下提到的 **IP 地址**。

启用通过 Wi-Fi 调试后，切换到您的 PC，将其连接到同一个 Wi-Fi 网络，并在 ADB 平台工具目录中打开一个新的命令提示符窗口。在命令提示窗口中输入 **adb connect，**后跟 IP 地址，然后点击 **enter** 连接到您的智能手表。

您应该立即在手表上看到一个提示，询问您是否允许调试。选择 **OK** ，如果你想允许调试这一次，或者**总是允许从这台计算机**，如果你不想重复这个过程。

现在，键入以下 ADB 命令并按 enter 键安装 Pixel Watch 手表面部 APK。如前所述，您必须将 APK 与 ADB 平台工具放在同一个目录中，这样该命令才能正常工作。您还应该重命名 APK，使命令不那么复杂。

```
 adb -s "IP address" install filename.apk 
```

安装完成后，您应该会在命令提示符窗口中看到“成功”。之后，使用以下命令断开与 ADB 的连接，并在智能手表上禁用 ADB 调试。

```
 adb disconnect 
```

就是这样！现在，您应该可以在手表的配套应用程序中看到新的 Pixel Watch 表盘。我在我的 Galaxy Watch 4 上安装了手表面部，所有 18 个都可以在可穿戴应用程序中使用。

*感谢米莎尔·拉赫曼的提示！*