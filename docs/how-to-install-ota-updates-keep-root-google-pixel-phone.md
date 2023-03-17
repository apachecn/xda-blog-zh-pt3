# 如何在谷歌 Pixel 手机上安装 OTA 更新并保持 root

> 原文：<https://www.xda-developers.com/how-to-install-ota-updates-keep-root-google-pixel-phone/>

拥有一部[谷歌 Pixel 手机](https://www.xda-developers.com/best-pixel-phones/)的部分好处来自于固件映像的适当可用性，这些映像可用于将设备恢复到出厂状态。即使你解锁了引导程序， [root 了手机](https://www.xda-developers.com/root/)，或者做了太多的修补，你可能会发现自己在进行每月安全更新之前，正在寻找恢复股票配置的最后手段。虽然许多铁杆 Android 粉丝知道该怎么做，但并不是每个人都擅长在不丢失 root 的情况下更新手机。

如果你有一台 PC/Mac，并且乐于自己处理事情，除了在你的 Google Pixel 上下载 OTA 更新之外，你还可以通过执行一些额外的步骤来轻松保持 root 访问。在本教程中，我们将向您展示如何操作。

**浏览这篇文章:**

* * *

* * *

## 寻根如何影响安装 OTA 更新的能力

boot 包括修改部分 Android 启动映像，以便获得超级用户访问权限。定期的每月 OTA 或“空中”更新本质上是增量式的，这意味着 it 不能应用增量补丁来升级库存启动映像，因为在根环境中存在明显的二进制不匹配。虽然选择完整的更新包是解决这个问题的可行方案，但它最终会覆盖从引导分区进行根访问所需的一些内容。

所以，对于那些打算弄脏你的 Pixel 并可能需要一个救世主的人，我们认为我们应该确保你知道如何在每月的安全更新中保持 root 访问。这个过程并不难，但是需要一些 ADB 和 Fastboot 命令。

* * *

## 如何保持根和 OTA 更新你的像素

开始之前，请注意，本教程假设您有一个解锁的引导加载程序，并且[已经以 Magisk](https://www.xda-developers.com/how-to-install-magisk/) 为根。此外，确保您的 PC/Mac 上安装了最新的 [ADB 和 Fastboot 二进制文件](https://www.xda-developers.com/install-adb-windows-macos-linux/)，并且这些工具可以检测到目标设备。

有几种方法可以让你的 Pixel 更新到最新的 Android 官方版本，同时保持 root。您可以恢复基本版本的普通启动映像，等到您的手机收到通知，提示您将任何等待的更新下载到您的手机(或手动下载更新)，然后修补更新的启动映像并刷新它。这是一个有点慢，但建议初学者使用的方法。

在保持 root 的同时，一个相对更快地获得 Google Pixel 最新更新的方法是用一个预打补丁的引导映像来刷新官方出厂映像。请记住，这两种方法都依赖于对 PC 或 Mac 的访问。它们都不需要你擦除设备，但是备份任何不可替代的数据是个好习惯，以防出错。

请注意， [Google Pixel 7 系列](https://www.xda-developers.com/google-pixel-7-pro/)(以及使用 Android 13 启动的设备)，通用内存磁盘从启动映像中移除，并放置在一个名为“init_boot”的独立分区中。因此，您需要修补 init_boot 映像，而不是常规的引导映像，以便对这些设备进行根操作。如果你有 Pixel 7 或 Pixel 7 Pro，在下面的教程中，将每次出现的 *boot.img* 替换为 *init_boot.img* 。

### 推荐方法

1.  找到谷歌 Pixel 手机上当前安装的软件的确切版本号。导航至**设置** > **关于手机**并记下**版本号**部分下的文本。
2.  现在我们需要恢复与已安装的构建版本相对应的未接触的引导映像。作为预防措施，打开 Magisk，切换到**模块**选项卡，禁用活动模块，并在此之前重启一次。
    *   根据修补方法的不同，Magisk 应用程序可能会保留一份普通启动映像的备份。在这种情况下，您应该能够在 Magisk 应用程序的**卸载**菜单下通过**恢复图像**选项恢复它们。尽管如此，我们还是建议从工厂映像中刷新未触及的 boot.img，以避免任何不可预见的问题。

3.  在您的 PC/Mac 上下载与您的 Google Pixel 手机的当前 Android 内部版本号相对应的 fastboot-flashable 工厂映像。应该命名为`<device codename>-<build number>-factory-<hash value snippet>.zip`。
4.  使用您最喜欢的归档管理器打开工厂映像，找到`image-<device codename>-<build number>.zip`文件(是的，在一个 ZIP 文件中有一个 ZIP 文件)，并从中提取 boot.img 文件。[](https://www.xda-developers.com/how-to-unlock-bootloader-root-magisk-google-pixel-6a/google-pixel-6a-firmware-stock-boot-image/)
5.  安装当前 Android 版本号的 stock boot.img:
    1.  确保在手机上启用了 USB 调试，并且电脑上的`adb devices`命令会返回手机的序列号。
    2.  重启手机至引导模式:`adb reboot bootloader`
    3.  闪现股票启动图像:`fastboot flash boot <full patch of the stock boot.img>`
    4.  重启:`fastboot reboot`

6.  你现在可以通过进入**设置** > **系统** > **系统更新** > **检查更新**来强制你的手机获取任何等待更新。或者，为您的型号下载最新的可恢复闪存完整 OTA 映像，并手动[侧载它](https://www.xda-developers.com/how-to-install-android-13/#method1)。
    *   不要选择最新的出厂映像进行升级，因为收件箱闪烁脚本会默认擦除设备。

7.  既然您已经使用了最新的构建版本，那么是时候用 Magisk 修补引导映像以重新获得 root 访问权限了。我们有一个关于如何安装 Magisk 的专门教程，所以如果你需要任何帮助，可以看看它。
8.  一旦你的手机重新启动后闪回补丁启动图像，你应该安全地与根访问最新的 OTA 更新。

* * *

### 快速方法

1.  在 PC/Mac 上下载与 Pixel 手机最新更新相对应的出厂映像。你可以从[谷歌的下载门户](https://developers.google.com/android/images)或者从我们的 [Android 13 下载索引](https://www.xda-developers.com/how-to-download-android-13/)中下载。
2.  使用您最喜欢的归档管理器打开工厂映像，找到映像- <device codename="">- <build number="">。zip 文件，并从中提取 boot.img 文件。</build></device>
3.  [使用 Magisk](https://www.xda-developers.com/how-to-install-magisk/) 修补股票引导镜像，但不要在你的手机上刷新。
4.  将 Magisk 修补的启动映像从手机复制到 PC/Mac，并将其重命名为 boot.img。
5.  用您选择的归档管理器打开步骤 2 中的`image-<device codename>-<build number>.zip`文件，并用步骤 4 中的文件替换其中的股票引导镜像文件。
6.  要删除数据擦除程序，请修改闪存脚本，如下所示:
    *   如果您在 Windows 上，那么用记事本(或您最喜欢的文本编辑器)打开名为“flash-all.bat”的文件，从快速启动闪存段中删除“-w”参数，并保存该文件。
    *   对于 Linux 和 macOS，使用您喜欢的文本编辑器打开名为“flash-all.sh”的文件，从快速启动闪存段中删除“-w”参数，并保存该文件。

7.  重启你的 Pixel 手机到引导模式，然后[使用快速启动](https://www.xda-developers.com/how-to-install-android-13/#method2)进行刷新操作。
8.  如果一切顺利，手机应该会自动重启到最新的操作系统版本——这也是一个预根的启动映像。

没有电脑吗？虽然可以指示 Magisk 在执行增量 OTA 之前将其自身安装到非活动插槽中，并在更新后保持 root，但在此过程中您可能会遇到一些意想不到的障碍。因此，我们建议您自己修补启动映像，并使用 PC 刷新它。

* * *

## 确认

检查你是否正确遵循了所有这些步骤的一个简单方法是前往**设置** > **关于手机** > **安卓版本**。你应该会看到你在谷歌 Pixel 设备上下载的补丁和版本号。

接下来，从应用程序抽屉中打开 Magisk 应用程序，Magisk 内部版本号应该列在“Installed”参数旁边，表明您已经成功地完成了该过程。

* * *

* * *

如果你对谷歌 Pixel 手机有任何疑问，请在下面的评论区留言。