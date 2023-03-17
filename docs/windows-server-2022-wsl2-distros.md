# Windows Server 2022 现在支持 WSL2 Linux 发行版

> 原文：<https://www.xda-developers.com/windows-server-2022-wsl2-distros/>

微软宣布，现在可以在 Windows Server 2022 中运行基于 WSL2 的 Linux 发行版。这一变化在最新的累积版本中推出，使操作系统达到了[内部版本号 20348.740](https://support.microsoft.com/en-us/topic/may-24-2022-kb5014021-os-build-20348-740-preview-2b180bd4-dceb-4c49-b8cf-402b342ebc84) ，尽管官方变更日志中没有提到这一变化。微软的 Craig Loewen 证实，在 GitHub 的评论中添加了对 WSL2 的支持，这是为了回应对 Windows Server 2022 中缺乏对它的支持的持续关注。

for Windows Subsystem for Linux 2 的简称)于 2019 年 5 月首次公布，并于 2020 年上半年发布的 Windows 10 版本 2004 中首次发货。当时微软也是通过半年更新来支持 Windows Server，就像 Windows 10 一样，只有运行 Windows Server 半年通道的用户才获得对 WSL2 的支持。如果你用的是 Windows Server 2019，那你就没那么幸运了。

去年，微软停止了 Windows Server 的半年期渠道，并回到了主要版本，如 [Windows Server 2022](https://www.xda-developers.com/windows-server-2022-available-new-security-features/) 。然而，就像 Windows Server 2019 一样，这个新版本仍然不包括对 WSL2 的支持。现在，差不多一年过去了，它终于来了。

如果你想知道为什么这可能是一件大事，实际上有很多。有了 WSL2，微软开始为 Windows 提供一个完整的 Linux 内核，并允许完整的系统调用兼容性。此外，Linux 发行版比基于 WSL 原始版本的发行版具有更好的性能。Linux 现在运行在一种虚拟机(VM)中，但它被设计成比传统 VM 更轻量级和更自然的体验。

如果你运行的是 Windows Server 2022，并且想使用 WSL2 Linux 发行版，你可以从 Windows Update 获取最新的更新(你需要手动寻找)，或者你可以[在这里](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5014021)下载。如果你不着急的话，这个改动将会包含在下一个星期二的更新中，也就是 6 月 14 日。

* * *

来源:[克雷格·勒文(GitHub)](https://github.com/microsoft/WSL/issues/6301#issuecomment-1136453235)