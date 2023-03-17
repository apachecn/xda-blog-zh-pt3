# Android 的 Windows 子系统为内部人员提供 IPv6 和 VPN 支持

> 原文：<https://www.xda-developers.com/windows-subsystem-android-ipv6-vpn-av1-support/>

# Android 的 Windows 子系统为内部人员提供 IPv6 和 VPN 支持

微软正在推出对 Android Windows 子系统的更新，支持 IPv6 和 VPN 连接，并增加了更多改进。

微软正在为所有渠道的 Windows Insiders 推出针对 Android 的 Windows 子系统的新更新，使其版本达到 2205.40000.14.0。通过此次更新，Android 的 Windows 子系统现在支持 IPv6 和 VPN 连接，扩展了 Windows 上 Android 应用程序的网络功能。如果你想绕过地区限制，或者如果你有要求你使用公司 VPN 的 Android 应用，VPN 支持是特别有趣的。然而，微软确实注意到一些 VPN 可能还不能正常工作。

这个月的另一个变化是高级网络功能，这些功能是在之前的更新中引入的，现在也在 Arm 设备上得到支持。这些功能允许 Android 应用程序访问与您的电脑位于同一本地网络上的设备，这对于联网打印机或智能家居设备非常有用。Android 设置应用的 Windows 子系统也已更新，以适应这一点，这意味着你将不再看到你的 IP 地址。这是因为 Android 子系统的 IP 地址与您的 PC 的 IP 地址相同，因此您可以始终将它用于相同的目的。

这次更新还增加了对 AV1 视频编解码器的支持，这意味着你应该能够在 Android 应用程序中播放更多类型的视频。它还包括 Chromium WebView 的更新，现在版本为 101，它为 Android 打包了 5 月份的内核补丁，增强了子系统的安全性。完整的变更日志如下:

*   支持高级网络功能，包括应用程序访问 ARM 的本地网络设备
*   虚拟机 IP 地址已从设置应用中删除。借助高级网络，现在虚拟机的 IP 地址与主机/计算机的 IP 地址相同。
*   最大化或调整大小时不可调整大小的应用程序内容的修复
*   修复了应用程序中使用鼠标和触控板滚动的问题
*   安卓 5 月内核补丁
*   标记为安全的 Android 窗口不能再截图了
*   改进网络浏览器启动
*   充电时启用打盹和应用待机，以提高省电效率
*   ADB 调试提示重定向到 Windows 以提高安全性
*   更新至 Chromium WebView 101
*   修复了图形问题，包括应用程序闪烁和图形损坏
*   视频播放的修复
*   AV1 编解码器支持
*   启用 IPv6 和 VPN 连接
*   提高了连接到集装箱中虚拟 WIFI 的性能和可靠性
*   视频播放应用程序现在可以在 Windows 中阻止屏幕关闭

像大多数其他微软商店应用一样，Android 的 Windows 子系统会自动更新，但如果你不想等待，你可以打开微软商店，然后前往**库** - > **获取更新**来更新你的所有应用。目前，这一功能仅适用于地区设置为美国的个人电脑，但微软[计划在年底前在另外五个市场](https://www.xda-developers.com/android-apps-windows-11-coming-europe-japan/)推出 Android 应用支持。

* * *

来源:[微软](https://blogs.windows.com/windows-insider/2022/07/06/update-to-windows-subsystem-for-android-on-windows-11-july-2022/)