# 突破:安卓 12 测试版 GSI 领先谷歌 I/O 2021 上线

> 原文：<https://www.xda-developers.com/android-12-beta-gsi/>

# 突破:安卓 12 测试版 GSI 领先谷歌 I/O 2021 上线

安卓 12 测试版 1 GSI 软件包已经可以从谷歌的服务器上下载。快去抓吧！

第一次 [Android 12](https://www.xda-developers.com/android-12/) 开发者预览版是在二月份[在](https://www.xda-developers.com/android-12-developer-preview-1/)发布的，随后是[预览版 2](https://www.xda-developers.com/android-12-developer-preview-2/) ，最近是[预览版 3](https://www.xda-developers.com/google-android-12-developer-preview-3-features/) 。谷歌应该在今天发布 Android 12 Beta 1，在 2021 年谷歌 I/O 期间加入 Pixel 阵容。然而，看起来官方的 Android 12 Beta 1 通用系统映像(GSI)包已经可以下载了！

GSI 是一个预构建的系统映像，可以在支持[高音项目](https://www.xda-developers.com/tag/project-treble/)的设备上启动。即使你没有兼容的 Pixel 智能手机，你仍然可以安装谷歌官方的 GSI 二进制程序来测试 Android 12，前提是你的设备与 Project Treble 兼容。您还需要一个未锁定的引导加载程序。我们需要说的最后一点是，闪烁 GSI 将需要您在工厂重置您的设备，所以在继续之前，请确保您准备好丢失应用程序数据。我们建议您制作一个设备外备份(例如在您的电脑或 SD 卡上)，以防出现任何问题。

## 安卓 12 测试版 GSI 下载

下载链接请参见下表:

您应该根据设备的架构选择合适的 GSI 二进制版本。要查看您的设备具有哪种体系结构，请运行以下命令:

```
 adb shell getprop ro.product.cpu.abi 
```

## 安卓 12 测试版 GSI 安装

在尝试安装 Android 12 GSI 之前，确保您可以使用安装了 [adb 和快速启动](https://www.xda-developers.com/install-adb-windows-macos-linux/)的 PC/Mac。

1.  提取。压缩文件，并将结果文件( **system.img** 和 **vbmeta.img** )复制并粘贴到您计算机上的 ADB 和 fastboot 文件夹中，以方便使用。
2.  在手机上启用 USB 调试-转到设置>关于手机>轻按“版本号”7 次(可选)输入您的模式、个人识别码或密码以启用开发人员选项，然后导航到设置>开发人员选项>启用“USB 调试”。
3.  将手机连接到电脑。如果这是您第一次使用这台 ADB 电脑，当您的手机出现提示时，请在手机上授权您的电脑连接。
4.  在您的计算机上，运行:

    ```
     adb reboot bootloader 
    ```

    这将重新启动您的手机进入快速启动模式。
5.  如前所述，目标设备的引导加载程序**必须事先解锁**。
6.  接下来，我们需要禁用 Android 验证启动(AVB)。为此，运行以下命令:

    ```
     fastboot flash vbmeta vbmeta.img 
    ```

7.  可选但推荐:输入以下命令来擦除系统分区:

    ```
     fastboot erase system 
    ```

8.  flash Android 12 GSI:

    ```
     fastboot flash system system.img 
    ```

9.  让图像闪烁，这可能需要几分钟时间。一旦完成，清除用户数据分区:

    ```
     fastboot -w 
    ```

10.  最后，重启你的设备:

    ```
     fastboot reboot 
    ```

11.  希望你的设备能启动到 Android 12 测试版。

如果你有一台运行 Android 11 的设备，那么你也可以尝试开发者选项中的 [DSU 加载器](https://www.xda-developers.com/android-11-dsu-loader-gsi-locked-bootloader-developers-test-apps-stock-android/)实用程序来启动 Android 12 GSI，而不需要摆弄任何 Fastboot 或 ADB 命令。

* * *

*感谢 XDA 知名开发商 [luca020400](https://forum.xda-developers.com/m/luca020400.5778309/) 提供的提示！***