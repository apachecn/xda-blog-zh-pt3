# 蒸汽甲板上的质子是如何工作的

> 原文：<https://www.xda-developers.com/how-proton-on-the-steam-deck-works/>

如果你有一个 [Steam Deck](https://www.xda-developers.com/steam-deck-review/) ，你可能会惊讶于许多游戏在上面运行得如此之好。它不仅是一款掌上电脑，还是一款运行 Linux 的掌上电脑。尽管该操作系统在运行视频游戏方面名声不佳，但诸如*赛博朋克:2077* 和*侠盗猎车手:V* 等 AAA 游戏在 Steam 平台上运行得非常好。这要归功于 Proton，这是 Valve 和 CodeWeavers 开发的兼容层。

## 质子是什么？它是如何工作的？

Proton 其实比 Steam Deck 早几年，Steam Deck 最早发布于 2018 年 8 月。当时，Valve 表示，“目前没有 Linux 版本的 Windows 游戏现在可以直接从 Linux Steam 客户端安装和运行，并提供原生 Steamworks 和 OpenVR 支持。”

在 Proton 之前，Linux 上的游戏玩家通常需要游戏的本地端口，或者被迫依赖第三方兼容层，如 Wine。Wine 运行得相当好，但往往需要大量的调整才能让事情完美运行，像 *DOOM (2016)* 这样的游戏只需一点点努力就可以玩了。

这就是质子的用武之地。它消除了最终用户方面的任何工作需求。这个想法是，你只需安装游戏，就像在本地运行一样，最终用户不需要知道游戏中发生了什么。

质子工程与葡萄酒的修改版本。Wine 作为一个层，将 Windows API 调用转换为 POSIX(可移植操作系统接口)调用，同时重新创建 Windows 目录结构，并提供系统服务的替代实现。Wine 不使用任何仿真或虚拟化来执行 Windows 二进制文件。

质子的另一个重要部分是它翻译 Direct3D API 调用的能力。它包括 DXVK，一个基于 Vulkan 的 Direct3D 9、10 和 11 的翻译层，并通过 VKD3D-Proton 提供对 Direct3D 12 的支持，VKD3D-Proton 是 Wine 的 VKD3D 的一个分支。

至于 Direct3D，它是一个用于 Windows 机器的图形 API，是 DirectX 的一部分，Proton 本质上解释了这些 Direct3D API 调用。质子创造了自己的版本，游戏可以与这个库接口。然后，Proton 在内部将这些调用路由到 Vulkan API，允许游戏像在 Windows 机器上一样运行。

质子是完全开源的，Valve 称这将“使高级用户能够改变质子”最受欢迎的定制质子构建是[质子-GE](https://github.com/GloriousEggroll/proton-ge-custom) ，它包含了最近的质子实验变化。它还包含其他常规质子没有的补丁和功能。

## 质子的未来

质子可以一直工作和改进，但就其现状而言，它已经是一个成熟和发达的项目。随着大量的游戏已经可以通过它来玩，游戏玩家没有更多的要求了。仍然有一些兼容性问题和图形故障出现，但总的来说，通过质子播放与在 Windows 上播放没有什么区别。

Valve 接下来绝对可以关注的一件事是，将 Proton 所基于的 Wine 版本升级到一个更新的版本。Proton 落后于最新的官方 Wine 版本几个版本，而 Proton-GE 等开源社区项目旨在为最新版本的 Wine 添加更多功能和基础。

当然，Valve 的最终目标是稳定性和兼容性，这就是为什么它不仅仅包括质子-GE 等项目已经能够实现的所有这些变化。如果你是一个超级用户，那么没有什么可以阻止你安装和使用 Proton-GE，但对于日常游戏玩家来说，稳定的 Proton 肯定是更好的选择。