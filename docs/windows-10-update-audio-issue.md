# 微软回滚导致声音问题的 Windows 10 更新

> 原文：<https://www.xda-developers.com/windows-10-update-audio-issue/>

微软在 7 月份首次测试了 Windows 10 系统的可选补丁,然后在 8 月 9 日推出了其中的一些变化，作为每月更新。然而，事实证明，7 月份的原始补丁弊大于利。虽然 KB5015878 更新旨在修复多[显示器设置](https://www.xda-developers.com/best-monitors/)的错误，以及视频播放的问题，但该公司后来更新了 Windows Health Dashboard，以提及更新 KB5015878 现已被回滚，因为它一直在用音频创建问题。

根据微软的说法，安装此更新或更高版本后，一些 Windows 10 系统可能会静音并不播放音频，而其他 Windows 10 系统可能会在某些端口或某些应用程序内不输出音频。大多数受影响的 Windows 10 系统在安装更新之前也禁用了“音频增强”设置。Microsoft 发布了一个已知问题回滚来防止此更新的传播，但如果您已经安装了它，您可能仍然有问题，并需要遵循一些官方的解决方法。

现在，如果你受到影响，你可以做一些事情。请注意，只有运行 Windows 10 版本 20H2、21H1 和 21H2 的系统才会受到此 bug 的影响。Windows 11 还没有受到这个问题的影响。

首先，如果您尚未安装此更新，您可以通过检查 Windows Update 来更新您的音频驱动程序，以帮助防止问题发生。在另一种情况下，如果您安装了更新，并且如果只有某些应用程序不播放音频，您可以尝试确保选择了正确的音频输出。

最后，如果你已经安装了更新，你可以通过运行 Windows 音频故障诊断程序，在 Windows 10 搜索框中搜索它，或者通过[跟随微软自己的自助教程](https://support.microsoft.com/windows/fix-sound-or-audio-problems-in-windows-73025246-b61c-40fb-671a-2535c7cd56c8)，来尝试恢复音频。微软建议的最终解决方案包括遵循微软关于[禁用音频增强](https://support.microsoft.com/topic/disable-audio-enhancements-0ec686c4-8d79-4588-b7e7-9287dd296f72)的指南。进入*开始* > *设置* > *系统* > *声音，可以在*附加设备属性*下找到音频增强设置。*这两种解决方法都相对简单，完成时间不会超过几分钟。

* * *

来源:[微软](https://docs.microsoft.com/en-us/windows/release-health/status-windows-10-21h2#2887msgdesc)