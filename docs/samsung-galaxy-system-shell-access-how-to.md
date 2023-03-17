# 如何在任何三星 Galaxy 设备上访问系统外壳

> 原文：<https://www.xda-developers.com/samsung-galaxy-system-shell-access-how-to/>

每个月的第一个星期一，谷歌都会发布 [Android 安全公告](https://www.xda-developers.com/how-android-security-patch-updates-work/)。它披露了 Android 操作系统各种组件以及 Linux 内核的所有已缓解的安全漏洞，以及谷歌自己或其他第三方迄今提交的补丁。像三星这样的大型原始设备制造商对 Android 有自己的看法，所以他们也选择将自己的补丁和更新纳入安全更新。

也就是说，很难处理好每一个漏洞。存在过多的攻击媒介，有时您可以基于以前已知的漏洞来构建自己的利用链，因为您有一种新方法来规避其中一种安全措施。这正是 XDA 资深成员 [K0mraid3](https://forum.xda-developers.com/m/k0mraid3.11993791/) 利用一个四年之久的漏洞所做的事情，该漏洞允许他获得所有三星 Galaxy 设备的系统外壳访问权限——包括最新的旗舰设备。虽然这与[拥有根权限](https://www.xda-developers.com/root/)不同，但这是足够高的本地权限升级。

该漏洞的主要入口点位于三星文本到语音(包名:com.samsung.SMT)中，这是一个预装的系统应用程序，可以在每台三星 Galaxy 设备上找到。其思路是将已安装的 app 版本降级为特定的易受攻击的 build(准确的说是 **v3.0.02.2** )，然后强制其加载一个库，进而打开一个具有系统权限(UID 1000)的 shell。

如果你想了解更多关于这个漏洞的信息，一定要查看 XDA 首席技术编辑亚当康威的解释。他采访了 K0mraid3，以便全面了解这种利用的范围以及它是如何工作的。

1.  重申一下，这不是 root (UID 0)访问，但是系统 shell 访问足够强大，可以执行一堆其他方面受限的二进制文件。
2.  K0mraid3 的概念验证需要一个助手 APK，您需要在启动漏洞链之前至少运行它一次。
3.  一个 UI，即三星的定制 Android 皮肤的内置节能例程可能会很麻烦，因为它们可能会妨碍 TTS 应用程序、助手 APK 和 shell 之间的通信。因此，我们建议预先将应用程序的省电模式设置为“无限制”。

## 先决条件

1.  从 [XDA 论坛线程](https://forum.xda-developers.com/t/4543071/)或下面链接的官方 GitHub 库下载漏洞利用的预编译版本: **[K0mraid3s 系统外壳漏洞利用](https://github.com/k0mraid3/K0mraid3s-System-Shell-PREBUILT/releases/latest)**
2.  解压存档文件，你应该会发现三星文本到语音转换 APK (samsungTTSVULN2.apk)的漏洞版本，助手应用程序(komrai3s _ POC _ VX . x . apk)，以及一个名为 systemshell-vx.x.exe 的 Windows 可执行文件。
3.  确保你的 PC/Mac/Chromebook 上安装了最新版本的 [ADB](https://www.xda-developers.com/install-adb-windows-macos-linux/) 。另外，如果你是 Windows 用户，记得[安装/更新三星 USB 驱动程序](https://www.xda-developers.com/download-android-usb-drivers/)。

## 如何利用任何三星 Galaxy 设备获取系统外壳访问权限

### 手动方法

1.  打开 USB 调试，将目标 Galaxy 设备连接到您的 PC，确保它可以被 ADB 发现，然后安装助手应用程序。

    ```
    adb install Komraid3s_POC_Vx.x.apk
    ```

    *   如前所述，在进行下一步之前，至少打开助手应用一次。

2.  现在将三星 TTS app 的漏洞版本推送到/data/local/tmp 并更改权限:

    ```
    adb push samsungTTSVULN2.apk /data/local/tmp
    ```

    ```
    adb shell chmod 777 /data/local/tmp/samsungTTSVULN2.apk
    ```

3.  重启设备。一旦你进入主屏幕，运行以下命令，用有漏洞的版本替换已经安装的 Samsung TTS 应用程序版本:

    ```
    adb shell pm install -r -d -f -g --full --install-reason 3 --enable-rollback /data/local/tmp/samsungTTSVULN2.apk
    ```

    *   如果一切正常，那么您应该会在控制台上看到一条“成功”消息。

4.  通过打开另一个终端窗口并执行 **adb shell** 在目标设备上打开一个 shell，然后执行 Netcat 二进制文件，并使用以下命令在 9997 端口上侦听传入的连接:

    ```
    adb shell nc -lp 9997
    ```

5.  在这个阶段，我们需要执行三星 TTS 应用程序的一个特定活动，它将为我们打开系统外壳。
6.  切换回第一个 shell，您应该会看到一个具有 system (UID 1000)权限的新提示符。

### 自动化方法

为了使事情变得更简单，K0mraid3 还提供了一个易于使用的 GUI 应用程序来自动化大多数任务。请记住，GUI 应用程序只适用于 Windows，所以如果你是 Linux/macOS 用户，最好坚持使用手动方法。

1.  在 USB 调试打开的情况下，将目标 Galaxy 设备连接到您的 PC，确保它可以被 ADB 发现，然后安装助手应用程序。

    ```
    adb install Komraid3s_POC_Vx.x.apk
    ```

    *   如前所述，在进行下一步之前，至少打开助手应用一次。

2.  ADB 发现目标设备后，在主机上运行 systemshell-vx.x.exe。
3.  单击“启动 SHELL”按钮。该应用程序会自动降级三星 TTS 应用程序，并尝试打开系统外壳。
    *   在您的手机/平板电脑上，您可能会看到 TTS 应用程序提示您下载一些语音数据。没有必要与这些选项进行交互，因为它们与攻击没有任何关系。
    *   如果应用程序在一段时间后挂起或无法打开 shell 窗口，请关闭它，重新启动目标 Galaxy 设备，然后重新开始。
    *   Galaxy Store 应用程序可以在后台自动更新和/或重置 TTS 应用程序的节能配置文件，因此请确保在从头开始该过程之前检查它。

## 确认

一旦获得了 shell 访问权限，就可以使用下面的命令之一来验证特权级别:

```
    whoami
    ```

    *   输出应该是“系统”

```
    id -u
    ```

    *   输出应该是“1000”

## 结论

在 Android 设备上实现 root 访问的典型方法是首先解锁引导加载程序，这允许您引导第三方二进制文件。由于 Android 的安全模型基本上与 root 分崩离析，这一步是有意禁用设备上的一个关键安全功能，这就是为什么用户必须通过通常在开发者选项中启用切换，然后向引导加载程序发出解锁命令来明确允许这种情况发生。一旦 bootloader 解锁，用户可以向系统引入一个超级用户二进制文件和一个超级用户管理应用程序(如 Magisk)来控制哪些进程可以访问 root。

但是，利用上面提到的系统外壳漏洞，用户不必解锁引导加载程序就可以获得提升的权限。尽管它远不是根用户，但“系统”用户有足够的能力访问许多低级分区(如/efs)，启动各种服务和调试工具，并更改许多受保护的属性值——所有这些甚至都不会影响 Knox。这些例子只涉及到几个方面；恶意行为者可以将这一点与其他漏洞结合起来，想出更加邪恶的行动。

我们将拭目以待谷歌和三星如何应对这一局面。无论哪种方式，你都应该暂时禁用或删除三星的文本到语音转换应用程序。