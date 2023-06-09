# 如何在 Nothing Phone 1 上下载 Nothing OS OTA 更新

> 原文：<https://www.xda-developers.com/how-to-sideload-nothing-os-ota-updates-on-nothing-phone-1/>

T2 的 Nothing 手机终于上市了，它带有一个叫做 Nothing OS 的轻量级 Android 皮肤。它可能没有得到谷歌像素得到的一些第一方秘密酱，但用户界面是一个令人惊讶的香草体验，充满了无处不在的设计语言的微妙联系。然而，该软件并不是没有问题，没有什么很好地意识到这一事实。该公司定期推出无操作系统更新，以消除漏洞并引入新功能。

有时，您可能想要在软件更新通过无线方式到达之前手动安装它。别担心，我们将向您展示如何在您的 Nothing Phone 1 上下载 Nothing OS OTA 更新。这不是一个非常困难的过程，但如果没有正确遵循，**你可能不得不彻底清除你的设备并重新开始**。

**浏览这篇文章:**

* * *

* * *

## 如何在 Nothing Phone 1 上下载 Nothing OS OTA 更新

从侧面加载过程开始，首先，您需要为您的设备变体获取合适的 OTA 更新包。为此，请查看我们的 [Nothing Phone 1 更新跟踪器](https://www.xda-developers.com/nothing-phone-1-nothing-os-update-tracker/)，并下载与您想要安装的 Nothing OS 版本相对应的 ZIP 文件。

对于每个 Nothing OS 版本，您应该能够找到两种类型的 OTA 文件:完整的和增量的。完整的更新包被推荐用于侧装，因为它们可以升级手机，不管以前安装的是什么版本。当您是根用户时，它们也很有用[，因为您可以从它们中提取股票引导映像，对其打补丁，然后刷新它以保持根用户访问。增量更新包比相应的完整 OTA 相对较小，但它只能在未接触的基础上应用。](https://www.xda-developers.com/how-to-bootloader-unlock-root-magisk-nothing-phone-1/)

此手动安装过程不会擦除您的设备，但最好备份任何不可替代的数据，以防出现问题。

### 包验证

在尝试手动安装无操作系统更新之前，您应该验证下载的软件包的 SHA-1 哈希。在这种情况下，恢复 ZIP 的 SHA-1 校验和应该与文件名完全相同(减去*。zip 扩展名)。即使一个字符的差异也足以表明文件被篡改。这就是你如何检测一个损坏的下载。

Android 附带了一个名为`sha1sum`的 CLI 工具，用于 SHA-1 校验和计算。您可以使用它来验证 OTA 文件的哈希。

### 通过恢复安装

Nothing Phone 1 带有谷歌像素式恢复模式。因此，您可以通过恢复界面轻松下载更新包。

1.  在 PC/Mac/Chromebook 上下载更新 ZIP 文件。
2.  确保 ADB 可以从您的计算机中发现“无电话 1”。
3.  在您的计算机上，运行命令:

    ```
     adb reboot recovery 
    ```

4.  你应该会在手机屏幕上看到“没有命令”。现在按住手机的电源键。按住电源，按下音量增大按钮，然后快速放开两个按钮。你应该 Android 恢复菜单。[](https://www.xda-developers.com/nothing-phone-1-nothing-os-update-tracker/nothing-phone-1-recovery-mode/)
5.  在手机上，选择**应用来自 ADB 的更新**选项。
6.  在您的计算机上，运行命令:

    ```
     adb devices 
    ```

    这将返回一个设备序列号，其名称旁边带有“sideload ”,表明您的设备以侧载模式连接到计算机。
7.  在您的计算机上，运行命令:

    ```
     adb sideload "filename".zip 
    ```

    ，其中“文件名”将替换为完整路径，后跟在步骤 1 中下载的文件的名称。
8.  更新应该会安装在您的手机上。安装完成后，在手机上选择“立即重启系统”来重启到新版本。

### 通过本地系统更新向导安装

Nothing OS 带有内置的系统更新安装应用程序，但该公司尚未将其作为用户可访问的选项。不过，你可以使用自定义拨号器代码或通过任何活动启动器应用程序来启动它。

1.  在手机内部存储的根目录下创建一个名为“ota”(不带引号)的文件夹。然后将更新 ZIP 文件复制到该文件夹。
2.  拨`*#*#682#*#*`打开离线更新工具。
    *   您还可以使用活动启动器应用程序来定位和执行“OfflineOTAUpgrade”工具。工具的包名是`com.nothing.OfflineOTAUpgradeApp`。[](https://www.xda-developers.com/nothing-phone-1-nothing-os-update-tracker/nothing-os-offline-ota-upgrade/)
3.  向导将尝试找到内存中存在的任何有效 OTA 文件并安装它。如果失败，它会让您手动浏览 OTA 包。
4.  选择 OTA 文件后，向导将应用更新并重启设备。

* * *

## 确认

检查您是否正确遵循了所有这些步骤并正确下载 OTA 文件的一个简单方法是在您的 Nothing Phone 1 上进入**设置** > **关于电话** > **软件信息**。

这应该是您已经侧装的确切的 Nothing OS 版本，表明您已经成功地完成了安装过程。

**[没事电话 1 XDA 论坛](https://forum.xda-developers.com/f/nothing-phone-1.12585/)**

Nothing OS 还处于初级阶段，这就是为什么你还找不到很多定制选项的原因。尽管如此，在当前的公共版本上手动[启用隐藏的字形照明音乐可视化特性](https://www.xda-developers.com/how-to-enable-glyph-lighting-music-visualization-nothing-phone-1/)是可能的。如果你没有 Nothing Phone 1，但喜欢在你当前的 Android 设备上应用 Nothing OS 美学，你也可以通过[下载股票壁纸](https://www.xda-developers.com/download-nothing-phone-1-wallpapers/)来实现。

* * *

**你对虚无 OS 和虚无 Phone 1 有什么看法？下面就让我们知道吧！**