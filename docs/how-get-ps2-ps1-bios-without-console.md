# 如何在没有主机的情况下获得 PlayStation 1 或 PlayStation 2 BIOS

> 原文：<https://www.xda-developers.com/how-get-ps2-ps1-bios-without-console/>

# 如何在没有主机的情况下获得 PlayStation 1 或 PlayStation 2 BIOS

如果你想模仿 PS2 或 PS1 的游戏，你需要一个 BIOS。这里有一个快速简单的方法来合法地得到一个。

对许多人来说，PlayStation 2 是一款怀旧的游戏机，但模仿它可能会很困难。如果你不修改你的主机并抛弃 BIOS，你将无法通过像 [AetherSX2](https://www.xda-developers.com/aethersx2-playstation-emulator/) 这样的游戏来模拟游戏。现在，事实证明，只需一点点工作，就可以从官方 PS3 固件中下载并提取 BIOS。

这些步骤是为 Windows 编写的，但是它们在 Linux 上也非常相似。这很重要，因为从 PS2 转储 BIOS 需要类似 FreeMcBoot 的东西，但转储游戏可以用 PC 上大多数传统的光盘阅读器来完成。

## 你需要什么

*   **互联网连接**:你需要互联网来下载 PS3 模拟器和 PS3 固件文件，除非你想从 PS3 光盘上下载。
*   **RPCS3** : RPCS3 是一款开源的 PlayStation 3 模拟器，可以让你从固件中提取 PS2 BIOS 文件。
*   一个 PS3 固件 PUP 文件:你可以[从索尼](https://www.playstation.com/en-ie/support/hardware/ps3/system-software/)下载这个。
*   **固件 BIOS 声明**:你可以从[互联网档案](https://archive.org/details/firmware_bios_claim_release1)下载。

## 步骤 1:安装 RPCS3 并下载 PS3 固件

你需要下载 RPCS3 并安装到 PlayStation 3 固件中，其中包含执行 PS1 和 PS2 游戏所需的 BIOS 文件。仿真器将允许我们与固件进行交互，并提取那些文件。

1.  安装 **RPCS3** 并下载你的 PS3 固件。
2.  点击左上方的**文件**，选择**安装固件**。
3.  导航到 **PS3UPDAT。PUP** 文件。

## 步骤 2:运行固件 BIOS 声明

这部分将从 PS3 固件中提取实际的 BIOS 文件。

1.  关闭 RPCS3 并解压缩固件 BIOS 声明 zip 文件。
2.  将**firmware _ BIOS _ claim . bat**和**firmware _ BIOS _ claim . PS1**复制到您的 RPCS3 文件夹中。
3.  运行**firmware _ BIOS _ claim . bat**然后点击**仍然运行**。
4.  在 Linux 上，改为复制 **firmware_bios_claim.sh** 文件并在文件夹中执行。
5.  如果有效，您应该会看到以下内容。

## 步骤 3:将 BIOS 文件复制到您选择的设备上

您的 BIOS 文件现在应该在 RPCS3 文件夹中。

你可以用 PS1 的 BIOS 来运行 [DuckStation](https://www.xda-developers.com/duckstation-playstation-1-emulator/) ，用 PS2 的 emu BIOS 来运行 AetherSX2 这样的仿真器。您可能需要启用快速启动来启动游戏，但这是为 PlayStation 1 或 PlayStation 2 获取工作 BIOS 以进行仿真的一种快速而简单的方法。

* * *

来源: [EZOnTheEyes](https://www.youtube.com/watch?v=gah74XQcezc)