# 苹果 M1 Pro vs M1 Max:这里是你需要知道的一切

> 原文：<https://www.xda-developers.com/deep-dive-apple-m1-pro-max/>

苹果公司的 M1 SoC 开始从基于 x86 的芯片转型。第一代 Mac 芯片在许多方面震撼了行业，并因其令人印象深刻的性能和一流的能效赢得了众多赞誉。M1 芯片是一个良好的开端，但这不足以帮助苹果争取更大的份额。嗯，随着新的 [M1 Pro 和 M1 Max](https://www.xda-developers.com/apple-announces-m1-pro-m1-max-two-new-custom-built-silicon-to-power-the-next-generation-of-macs/) 的出现，这种情况正在改变——这是苹果硅产品系列中的两个新 SOC。如果苹果的精心展示还不够，那么让人们知道这些新芯片将使该公司能够与市场上更耗电的芯片竞争。新芯片以更多的 CPU 和 GPU 核心展开翅膀。值得注意的是，他们还将使用比 M1 更多的动力来超越竞争对手。

M1 Pro 和 Max 都是非常强大的苹果芯片，具有一些重叠的功能。然而，它们确实有不同的功能，基于这些功能，您将被迫选择一个而不是另一个。在本指南中，我们将尝试着眼于更大的画面，超越苹果在[主题演讲](https://www.apple.com/in/newsroom/2021/10/introducing-m1-pro-and-m1-max-the-most-powerful-chips-apple-has-ever-built/)期间向我们展示的内容，同时推出 [2021 MacBook Pro 笔记本](https://www.xda-developers.com/macbook-pro-2021/)。

**注意:**我们将根据可用性在未来更新更多真实世界的性能指标。目前，主要的重点是在做出购买决定之前了解现有的信息。

**浏览本文:**

## 苹果 M1 Pro:比 M1 更上一层楼

M1 Pro 是苹果不断增长的 M1 芯片家族中的超大 SOC 之一。基于 5 纳米工艺技术，M1 Pro 芯片拥有 337 亿个晶体管。不出所料，苹果正在使用定制的 SoC 封装来支持统一内存。容纳 SoC 芯片和内存芯片的单个 PCB，而不是将内存芯片焊接到主板上。M1 芯片通过这种封装提高了能效，获得了巨大的回报，所以看到新芯片效仿也就不足为奇了。

此外，苹果还将内存总线增加了一倍。我们现在正从 128 位 LPDDR4X 接口转向更快的 256 位 LPDDR5 接口。由于这一点，M1 Pro 芯片承诺高达 200GB/s 的系统带宽。内存控制器占用了 SoC 上的巨大空间，就像 SLC 块一样。系统级高速缓存服务于整个 SoC，允许其共享带宽并减少延迟。

谈到 CPU 本身，M1 Pro 只有两个效率核心，而 M1 芯片上有四个。然而，它的性能内核数量增加了一倍，大概是为了提高多线程性能。这使得 M1 专业版可以在对抗内核数量更高的新型英特尔/AMD 芯片时大展拳脚。苹果的性能图显示了 M1 Pro 如何超越英特尔的 8 核老虎湖 CPU，如酷睿 i7-1185G7 和酷睿 i7-11800H。

苹果这次也对 GPU 架构做了一些改变。M1 Pro 现在拥有一个 16 核 GPU 和 2048 个执行单元。我们的计算吞吐量性能为 5.2 万亿次，比市场上几乎任何其他 iGPU 都要快。它可能无法与英伟达 RTX 3050Ti (8.7 TFLOPs)等竞争，但苹果可以灵活使用降低的功耗。

## 苹果 M1 Max:苹果迄今为止最大的芯片

苹果的 M1 Pro 是 M1 芯片的一大进步，但 M1 Max 才是真正的亮点。这是苹果迄今为止最大的芯片，拥有高达 570 亿个晶体管，将其内部硅的性能推向了一个全新的水平。苹果的展示让它看起来像是 M1 Max 在所有方面都建立在 M1 Pro 的基础上，但它的 GPU 性能使它更优越。值得指出的是，M1 Max 拥有与 M1 Pro 相同的 CPU 包，这意味着它装有一个 10 核 CPU。

这不一定是一件坏事，因为苹果只需要一个 8 核封装就可以敲开英特尔和 AMD 的大门。例如，英特尔的 Tiger Lake Core i9-11980HK 无锁 CPU 具有 8 个内核和 16 个线程，可为市场上的一些高端游戏笔记本电脑提供动力。如果有什么不同的话，M1 最大将达到类似的性能，而消耗更少的能源。

苹果公司已经用总共 32 个核心对 M1 Max GPU 进行了增压，以形成一个具有 10.2 万亿次计算吞吐量的巨大 GPU 块。与占据中心舞台的 32 核 GPU 相比，CPU 块似乎小得可笑。M1 Max 还有两个额外的 128 位 LPDDR5 模块，用于将内存接口从 256 位增加到 512 位(LPDDR5)。

据苹果公司称，M1 Max 的总带宽为 400GB/s，接近市场上的一些高端 GPU。例如，英伟达的 RTX 3060 拥有 360GB/s 的带宽，并使用 192 位内存接口。当然，这不是苹果之间的比较(相当字面上)，因为 M1 Max 使用统一内存，而不是独立 GPU 上的专用 VRAM。

苹果 M1 Max 可以与笔记本电脑 GeForce RTX 3080 GPU 短兵相接。功率曲线图显示了 M1 Max 如何接近 160 瓦 RTX 3080 GPU 的性能，而功耗却降低了 100 瓦。值得指出的是，M1 Max 显示出与 Nvidia 最好的笔记本电脑 GPU 竞争，所以它的价值令人印象深刻。

## 苹果 M1 Pro 和 M1 Max 定制包

我们已经讨论过这些新芯片上的大量晶体管。多亏了 TSMC 的 5 纳米工艺，苹果公司能在芯片中塞进多少东西真是令人难以置信。苹果公司宣传的 M1 Pro 和 M1 Max 的晶体管数量分别为 337 亿和 570 亿，远远高于用于 AMD RX 6000 系列 GPU 的 Navi 21 GPU 的 268 亿晶体管。Nvidia 基于 Ampere 架构的 GA100 GPU 支持 A100，包括 542 亿个晶体管。值得注意的是，Nvidia 和 AMD 都在使用 TSMC 的 7 纳米制造工艺。

不谈论这两种芯片上大大改进的媒体引擎是不明智的。创意专业人士可以期待看到巨大的性能提升，因为这些芯片可以处理 ProRes 和 ProRes RAW 的硬件加速解码和编码。按照典型的 M1 方式，他们在处理这一问题的同时还考虑到了能效。M1 Max 配备两个 ProRes 加速器，视频编码速度比 M1 Pro 快 2 倍。ProRes 加速器数量的两倍也意味着 M1 Max 可以在不同的屏幕上处理多达四个高质量视频播放流。

## 苹果 M1 Pro vs M1 Max:主要区别

| 

苹果 M1 Pro 芯片

 | 

苹果 M1 Max 芯片

 |
| --- | --- |
| 高达 16 核 GPU | 最高 32 核 GPU |
| 256 位存储器接口 | 512 位存储器接口 |
| 200 GB/秒内存带宽 | 400 GB/秒内存带宽 |
| 高达 32GB 的统一内存 | 高达 64GB 的统一内存 |
| ProRes 编码和解码引擎 | 2x ProRes 编码和解码引擎 |

## 最后的想法

苹果新的 M1 Pro 和 M1 Max 芯片在很多方面都比最初的 M1 芯片有所提升，超出了人们的想象。这些新芯片基本上吸收了 M1 芯片的所有优点，并将其放大到一个对超级用户来说显而易见的程度。M1 确实是一个梦幻般的开始，但由于其有限的 SOC 和相对较低的 TDP 值，它还没有准备好与最好的竞争。新芯片通过新的封装、更多的 CPU 和 GPU 核心、更快的内存和其他一些高级功能改变了这一局面。M1 Pro 和 M1 Max 走向更多像 Mac Pro 这样的苹果计算设备只是时间问题。

那么，你应该买哪个呢？总而言之，M1 Pro 是一款非凡的芯片，我们认为它能够处理大多数创造性的工作流程。它的 10 核 CPU 在多线程应用中与英特尔和 AMD 的 8 核巨头展开了竞争。此外，32GB 的统一内存和 16 核 GPU 应该足以满足大多数用户在几乎所有用例中的需求。当然，M1 Max 更强大，但 M1 Pro 用户不会错过任何特别的功能。M1 马克斯只是碰巧做得更好一点。特别是，M1 Max 擅长处理更多 GPU 密集型工作流，如 3D 渲染、视频编辑、编码等。它还配备了额外的视频引擎，性能更好。

我们向寻求最佳工作表现的创意专业人士推荐 M1 Max。它已经取代了旧的 16 英寸 MacBook Pro 中的英特尔芯片，我们知道它将用于所有的最好的 MAC 电脑。对于那些想要更经得起未来考验的芯片的人来说，这也是一个不错的选择。但对于世界上的其他人来说，M1 Pro 是苹果内部芯片的一个很好的展示。你现在就可以[购买采用这些新芯片的新款 MacBook Pro 笔记本电脑](https://www.xda-developers.com/best-macbook-pro-deals/)。