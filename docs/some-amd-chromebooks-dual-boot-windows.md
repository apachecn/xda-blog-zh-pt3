# 一些 AMD 驱动的 Chromebooks 现在可以双启动 Windows 11

> 原文：<https://www.xda-developers.com/some-amd-chromebooks-dual-boot-windows/>

如果你一直想在 Chromebook 上安装 Windows 10 或 Windows 11，今天有一些潜在的好消息给你。由于 Reddit 用户 Coolstarorg 的工作，现在可以在 AMD 锐龙 3000 系列处理器支持的部分 Chromebooks 上双启动 Windows 10 或 11 以及 Chrome OS。有一些限制，但在大多数情况下，Windows 应该可以在这些机器上很好地工作。

目前，只有很少的设备受到支持，这主要是因为在 Chromebook 上双启动 Windows 时，eMMC 存储还不能正常工作。你需要一台配备固态硬盘的笔记本电脑，官方只支持三种设备:惠普 Chromebook 14b、惠普 Chromebook Pro C645 Enterprise 和联想 Yoga C13。华硕 Chromebook Flip CM5 应该也支持，但是这个项目的创建者还没能测试出来。

除了 eMMC 存储无法工作——Windows 可以读写，但 UEFI 无法启动——唯一无法工作的其他功能是指纹识别器。您将无法使用 Windows Hello 登录到 Windows，这可能会有问题，但可能不会导致交易中断。除了这两个功能之外，包括音频、触摸屏、亮度控制、电源管理等在内的一切都应该可以在 Windows 上正常工作。

至于它是如何工作的，这并不是什么新鲜事。你首先需要使用 chrx 对 Chrome 操作系统进行重新分区，chrx 是一种在 Chromebooks 上双启动 Linux 的流行工具。然后，使用 MrChromebox 提供的[脚本更新 PC 上的 RW_LEGACY 固件，最后，使用 coolstarorg 创建的脚本设置双引导。你可以访问这个页面，获得如何在 Chromebook 上双启动 Windows 的完整指南，前提是你的型号受支持。各种基于英特尔的 Chromebooks 也支持这种方式的 Windows 双启动，而不仅仅是新加入的 AMD。](https://mrchromebox.tech)

我们应该注意到，虽然你*可以*这样做，但我们想不出你想要这样做的好理由。如果你对运行 Windows 感兴趣，首先你可能会买一台 Windows 笔记本电脑，当你采取这些步骤时，总有可能会出错。此外，Chrome 操作系统的一大优点是，它可以在搭载它的设备上无缝运行，这在 Windows 上并不常见。如果你真的想在 Chrome OS 上运行 Windows 应用程序，还有像 [Parallels Desktop](https://www.xda-developers.com/parallels-desktop-chrome-os-now-supports-amd-ryzen-processors/) 这样的虚拟化软件。不过，如果你想尝试一下，你现在有这个选择。

* * *

来源:[酷星组织(Reddit)](https://www.reddit.com/r/chrultrabook/comments/vt7bsf/windows_10_and_11_now_available_for_amd_ryzen/)