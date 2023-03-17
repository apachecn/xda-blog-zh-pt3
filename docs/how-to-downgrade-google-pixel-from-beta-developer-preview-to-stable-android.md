# 如何在谷歌 Pixel 上从 Android 13 测试版降级到 Android 12

> 原文：<https://www.xda-developers.com/how-to-downgrade-google-pixel-from-beta-developer-preview-to-stable-android/>

掌握软件更新游戏的智能手机公司少之又少。幸运的是，谷歌 Pixel 用户不仅可以先于所有人获得重大更新，还可以通过公共测试程序测试即将推出的 Android 版本。自从谷歌通过测试版渠道为符合条件的 Pixel 设备发布 Android 13 已经有一段时间了，尽管这一更新获得了普遍好评，但我们不能忘记这仍然只是一个测试版软件，而不是像 Android 12 那样的日常驱动程序。

如果你不小心安装了一个开发者预览版/测试版，并且你一直想知道如何将你的 Google Pixel 降级回稳定的 Android 版本，那么这个指南就是为你准备的。

**浏览本文:**

* * *

## 将你的谷歌 Pixel 智能手机降级到稳定的安卓版本

虽然开发者预览版和测试版通常旨在帮助应用开发者发现和解决新 Android 版本的问题，但任何人都可以在兼容设备上刷新它们。如果你还没有，想试试，这里有[如何在你的谷歌 Pixel 手机](https://www.xda-developers.com/how-to-install-android-13/)上安装 Android 13。尽管如此，出于可用性的考虑，我们还应该了解从测试版到稳定版的降级过程。我们都可以比其他人更好地处理一些错误，如果更新带来了您无法处理的错误，您可能会寻找返回的选项。

幸运的是，将你的谷歌 Pixel 设备恢复到稳定版本的安卓系统实际上相当容易。你可以要求 Google 给你发送一个特殊的 OTA 来执行转换，或者自己在你的设备上手动刷新稳定版本。唯一的问题是，将操作系统恢复到旧版本需要在此过程中将其重置为出厂设置，这**会从设备**中清除所有数据和设置。因此，在进行下一步之前，请务必[备份您的个人数据](https://www.xda-developers.com/how-to-backup-android/)。

*   从开发者预览版/测试版降级到稳定版通常需要完全的数据擦除。
*   无论是否使用电脑，你都可以对谷歌 Pixel 手机进行降级。
*   恢复到测试频道不需要数据擦除。

* * *

### 方法 1:退出测试程序

这与加入谷歌的 Android 开发者预览/测试计划正好相反。你所需要做的就是将目标像素设备从测试程序中分离出来。然后，谷歌将发布一个特制的 OTA 包，该包将删除测试版，并在你的设备上安装最新的稳定 Android 版本。值得注意的是，这个过程不需要解锁的引导加载程序。

1.  前往 [Android Beta 程序页面](https://www.google.com/android/beta)。
2.  点击或轻触**查看您的合格设备**查看 beta 版注册的 Pixel 设备。
    *   如果您找不到您的设备，请确保您已登录到与您希望回滚的设备相关联的 Google 帐户。
3.  为您需要从 beta 计划中删除的列出设备选择**退出**选项。
4.  目标设备将在 24 小时内收到新的更新。你也可以导航到**设置** > **系统** > **系统更新** > **查看手机上的更新**看看是否有更新。
5.  OTA 一到就装。
6.  就是这样！

如前所述，OTA 会在闪存过程中擦除设备上的所有数据。尽管你不需要一个解锁的引导装载程序，但是当你处理 beta 版本时，保持引导装载程序解锁总是更好的。

随着 Android 12 的发布，谷歌开始提供“一个机会之窗”,在不擦除测试参与者设备的情况下从测试中注销:

> #### 当您为正在测试的版本应用稳定发布更新时，您可以在有限的时间内选择不进行数据擦除，直到您应用下一个测试更新。

服务器端交换将仅在测试周期结束时提供。由于还不清楚在新的预览版/测试版开始之前会有多少时间，这比手动取消注册更不可靠。

* * *

### 方法 2:手动降级

如果你不想等待谷歌发布回滚更新，那么你可以选择自己刷新最新的稳定的 Android 版本。但是，您需要一台 PC/Mac/Chromebook 来执行刷新操作。目标设备也需要解锁引导加载程序。

#### 使用 Android Flash 工具

谷歌的 [Android Flash 工具](https://www.xda-developers.com/google-android-flash-tool-project-treble-gsi/)(顾名思义)本质上是浏览器标签中的闪光器。得益于 [WebUSB API](https://wicg.github.io/webusb/) ，它通过将所有内容打包到一个 web 应用程序中，简化了刷新 Pixel 设备的整个过程。不需要下载映像、配置 CLI 平台工具、安装驱动程序和执行 Flash 命令——Android Flash Tool 可以完成所有工作。

1.  确保您的 PC/Mac/Chromebook 上安装了与 WebUSB UPI 兼容的浏览器。推荐使用基于 Chromium 的浏览器，如谷歌 Chrome 或微软 Edge。
2.  在目标 Android 设备上启用开发人员选项和 USB 调试(如果尚未完成)。
3.  将您的设备直接连接到 PC/Mac/Chromebook 的一个 USB 端口。
    *   避免 USB 集线器、适配器或扩展器，以避免潜在的错误。
4.  在你电脑上的浏览器中打开 flash.android.com。[](https://www.xda-developers.com/?attachment_id=666761)
5.  点击**开始**按钮。接下来，允许基于 web 的 flash 工具通过 ADB 与目标设备通信，方法是接受弹出窗口，该窗口显示**授权 Android Flash 工具访问其 ADB 密钥，以便它与连接的设备通信**。[](https://www.xda-developers.com/?attachment_id=666765)
6.  点击**添加新设备**。[](https://www.xda-developers.com/?attachment_id=666767)
7.  从列表中选择目标像素设备，点击**连接**。[](https://www.xda-developers.com/?attachment_id=666769)
8.  在你的 Pixel 屏幕上，选择**总是允许来自这台电脑**并点击**确定**接受 USB 调试连接。
9.  在浏览器中选择连接的设备。
10.  从列表中选择显示“返回公共”的构件。然后，您可以选择选项，如擦除设备、重新锁定引导加载程序或强制刷新所有分区。[](https://www.xda-developers.com/?attachment_id=666771)
11.  点击**安装构建**开始该过程。[](https://www.xda-developers.com/?attachment_id=666773)
12.  刷新过程完成后，断开设备与 USB 电缆的连接。

如果一切顺利，那么你的 Pixel 设备将重新启动到 Android 的最新稳定版本。它现在应该开始设备设置过程，允许您注册并享受稳定的 Android 软件。

#### 使用快速启动

如果您喜欢完全控制闪存操作，那么选择快速启动闪存方法。

1.  为您的 Pixel 智能手机下载最新稳定的 Android 工厂映像。对于 Android 12/12L，[看一下我们的下载指数](https://www.xda-developers.com/how-to-download-android-12/)。
2.  [使用快速启动](https://www.xda-developers.com/how-to-install-android-12/#method2)刷新工厂镜像。
3.  或者，重新锁定 Pixel 手机的引导程序:
    1.  恢复稳定的 Android 固件后，使用 ADB:

        ```
         adb reboot bootloader 
        ```

        将设备重新引导至引导加载程序模式
    2.  执行以下命令来重新锁定引导程序:

        ```
         fastboot flashing lock 
        ```

    3.  在你的 Pixel 手机上，使用音量键滚动到“锁定引导程序”选项，并使用电源按钮接受该选项。
    4.  手机将重新启动，并再次擦拭自己。

* * *

至于如何将你的谷歌 Pixel 智能手机从 beta/developer preview 降级到稳定的 Android 版本，这就是你需要知道的。你会选择回滚吗？在下面的评论区让我们知道你的理由吧！