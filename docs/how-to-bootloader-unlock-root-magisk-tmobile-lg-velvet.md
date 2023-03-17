# 如何 bootloader 解锁 T-Mobile LG Velvet 并用 Magisk root

> 原文：<https://www.xda-developers.com/how-to-bootloader-unlock-root-magisk-tmobile-lg-velvet/>

解锁引导程序、[给设备找根](https://www.xda-developers.com/root/)和刷新售后光盘是 XDA 这里流行的爱好。超级用户群体非常重视修改他们设备的能力，如果他们不能解锁引导程序，他们几乎不会对手机感兴趣。许多传统设备实际上是由第三方 rom 保持活力的，这对站在失去官方支持边缘的智能手机来说也是天赐之物。例如，LG 不再生产 Android 智能手机，因此 LG 设备的所有者可能希望在不久的将来使用[定制 rom](https://www.xda-developers.com/most-popular-custom-roms-android/)。然而，由于 LG 的引导加载程序解锁政策，这个过程并不简单。

LG 在引导加载程序解锁方面有着传奇的历史。韩国原始设备制造商过去只允许少数型号被最终用户解锁——可能是由于运营商的要求。尽管如此，[公司在几个月前永久地抓住了这个机会](https://www.xda-developers.com/lg-bootloader-unlocking-shut-down-december-31/)，这意味着人们不得不依靠非官方的方法来解锁他们的引导程序。这一次，XDA 资深成员 [Wish39](https://forum.xda-developers.com/m/wish39.6328729/) 提出了一个真正创新的过程来解锁 LG Velvet 的 T-Mobile 变种的引导加载程序，并随后对设备进行 root。

*   你现在可以非正式地解锁 LG Velvet 的 T-Mobile 变种的引导程序了。
*   这个过程需要降级到 Android 10。
*   解锁引导程序后，您可以使用 Magisk 来引导设备。

## 如何 bootloader 解锁并 root T-Mobile LG Velvet

LG Velvet 的 T-Mobile 版(型号 LM-G900TM)搭载的是联发科天玑 1000C SoC。这使得它在 Velvet 系列中独一无二，因为所有其他智能手机都采用高通骁龙 750G (5G)或骁龙 845 (4G)芯片组。前面提到的联发科平台容易受到[已知 bootrom 漏洞](https://www.xda-developers.com/bypass-mediatek-sp-flash-tool-authentication-requirement/)的攻击，该漏洞可被用来绕过引导加载程序安全并解锁引导加载程序。之后，对设备进行 root 是一件轻而易举的事情。

在我们进入如何扎根 T-Mobile LG Velvet 之前，记得进行设备外备份。这是因为引导加载程序解锁过程**需要擦除你手机上的每一条个人数据，包括内部存储器上的文件**。

### 第一步:降级到 Android 10

万一目标 T-Mobile LG Velvet 运行的是 Android 11，我们需要将其降级到 Android 10。这是因为该设备的 Android 11 固件已经修补了可利用的预加载程序(又名第一阶段引导加载程序)。你还需要一台电脑，因为 flash 工具只能在 Windows 下工作。

1.  [下载并安装 LG 最新的 USB 驱动](https://www.xda-developers.com/download-android-usb-drivers/)。
2.  从一个著名的 LG 固件托管网站下载任何基于 Android 10 的 KDZ 固件包。
3.  下载一个正确修补的 LGUP 工具来刷新 KDZ 包。
4.  安装 LGUP 并打开其可执行文件。
5.  选择**整修**选项作为流程。接下来，点击右下角有三个点的按钮来选择 KDZ 文件。
6.  重启 LG Velvet 至下载模式。为此，请关闭您的手机。接下来，将 USB 电缆插入您的 PC，按住电话的音量增加按钮，并将电缆的另一端连接到电话。你应该会看到一个屏幕上的文字“固件更新”旁边的手机上的 USB 标志。
7.  点击**开始**按钮，等待刷新过程结束。
8.  如果一切顺利，手机将重启至 Android 10 固件。

### 步骤 2:解锁引导加载程序

现在我们已经恢复了 T-Mobile LG Velvet 上的可利用预加载程序，我们可以在瞬间解锁它的引导加载程序。由于安全分析师 Bjoern Kerler 的 MTKClient 项目，您不必关心漏洞有效载荷和其他低级逆向工程工具。您需要做的就是执行几个 Python 脚本。

1.  从其官方 GitHub repo[下载 MTKClient 工具，并按照自述文件进行设置。](https://github.com/bkerler/mtkclient)
2.  确保手机关机。接下来，在 PC 的终端窗口中运行以下命令，然后将电话插入 PC。这将删除你手机上的`metadata`和`userdata`分区
3.  在这个阶段，我们准备执行解锁命令

    ```
     python mtk xflash seccfg unlock 
    ```

4.  使用以下命令重启手机:

    ```
     python mtk reset 
    ```

    接下来，断开 USB 电缆让手机重启。
5.  现在你有了一个 bootloader 解锁的 T-Mobile LG Velvet。

### 第三步:升级到 Android 11

由于引导程序现在已经解锁，我们可以(重新)升级到 Android 11 固件。然而，直接刷新 Android 11 KDZ 将取代可利用的预加载程序，因此我们需要选择选择性刷新程序。

1.  为 T-Mobile LG Velvet 下载最新的 Android 11 KDZ。
2.  打开 LGUP 并选择 KDZ。
3.  启动手机到下载模式，并将其连接到您的电脑。
4.  选择**分区 DL** 选项，点击**开始**按钮。
5.  当你看到分区列表窗口时，点击**全选**并取消预装分区，然后按 OK 开始刷新。
6.  在完成闪烁过程后，手机应该会使用解锁的引导程序引导到 Android 11。

### 步骤 4:使用 Magisk 为 root 用户修补普通引导映像

解锁的引导加载程序允许我们在设备上运行未签名的代码。因此，我们现在可以使用 Magisk 修补股票引导映像，并刷新修改后的映像以获得 root 访问权限。

1.  使用 MTKClient 将股票启动映像从手机转储到 PC [。](https://github.com/bkerler/mtkclient#read-flash)
2.  将转储的图像复制到您的手机，并使用 Magisk 对其进行修补。然后将修补后的图像从手机复制到 PC。
3.  使用 ADB:

    ```
     adb reboot fastboot 
    ```

    将手机重启至引导程序界面
4.  使用 Fastboot:

    ```
     fastboot flash boot name_of_the_patched_boot_image.img 
    ```

    刷新 Magisk 修补的引导映像
5.  重启手机。
6.  这就是让你的 T-Mobile LG Velvet 扎根所需要的一切。

### 下一步是什么？

目前在我们的 T-Mobile LG Velvet 论坛上没有 TWRP 的版本或者任何定制的 rom。尽管如此，一个解锁的引导程序允许你玩不同的 GSI 版本。作为根用户，你将能够利用大量的根应用程序和 Magisk 模块，这允许你改变你设备的不同方面。

如果你想了解更多关于这个过程的细节，请查看我们论坛中的以下帖子:

**[T-Mobile LG Velvet 的 Bootloader 解锁和 Root(仅限 g 900 TM)](https://forum.xda-developers.com/t/4458055/)**