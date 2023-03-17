# Pixel 7 系列上的 Google 张量 G2 从原始张量停止的地方开始

> 原文：<https://www.xda-developers.com/google-tensor-g2-changes/>

谷歌 Pixel 7 已经上市，随之而来的是一系列全面的显著改进。然而，最令人兴奋的改进之一来自芯片组的形式，因为它是任何智能手机的心脏。谷歌去年 Pixel 中的 Tensor 相当不错，尽管存在一些问题。这一次，该公司表示要在 Tensor G2 中改善电池寿命和其他方面，规格基本上是去年 Tensor 的迭代。

## 谷歌张量 G2:规范

| 

规格

 | 

谷歌张量 G2

 | 

谷歌张量

 |
| --- | --- | --- |
| **大核心** | 2 个 Cortex-X1 @ 2.85GHz | 2 个 Cortex-X1 @ 2.8GHz |
| **中芯** | 2 个 Cortex-A78 @ 2.35GHz | 2 个 Cortex-A76 @ 2.25GHz |
| **小核心** | 4x Cortex-A55 @ 1.8GHz | 4x Cortex-A55 @ 1.8GHz |
| **CPU L3 缓存** | 4MB | 4MB |
| **系统级缓存(SLC)** | 8MB | 8MB |
| **GPU** | ARM Mali G710 MP07 | 马里 G78 MP20 |
| **TPU** | 下一代定制边缘 TPU | 自定义边缘 TPU |
| **DSP** | 是 | 死后无子女。 |
| **ISP** | 10 位 HDRGoogle HDRnet108MP ZSL4K60 视频 | 8 位 HDRGoogle HDRnet4K60 视频 |
| **语境枢纽** | 是 | 是 |
| **安全** | 张量安全核心认证 M2 安全芯片 CPU 虚拟化可信操作系统在可信区域 5 年安全更新 | 张量安全核心认证 M2 安全芯片 CPU 虚拟化可信操作系统在可信区域 5 年安全更新 |
| **DRAM** | LPDDR5 | LPDDR5 |

## Google Tensor G2 在与 Tensor 相同的 CPU 公式上翻倍

比较这两种芯片组会发现许多相似之处，每组内核的基本功能都保留了下来。谷歌仍然保持其有点不正常的 2+2+4 设置，而是选择稍微缓冲大中型核心的时钟速度。理论上，这意味着谷歌将在任何使用两个线程处理的应用程序中拥有性能优势，尽管这取决于它节流的速度。

谷歌也将中间的内核提升到一对 A78 内核，这是一个非常受欢迎的变化。去年令人困惑的是，谷歌选择了一对 A76 内核，因为它们的能效和性能都比 A77 和 A78 差。这应该有望看到一些明显的性能和效率提升，从而延长电池寿命。

最后，和去年的张量一样，保留了四个小核。这里没有真正的变化。

总的来说，虽然看到完全升级到 Armv9(配有 Cortex X2、A710 和 A510 trio)会很好，但这将需要谷歌进行大规模的重新设计，特别是考虑到这是对已经是经过修改的 Exynos 设计的修改。也许明年？

## 谷歌张量 G2 的 GPU 有一个相当不错的升级

Google Tensor G2 在 GPU 部门进行了一次相当大的升级，从 Mali G78 MP20 升级到 Mali G710 MP07。Mali G710 MP07 与 Dimensity 9000 中的 GPU 类似，但可能会有一些修改，因为后缀是“MP07”。作为参考，联发科天玑 9000 有一个 Mali G710 MC10。很可能“7”指的是核心的数量(就像在原始张量的情况下一样)，但我们必须等等看。

然而，Mali G710 的改进不仅仅来自核心数量，而是来自实际结构本身。它承诺不仅在图形方面有重大改进，尤其是在 Vulkan 性能方面。我们需要等待，看看这些改进会有多少成果，但理论上，不仅在游戏和其他图形密集型任务中，甚至在像 [AetherSX2](https://www.xda-developers.com/aethersx2-playstation-emulator/) 这样的模拟器中，都应该有更好的性能。

上一次，张量中 G78 的 20 核怪兽虽然强大，但在开始减速前仅真正保留了几秒钟的功率。一开始，它保持高频率，但由此产生的高能耗和高热量是一个主要问题。看到谷歌把它调低一点，倾向于一个更正常的移动 GPU 配置，确实给了我们希望。

## 谷歌张量 G2 TPU 改进

谷歌正在宣传 Tensor G2 的 TPU 是“下一代”，在去年 Tensor SoC 已经令人印象深刻的基础上进行改进。去年，谷歌的张量芯片组在驱动程序中提到了“edgeTPU”。如果它是该公司在其云平台和 [Coral devices](https://coral.ai/products/dev-board/) 中宣传的同一款 Edge TPU，那么它只需 2W 的电源就能支持 4 TOPS。

在 Google Tensor G2 的例子中，Google 称 TPU 的功能和效率分别提高了 60%和 20%。这些都是相当大的改进，假设 TPU 的优势是一样的，已经很好了。它支持照片模糊和电影模糊等功能。

## 谷歌张量 G2 改善了基本面

谷歌张量 G2 看起来可能是一个非常好的芯片组，但我们不知道它是否足以改善张量去年下降的地方。我们仍然不太了解调制解调器及其功能，但有消息称它也有所改进。

我们期待着拿到张量 G2，看看这些改进实际上有多少成果。

 <picture>![The Pixel 7 packs the second-gen Tensor SoC, a brighter display, and improved cameras.](img/8b31c0e15e95c3f8bf719fbd3ebefc29.png)</picture> 

Google Pixel 7

Pixel 7 包含第二代 Tensor SoC、更亮的显示屏和改进的摄像头。

 <picture>![The Pixel 7 Pro is Google's top-of-the-line flagship of the year, featuring the second-gen Tensor SoC, a 120Hz LTPO display, a telephoto sensor, and a bigger battery.](img/26bf32dcd1e54473d448d9be3b56170c.png)</picture> 

Google Pixel 7 Pro

##### 谷歌 Pixel 7 Pro

Pixel 7 Pro 是谷歌今年的顶级旗舰产品，具有第二代张量 SoC，120Hz LTPO 显示屏，长焦传感器和更大的电池。