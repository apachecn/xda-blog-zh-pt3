# 在你的 Galaxy Watch 4 上安装 Galaxy Watch 5 的表盘

> 原文：<https://www.xda-developers.com/install-galaxy-watch-5-watch-faces-galaxy-watch-4/>

本月早些时候，三星发布了全新的 [Galaxy Watch 5](https://www.xda-developers.com/samsung-galaxy-watch-5-launch/) 阵容，以及 [Galaxy Z Fold 4](https://www.xda-developers.com/samsung-galaxy-z-fold-4-hands-on/) 和 [Galaxy Z Flip 4](https://www.xda-developers.com/samsung-galaxy-z-flip-4-hands-on/) 。Wear OS 智能手表的新系列带来了几项硬件和软件改进，包括几个新的表盘。如果你有一个旧的 Galaxy Watch 4 型号，并想在你的智能手表上安装新的 Galaxy Watch 5 手表表面，你很幸运！

XDA 成员 [niff2005](https://forum.xda-developers.com/m/niff2005.10449873/) 已经从固件中提取了五个新的 Galaxy Watch 5 手表表面的 APK 文件，你可以使用 ADB 将它们下载到你的 Galaxy Watch 4 上。然而，五个可用的手表表面中只有四个可以在 Galaxy Watch 4 上工作。新的 HealthMonitor 手表 face 不能在 Galaxy Watch 4 上使用，但这很可能是因为智能手表上已经有了一个旧版本。查看以下图库，了解您可以在 Galaxy Watch 4 上尝试的其他手表外观。

*截图:niff2005*

要在你的 Galaxy Watch 4 上安装这些手表外观，请从下面链接的 XDA 论坛下载带有相应 apk 的 ZIP 文件。从*开发者选项*中启用 *ADB 调试和 Wi-Fi 调试*。

将手表连接到 Wi-Fi 网络，并记下在*通过 Wi-Fi 调试*选项中提到的 IP 地址。确保您的电脑连接到同一个 Wi-Fi 网络，并在安装 ADB 平台工具的目录中打开命令提示窗口。在命令提示符窗口中键入“adb connect ”,后跟 IP 地址，然后按 enter 键。

您应该立即在手表上看到一个提示，询问您是否允许调试。选择*确定，如果您想允许调试一次，选择*，或者如果您不想重复该过程，选择*总是允许从这台计算机*。现在，键入以下 ADB 命令，并按 enter 安装手表脸 APK。为了使该命令按预期工作，您还需要将相应的 APK 文件放在与 ADB 平台工具相同的目录中。

```
 adb -s "IP address" install filename.apk 
```

安装完成后，您应该会在命令提示符窗口中看到“成功”。现在，使用以下命令断开与 ADB 的连接。

```
 adb disconnect 
```

你现在应该可以在 Galaxy Watch 4 上看到新的表盘了。如果你希望编辑表盘，niff2005 建议在你的智能手表上编辑，而不是在 Galaxy Wearable 应用程序上编辑，因为在应用程序上编辑似乎会破坏表盘。

**[为您的 Galaxy Watch 4](https://forum.xda-developers.com/t/galaxy-watch5-5-pro-watchfaces-for-watch4-4-classic.4480353/)** 下载新的 Galaxy Watch 5 手表面孔

如前所述，五个 watch face APKs 中的四个应该可以在所有 Galaxy Watch 4 型号上正常工作。但是您的里程可能会有所不同。

你能让这些 Galaxy Watch 5 的表盘在你的 Galaxy Watch 4 上运行吗？请在下面的评论区告诉我们。