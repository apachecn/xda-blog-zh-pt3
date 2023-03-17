# 如何在谷歌 Pixel 和其他 Android 设备上安装 Android 12 和 12L

> 原文：<https://www.xda-developers.com/how-to-install-android-12/>

又到了一年的这个时候了！ [Android 12](https://www.xda-developers.com/android-12/) ，即 Android 的下一个主要版本现已通过[稳定渠道](https://www.xda-developers.com/android-12-stable-rollout-google-pixel/)在[上市](https://www.xda-developers.com/android-12-launched/)。谷歌也已经开始推出 Android 12L，这是一个功能下降，为大屏幕设备带来了一些优化和改进。对于拥有谷歌 Pixel 3a、Pixel 3a XL、Pixel 4、Pixel 4 XL、Pixel 4a、Pixel 4a 5G、Pixel 5、Pixel 5a、 [Pixel 6 或 Pixel 6 Pro](https://www.xda-developers.com/google-pixel-6/) 的幸运用户来说，你将是第一批看到新操作系统更新提供了什么的用户。

如果你有任何上述 Pixel 智能手机运行和旧的稳定版本，并想知道如何安装 Android 12 或 12L，只需向下滚动，因为我们已经为你准备好了教程。请记住，谷歌将为现有的测试版用户提供增量 OTA，以转移到稳定版本，但他们也可以选择手动更新。一旦[下载了相关的 Android 12 发布包](https://www.xda-developers.com/how-to-download-android-12/)，您将需要一台安装了 ADB 和 Fastboot 的 [PC/Mac 来成功执行安装过程。](https://www.xda-developers.com/install-adb-windows-macos-linux/)

除了受支持的谷歌 Pixel 设备，Android 12/12L 还以 GSI 的形式提供，可以在更广泛的设备上播放。原始设备制造商也加入了这场派对，你可以在以下手机上 flash Beta 1:

**警告:**更新仅供开发者使用，所以不要安装在你的日常驱动上。这些构建是早期版本，包含错误和其他系统不稳定性。即使刷新过程不一定会擦除您的设备，也强烈建议您在继续之前备份数据。建议用户谨慎使用。

**安装更新的三种方法是:**

* * *

## 方法 1:通过恢复和 ADB 侧装 Android 12/12L

要安装稳定版本，您需要通过 ADB 为您的设备从恢复中下载适当的 OTA 包。这种方法也适用于带有锁定引导程序的 Google Pixel 设备。

1.  下载更新。你电脑上的 zip 文件[从这里](https://www.xda-developers.com/how-to-download-android-12/)。为了方便起见，您可以将该文件重命名为一个更简单的名称，并将该文件放在您计算机上 ADB 所在的目录中。
2.  可选但建议:验证您下载的文件的 SHA-256 校验和，以确保该文件已完全正确下载。
3.  在手机上启用 USB 调试-进入设置>关于手机>轻按“内部版本号”7 次，(可选)输入您的模式，PIN 或密码以启用开发者选项，然后导航到设置>开发者选项>启用“USB 调试”。
4.  将手机连接到电脑。如果这是您第一次与亚行计算机连接，当手机上出现提示时，请在手机上授权您的计算机连接。
5.  在您的计算机上，运行命令:

    ```
     adb reboot recovery 
    ```

6.  你应该会在手机屏幕上看到“没有命令”。现在按住手机的电源键。按住电源的同时，按下音量增大按钮，然后快速放开这两个按钮。你应该 Android 恢复菜单。
7.  从恢复菜单中选择选项*应用来自 ADB 的更新*。
8.  在您的手机上，选择“应用亚行更新”选项
9.  在您的计算机上，运行命令:

    ```
     adb devices 
    ```

    这将返回一个设备序列号，其名称旁边带有“sideload ”,表明您的设备以侧载模式连接到计算机。
10.  在您的计算机上，运行命令:

    ```
     adb sideload "filename".zip 
    ```

    ，其中“文件名”将替换为步骤 1 中下载的文件的名称
11.  更新应该会安装在您的手机上。安装完成后，在手机上选择“立即重启系统”，重启进入 Android 12。

* * *

## 方法 2:通过快速启动刷新完整的工厂映像

如果你在谷歌 Pixel 设备上有一个解锁的引导程序，你需要通过 Fastboot 刷新 Android 12 或 12L 的完整出厂映像。通常，这是通过下载文件中包含的 *flash-all.sh* 或 *flash-all.bat* 脚本文件来完成的，但其默认配置也会完全擦除设备。但是，您可以通过从脚本的命令中删除“-w”wipe 属性来保留您的数据。

1.  下载工厂图像。从这里打开你电脑上的[zip 文件。](https://www.xda-developers.com/how-to-download-android-12/)
2.  可选但建议:验证您下载的文件的 SHA-256 校验和，以确保该文件已完全正确下载。
3.  提取。zip 文件，为了方便起见，将结果文件复制并粘贴到您计算机上的 ADB 和 fastboot 文件夹中。
4.  可选:结果文件将包含一个 *flash-all.sh* 或 *flash-all.bat* 脚本文件。使用文本编辑器，打开 *flash-all.sh* (如果你在 macOS/Linux 上)或 *flash-all.bat* 脚本文件(如果你在 Windows 上)。找到并移除/删除`fastboot update`命令中的-w 标志。这将跳过你的手机数据擦除。为了避免兼容性问题，建议进行数据擦除。
5.  在手机上启用 USB 调试-进入设置>关于手机>轻按“内部版本号”7 次，(可选)输入您的模式，PIN 或密码以启用开发者选项，然后导航到设置>开发者选项>启用“USB 调试”。
6.  将手机连接到电脑。如果这是您第一次与亚行计算机连接，当手机上出现提示时，请在手机上授权您的计算机连接。
7.  在你的电脑上运行:

    ```
     adb reboot bootloader 
    ```

    这将重启你的手机进入快速启动模式。
8.  在您的 Mac/Linux PC 上，运行:

    ```
     flash-all 
    ```

    该命令执行 *flash-all.sh* 脚本文件，然后安装必要的引导程序、基带固件和操作系统。如果您使用的是 Windows，只需双击 flash-all.bat 文件。
9.  一旦脚本完成，您的设备将重新启动到新的操作系统。

* * *

## 方法三:安装安卓 12/12L GSI

即使你没有兼容的 Pixel 智能手机，你仍然可以安装谷歌官方的 GSI 二进制文件来测试 Android 12 或 12L，前提是你的设备兼容 Project Treble。您还需要一个解锁的引导加载程序。我们需要说的最后一件事是，刷新 GSI 将需要您在工厂重置您的设备，所以请确保您在继续操作之前准备好丢失应用程序数据！我们建议您进行设备外备份(例如在您的 PC 或 SD 卡上)，以防出现任何问题。

1.  官方 Android 12/12L Beta GSIs 的下载链接可以在[这里](https://www.xda-developers.com/how-to-download-android-12/)找到。Google 还没有发布基于稳定版本的 GSIs。您应该根据您设备的架构下载合适的版本。要查看您的设备的架构，运行以下命令:

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
7.  如前所述，目标设备**的引导程序必须事先解锁**。
8.  接下来，我们需要禁用 Android 验证启动(AVB)。为此，运行以下命令:

    ```
     fastboot flash vbmeta vbmeta.img 
    ```

9.  可选但推荐:输入以下命令来擦除系统分区:

    ```
     fastboot erase system 
    ```

10.  flash Android 12/12L GSI:

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

**请务必关注我们的 [Android 12](https://www.xda-developers.com/tag/android-12/) 和 [Android 12L](https://www.xda-developers.com/tag/android-12l/) 标签，了解新 Android 版本的所有最新消息！**