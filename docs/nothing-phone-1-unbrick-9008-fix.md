# 如何使用 EDL 闪光解除你的一无所有的手机 1

> 原文：<https://www.xda-developers.com/nothing-phone-1-unbrick-9008-fix/>

凭借其独特的发光通知“字形”和玻璃铝设计， [Nothing Phone 1](https://www.xda-developers.com/nothing-phone-1-review/) 无疑是市场上最漂亮的智能手机之一。制造商也已经接受了 XDA 的售后开发商社区。除了现成的内核源代码，你可以很容易地解锁手机的引导程序，这意味着对于一无所有的手机 1 来说，进入修改场景是相当无缝的。

## 救命啊！我的电话打不开

然而，修改你的设备并不是没有风险的，它甚至会导致你暂时屏蔽你的手机。如果您不想去服务中心或把您的手机送到服务中心，而是想让您的手机起死回生，您需要找到一个合适的闪存工具，它可以使用 SoC 专用的低级闪存协议与设备通信。采用高通骁龙芯片组的设备具有一种称为**E**emergency**D**own**l**oad Mode(EDL)的替代引导模式，该模式严格用于 OEM 服务。现在你终于可以利用这种模式来恢复你的设备。

XDA 资深成员 mark332 将所有需要的软件包放在一个地方，并设计了一个方便的 GUI，这样你就可以用它来恢复你一无所有的手机 1，甚至从一块硬砖。该工具需要 Windows，尽管从技术上讲，如果您设法获得合适的高通 flash 二进制文件，您也可以在 Linux 上使用它。

## 如何取消无手机 1

与谷歌不同，Nothing 没有为与 Nothing Phone 1 对应的工厂图像维护一个官方门户。当然，你可以从我们的[Nothing Phone 1 update tracker](https://www.xda-developers.com/nothing-phone-1-nothing-os-update-tracker/)中手动抓取 OTA 包，但是当你甚至无法访问引导程序/快速引导模式，并且遇到类似这样的情况时，这不足以恢复你的设备:

幸运的是，你可以通过组合键强制手机 1 进入 EDL 模式。只要确保目标设备完全关闭，然后在将手机插回 PC 时按住音量增大和音量减小按钮。您还需要一根经过修改的 USB 电缆来强制设备启动到 EDL 模式。

万一上面的方法不行，你就得把手机拆开，短接两个测试点。如果一切正常，手机此时应该会启动到 EDL 模式，这可以通过在设备管理器下搜索新的“高通 HS-USB QDLoader 9008”条目(或“QHUSB_BULK”，如果驱动程序没有正确安装)来轻松验证。

值得注意的是，当 Android 启动时，`adb reboot edl`命令应该足以引导手机进入紧急下载模式，但对于硬砖场景来说，这是没有用的。

现在，您的电脑可以在 EDL 模式下识别手机，我们可以进入下一阶段。要刷新设备，请执行以下操作:

1.  [从 mark332 的线程](https://forum.xda-developers.com/t/4552471/)下载 flashing 工具。
2.  在路径短且没有任何空格的地方打开 flash 工具的包装(例如 D:\unbricktool)。
3.  确保无电话 1 通过虚拟 COM 端口以 QDLoader 9008 模式连接到 PC。
4.  启动 unbricktool.exe 并检查它是否在右上角列出了相同的 COM 端口。
5.  选择“固件刷新”，点击“开始”，然后等待该过程完成。
6.  手机应该重新启动到一个完全正常的操作系统环境。

该工具将完全擦除你的手机在闪烁的过程中。它还会(重新)锁定目标设备的引导加载程序。鉴于你可以轻松地再次解锁，这并不是什么大不了的事情，但仍然值得注意。

## 下一步是什么？

请记住，EDL 软件包是基于 Nothing OS 1.1.7，而不是最近发布的基于 Android 13 的 [Nothing OS 1.5.2。也就是说，手动](https://www.xda-developers.com/nothing-phone-1-stable-android-13-nothing-os-1-5-2/)[侧载 Nothing OS 更新](https://www.xda-developers.com/how-to-sideload-nothing-os-ota-updates-on-nothing-phone-1/)非常容易，所以你可以在解锁手机后立即获得最新的固件，而无需等待一系列 OTA。

由于几乎不受限制的低级别访问，该工具足够强大，可以读回分区内容，备份 IMEI 和类似的唯一标识符，更改区域，等等。因此，只有在你知道自己在做什么的情况下才尝试修补。

**[无事电话 1 XDA 论坛](https://forum.xda-developers.com/f/nothing-phone-1.12585/)**

* * *

**来源** : XDA 论坛( [1](https://forum.xda-developers.com/t/4552471) 、 [2](https://forum.xda-developers.com/t/4552965/) )