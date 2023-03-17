# 如何在谷歌 Pixel 和其他 Android 设备上安装 Android 13

> 原文：<https://www.xda-developers.com/how-to-install-android-13/>

安卓 13 的稳定版来了。如果你有一部[合格的 Pixel 智能手机](https://www.xda-developers.com/how-to-download-android-13/)，你现在就可以试一试。谷歌还提供通用系统映像(GSI)，这意味着最新版本的 Android 也可以在非谷歌 Project Treble 兼容设备上启动。

如果你有 Pixel 4、Pixel 4 XL、Pixel 4a、Pixel 4a 5G、Pixel 5、Pixel 5a、Pixel 6、Pixel 6 Pro 或 Pixel 6a 运行较旧的稳定版本，并且想知道如何安装 Android 13，只需向下滚动，因为我们已经为你准备好了教程。下面列出的方法同样适用于新发布的 [Pixel 7 系列](https://www.xda-developers.com/google-pixel-7-pro/)。您需要一台安装了 [ADB 和 Fastboot](https://www.xda-developers.com/install-adb-windows-macos-linux/) 的 PC/Mac 来成功执行安装过程。

**警告:**虽然你仍然可以 flash 预览版本，但那些预稳定的版本仅供开发人员使用，所以不要在你的日常驱动中安装它们。您可能会遇到 showstopper 错误或其他系统不稳定问题。强烈建议您在继续之前备份数据。建议用户谨慎使用。

**安装更新的三种方法是:**

* * *

## 方法一:通过恢复和 ADB 侧装 Android 13

要安装开发者预览版/测试版，您需要通过 ADB 为您的设备从 Recovery 中下载适当的 OTA 包。这种方法也适用于带有锁定引导程序的 Google Pixel 设备。

1.  下载更新。从这里打开您计算机上的 zip 文件[。为了方便起见，您可以将该文件重命名为一个更简单的名称，并将该文件放在您计算机上 ADB 所在的目录中。](https://www.xda-developers.com/how-to-download-android-13/)
2.  可选，但建议:验证您下载的文件的 SHA-256 校验和，以确保文件已被完全和正确下载。
3.  在手机上启用 USB 调试-进入*设置* > *关于手机* >轻点*构建号* 7 次，(可选)输入你的模式、PIN 或密码启用开发者选项，然后导航至*设置* > *开发者选项* >启用 *USB 调试*。
4.  将手机连接到电脑。如果这是您第一次连接此计算机的 ADB 实例，当提示出现在您的电话上时，在您的电话上授权您的计算机连接。
5.  在您的计算机上，运行命令:

    ```
     adb reboot recovery 
    ```

6.  你应该会在手机屏幕上看到“没有命令”。现在按住手机的电源键。按住电源，按下音量增大按钮，然后快速放开两个按钮。你应该 Android 恢复菜单。
7.  从恢复菜单中选择选项*应用来自 ADB 的更新*。
8.  在您的计算机上，运行命令:

    ```
     adb devices 
    ```

    这将返回一个设备序列号，其名称旁边带有“sideload ”,表明您的设备以 sideload 模式连接到计算机。
9.  在您的计算机上，运行命令:

    ```
     adb sideload "filename".zip 
    ```

    “filename”部分将替换为在步骤 1 中下载的文件的名称。
10.  更新应该会安装在您的手机上。安装完成后，在手机上选择*立即重启系统*重启进入 Android 13。

* * *

## 方法 2:通过快速启动刷新完整的工厂映像

如果你在谷歌 Pixel 设备上有一个解锁的 bootloader，你需要通过 Fastboot 刷新 Android 13 开发者预览版/测试版的出厂映像。通常，这是通过下载文件中包含的 *flash-all.sh* 或 *flash-all.bat* 脚本文件来完成的，但其默认配置也会完全擦除设备。但是，您可以通过从脚本的命令中删除“-w”wipe 属性来保留您的数据。

1.  下载工厂图像。从这里打开您电脑上的 zip 文件[。](https://www.xda-developers.com/how-to-download-android-13/)
2.  可选，但建议:验证您下载的文件的 SHA-256 校验和，以确保文件已被完全和正确下载。
3.  提取。zip 文件，为了方便起见，将结果文件复制并粘贴到您计算机上的 ADB 和 fastboot 文件夹中。
4.  可选:结果文件将包含一个 *flash-all.sh* 或 *flash-all.bat* 脚本文件。使用文本编辑器，如果你在 macOS/Linux 上，打开 *flash-all.sh* ，或者如果你在 Windows 上，打开 *flash-all.bat* 脚本文件。找到并移除/删除`fastboot update`命令中的-w 标志。这将跳过你的手机数据擦除。为了避免兼容性问题，建议进行数据擦除。
5.  在手机上启用 USB 调试-进入*设置* > *关于手机* >轻点*编译号* 7 次，(可选)输入你的模式、PIN 或密码启用开发者选项，然后导航至*设置* > *开发者选项* >启用 *USB 调试*。
6.  将手机连接到电脑。如果这是您第一次连接此计算机的 ADB 实例，当提示出现在您的电话上时，在您的电话上授权您的计算机连接。
7.  在你的电脑上运行:

    ```
     adb reboot bootloader 
    ```

    这将重启你的手机进入快速启动模式。
8.  在您的 Mac/Linux PC 上，运行:

    ```
     flash-all 
    ```

    该命令执行 *flash-all.sh* 脚本文件，然后安装必要的引导加载程序、基带固件和操作系统。如果你在 Windows 上，你可以简单地双击 *flash-all.bat* 文件。
9.  一旦脚本完成，您的设备将重新启动到新的操作系统。

* * *

## 方法三:安装安卓 13 GSI

即使你没有兼容的 Pixel 智能手机，你仍然可以安装谷歌官方的 GSI 二进制文件来测试 Android 13，前提是你的设备兼容 Project Treble。您还需要一个解锁的引导加载程序。我们需要说的最后一件事是，刷新 GSI 将需要您在工厂重置您的设备，所以请确保您在继续操作之前准备好丢失应用程序数据！我们建议您进行设备外备份(例如在您的 PC 或 SD 卡上)，以防出现任何问题。

1.  官方 Android 13 测试版 GSIs 的下载链接可以在[这里](https://www.xda-developers.com/how-to-download-android-13/)找到。Google 还没有发布基于稳定版本的 GSIs。您应该根据您设备的架构下载合适的版本。要查看您的设备的架构，请运行以下命令:

    ```
     adb shell getprop ro.product.cpu.abi 
    ```

2.  可选但建议:验证您下载的文件的 SHA-256 校验和，以确保该文件已完全正确下载。
3.  提取。zip 文件，为了方便起见，将结果文件( **system.img** 和 **vbmeta.img** )复制并粘贴到您电脑上的 ADB 和 fastboot 文件夹中。
4.  在手机上启用 USB 调试-进入设置>关于手机>轻按“内部版本号”7 次，(可选)输入您的模式，PIN 或密码以启用开发者选项，然后导航到设置>开发者选项>启用“USB 调试”。
5.  将手机连接到电脑。如果这是您第一次与亚行计算机连接，当手机上出现提示时，请在手机上授权您的计算机连接。
6.  在你的电脑上运行:

    ```
     adb reboot bootloader 
    ```

    这将重启你的手机进入快速启动模式。
7.  如前所述，目标设备**的引导加载程序必须事先解锁**。
8.  接下来，我们需要禁用 Android 验证启动(AVB)。为此，运行以下命令:

    ```
     fastboot flash vbmeta vbmeta.img 
    ```

9.  可选但推荐:输入以下命令来擦除系统分区:

    ```
     fastboot erase system 
    ```

10.  flash Android 13 GSI:

    ```
     fastboot flash system system.img 
    ```

11.  让图像闪烁，这可能需要几分钟时间。一旦完成，清除用户数据分区:

    ```
     fastboot -w 
    ```

12.  最后，重启你的设备:

    ```
     fastboot reboot 
    ```

13.  希望你的设备能够启动新版本的 Android。

* * *

除了受支持的谷歌 Pixel 设备，Android 13 作为一个主要版本也可以在不同 OEM 厂商的各种设备上使用——无论是测试版还是稳定版。万一你在寻找“*如何在我的手机上安装 Android 13 这个问题的答案呢？*"，看看以下 OEM 专用追踪器就知道了: