# 霹雳 5:发布日期，规格，以及我们所知道的一切

> 原文：<https://www.xda-developers.com/thunderbolt-5/>

英特尔的 Thunderbolt 接口长期以来一直是基于英特尔的个人电脑的最大吸引力之一，该公司已经在开发下一版本。虽然还没有正式名称，但英特尔已经宣布了下一代 Thunderbolt，我们预计它将被称为 Thunderbolt 5。虽然一些细节仍然未知，但我们已经对下一代 Thunderbolt 的能力有了一个概念。让我们来看看。

## 什么是霹雳*？*

Thunderbolt 是由英特尔开发的硬件接口，旨在允许用户将外围设备连接到他们的 PC。最初的版本使用迷你显示端口连接器，但英特尔从雷电 3 开始改用 USB Type-C。虽然使用相同的连接器，但 Thunderbolt 通常比标准 USB 提供更高的数据速率，使该技术非常引人注目。Thunderbolt 连接支持即插即用的外部 GPU，如 [Razer Core X](https://www.amazon.com/Razer-Chroma-Aluminum-External-Enclosure/dp/B07Q78VMPW/?tag=xda-7ivtan0-20&ascsubtag=UUxdaUeUpU3776&asc_refurl=https%3A%2F%2Fwww.xda-developers.com%2Fthunderbolt-5%2F&asc_campaign=Evergreen) ，以及外部显示器和其他外围设备。

当然，这项技术是由英特尔开发的，通常只有基于英特尔的电脑才有。雷电 3 已被 USB 实现者论坛采用，被称为 USB4，也有一些非英特尔笔记本电脑支持它，如[联想的 ThinkPad Z 系列](https://www.xda-developers.com/lenovo-thinkpad-z-series/)或苹果的 [MacBook Air](https://www.xda-developers.com/macbook-air-m2-2022-review/) 。但 Thunderbolt 仍然是英特尔技术，虽然免版税，但要求更高。认证 Thunderbolt 设备是有成本的，所以没有英特尔处理器的设备通常会放弃 Thunderbolt 认证，坚持使用普通的 USB 端口。即使这样，USB4 端口仍然不常见，至少现在是这样。

Thunderbolt 的独特之处，特别是从 Thunderbolt 4 开始，在于认证要求相当高。笔记本电脑可以有一个 USB4 端口，仅支持 20Gbps 带宽，不支持功率传输(PD ),或者它可以达到 40Gbps，并添加 PD 支持。这是一个灵活的规范，但它可能会混淆消费者。另一方面，Thunderbolt 4 端口*拥有*来支持 40Gbps、电力传输和外部 GPU 的 PCIe 隧道。当你看到一台 Thunderbolt 4 笔记本电脑时，你会更清楚地知道你会得到什么。

## 霹雳 5 有什么新功能？

英特尔已经开始戏弄下一代 Thunderbolt，我们已经知道了它的一些功能，尽管我们还不知道官方的品牌。英特尔尚未讨论功率传输要求，但我们知道它将显著增加可用带宽，至少达到 80Gbps。

### 80Gbps 双向带宽(或高达 120Gbps 单向带宽)

下一代 Thunderbolt 的重大升级将是最大带宽，从 40Gbps 双向增加到 80Gbps。换句话说，Thunderbolt 5 将使用四个数据通道，每个通道支持 40Gbps。在标准配置中，每个方向有两条线路，因此可以提供 80Gbps 的带宽。

然而，对于特殊配置，例如使用非常高分辨率的显示器，通道可以动态地重新配置，以便三个通道在一个方向上发送数据。这意味着你可以在一个方向上获得 120Gbps 的带宽，而在另一个方向上仍然可以获得 40Gbps 的带宽。如果你使用非常清晰的显示器，这将使使用一个 Thunderbolt 端口驱动它们成为可能，即使你使用多个端口。

由于一种新的信号技术，这种新的带宽限制甚至可以在现有的 1 米长的 Thunderbolt 4 无源电缆上得到支持。只要你的设备支持 Thunderbolt 5，电缆就不是问题。

### 新的显示端口、PCI Express 和 USB 规格

为了适应新的带宽限制，Thunderbolt 4 还支持最新的显示端口、PCIe 和 USB 数据隧道规范，就像 USB4 版本 2.0 一样。首先，这包括 DisplayPort 2.1，它对 DisplayPort 信号通过 USB 电缆的方式进行了具体的改进。这一新版本更加高效，它支持 DisplayPort 信号高达近 80Gbps 的带宽，可以在 60Hz 下驱动 8K 显示器，无需流压缩或色度二次采样。

下一代 Thunderbolt 还将使 PCIe 带宽翻倍，允许更快的外部存储和显卡，这在一定程度上受到当前带宽限制的制约。作为参考，目前的 Thunderbolt 固态硬盘的速度可以达到 2800 MB/s(广告)，因此翻一番将达到 5600 MB/s，几乎与今天的许多内部固态硬盘一样快。外部 GPU 市场在过去几个月里也一直处于平静状态，因为显卡需要比 Thunderbolt 4 允许的更多的带宽，因为自 2015 年推出雷电 3 以来，这种能力一直没有真正改变。

最后，虽然英特尔没有提到，但 USB 4 2.0 版规范还包括一个新的 USB 数据隧道规范，支持高达 20Gbps 的数据传输。这基本上相当于 USB 3.2 Gen 2x2，没有多少设备支持。不过，如果你有一个外部驱动器可以支持它，你现在可以得到更快的传输。

## 霹雳 5 什么时候来？

英特尔尚未分享下一代 Thunderbolt 的任何细节，到目前为止，我们所拥有的只是一个早期的预告。英特尔只分享了一些关于带宽的一般信息，但发布日期仍然未知。

英特尔最近推出了用于台式机和笔记本电脑的第 13 代处理器，而 Thunderbolt 5 尚未亮相，因此可以肯定的是，我们最早将在下一代英特尔处理器中看到它。这些应该会在年底首次亮相，所以你还需要一段时间才能看到这些好处。

## 我的设备支持它吗？

如果你想充分利用 Thunderbolt 5，你将需要专门支持它的设备，而这些设备目前还不存在。然而，正如我们上面提到的，长达一米的无源 Thunderbolt 4 电缆仍然可以支持 Thunderbolt 5。

至于哪些设备将支持 Thunderbolt 5，你可以期待大多数采用英特尔处理器的高端笔记本电脑都内置了它。虽然 Thunderbolt 不是英特尔处理器独有的，但大多数 AMD 笔记本电脑都倾向于错过对它的支持，除非有重大转变，否则这种情况可能会继续下去。

不过，下一代 Thunderbolt 将向后兼容现有的 Thunderbolt 版本，因此任何基于 Thunderbolt 4 的配件都将继续工作。当然，带宽将被限制在你的旧 Thunderbolt 设备支持的范围内，所以你不能在旧设备上神奇地获得 Thunderbolt 5 的好处。Thunderbolt 还可以与任何操作系统的设备兼容——无论是 Windows 11、macOS、Chrome OS 还是其他操作系统。