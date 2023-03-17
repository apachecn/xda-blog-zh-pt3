# Windows 11 系统要求并不是世界末日

> 原文：<https://www.xda-developers.com/windows-11-defending-system-requirements/>

距离微软宣布 [Windows 11](https://www.xda-developers.com/windows-11/) 已经过去了一周，尘埃终于开始落定。即将推出一系列新功能。Windows 获得了全新的设计，新的通知中心，快速设置，Android 应用支持，以及全面的改进。但是 Windows 11 的一个变化引起了很多反对，那就是[新系统要求](https://www.xda-developers.com/windows-11-minimum-requirements/)。

事实上，RAM 和存储需求翻了一番，达到 4GB 和 32GB，但这并不是引起愤怒的原因。人们对两件重要的事情感到不安 TPM 要求和 CPU 要求。

我理解这种愤怒。真的。如果我在 2018 年夏天买了一台 Surface 笔记本电脑，我会对我的硬件制造商即将推出不支持我的笔记本电脑的新版本 Windows 感到超级沮丧。也许是时候喘口气了，因为一切都会好的。

## Windows 11 最低系统要求

| 

处理器:

 | 兼容的 64 位处理器或片上系统(SoC)上的 2 个或更多内核可提供 1 GHz 或更快的速度 |
| 

内存:

 | 4 千兆字节(GB) |
| 

存储:

 | 64 GB 或更大的存储设备注:请参见下面的“有关保持 Windows 11 最新的存储空间的更多信息”了解更多详细信息。 |
| 

系统固件:

 | UEFI，支持安全引导 |
| 

TPM:

 | 可信平台模块(TPM)版本 2.0 |
| 

显卡:

 | 与 DirectX 12 或更高版本的 WDDM 2.0 驱动程序兼容 |
| 

显示:

 | 对角线大于 9 英寸的高清(720p)显示屏，每个颜色通道 8 位 |
| 

互联网连接和 Microsoft 帐户:

 | Windows 11 家庭版需要互联网连接和 Microsoft 帐户才能在首次使用时完成设备设置。在 S 模式下将设备切换出 Windows 11 家庭也需要互联网连接。在这里了解更多关于 S 模式的信息。对于所有 Windows 11 版本，需要访问互联网才能执行更新、下载和利用某些功能。某些功能需要 Microsoft 帐户。 |

乍一看，对 CPU 的要求似乎并不太疯狂。Windows 11 和 Windows 10 需求之间的唯一区别是不支持 32 位 CPU，也不支持单核 CPU。

随后，微软[公布了一份支持的 CPU 清单](https://www.xda-developers.com/cpus-compatible-windows-11/)。事实证明，这个列表更加极端。根据列表，支持 Intel 8 代及更新版本，支持 AMD Zen 2 APUs。如上所述，你可以有一台不到三年的电脑，它不符合 Windows 11 的条件。

这里有一个更好的例子。你今天可以买一个 Surface Studio 2*在今天的要求下它将没有资格使用 Windows 11。Surface Studio 2 中的 CPU 是产品推出时的一代老款，至今仍未刷新。微软正在销售全新的第七代 CPU 和 NVIDIA GeForce GTX 1070 显卡。连折扣都没有；你可以在微软商店花 4800 美元买一个。*

 *## 为什么微软在 Windows 11 中改变了系统要求

我想我们都同意这不是一个微妙的变化。当该公司首次推出其下一代操作系统时，它没有提到任何关于这一点的事情。所有的新需求都是在文档中发现的。四天后在一篇博客文章中提到了这个问题。以下是微软对事情发生变化的确切解释:

1.  **安全。** Windows 11 提高了安全性的标准，要求硬件支持 Windows Hello、设备加密、基于虚拟化的安全性(VBS)、受虚拟机管理程序保护的代码完整性(HVCI)和安全引导等保护功能。这些特性的结合已经被证明能够[在测试设备上减少 60%的恶意软件](https://www.microsoft.com/security/blog/2021/01/11/new-surface-pcs-enable-virtualization-based-security-vbs-by-default-to-empower-customers-to-do-more-securely/)。为了满足这一原则，所有 Windows 11 支持的 CPU 都具有嵌入式 TPM，支持安全引导，并支持 VBS 和特定的 [VBS 功能](https://techcommunity.microsoft.com/t5/virtualization/virtualization-based-security-enabled-by-default/ba-p/890167)。
2.  **可靠性。**升级到 Windows 11 的设备将处于受支持的可靠状态。通过选择采用新的 [Windows 驱动程序模型](https://docs.microsoft.com/en-us/windows-hardware/drivers/develop/getting-started-with-windows-drivers)并得到我们的 OEM 和芯片合作伙伴支持的 CPU，实现 99.8%的无崩溃体验。
3.  **兼容性**。Windows 11 旨在与您使用的应用程序兼容。它拥有> 1GHz、双核处理器、4GB 内存和 64GB 存储，符合我们对 Office 和微软团队的最低系统要求。

很明显，微软本可以只为[新款电脑](https://www.xda-developers.com/best-15-inch-laptops/)提供一些功能，但是还有一个关键原因没有被提及。微软想让你买一台新电脑。

Redmond 公司真的希望生活在一个每个人大约每五年就买一台新电脑的世界里。你猜对了，TPM 2.0 成为新计算机的一项要求已经有五年了，这不是一个错误。微软并不指望你明天就去买一台新的兼容 Windows 11 的电脑。你可以继续使用 Windows 10 一段时间。但它希望你能比升级的时候更早购买 Windows 11 电脑。

当微软开始提供免费的 Windows 10 升级时，每个人都在问该公司将如何利用 Windows 赚钱。嗯，它通过出售 OEM 许可证来赚钱。这是每家 OEM 厂商为每台机器安装 Windows 所支付的费用。

## 几十年来 Windows 系统要求的第一次重大变化

我们不要试图忽视这一点。Windows 11 最低要求的转变是一个重大转变，可能是 Windows 历史上最大的转变之一。然而，值得注意的是，Windows 需求在很长一段时间内都没有发生有意义的变化。

2015 年 7 月 29 日，六年前推出的 Windows 10。从那以后，要求有了一些小的变化，特别是对于新的电脑。事实上，一年后，微软开始强制推行 TPM 2.0。稍晚一点，它授权了 64 位 CPU。对每个人来说，唯一改变的是最低存储空间从 32 位 PC 上的 16GB 和 64 位 PC 上的 20GB 增加到 32GB。

然而，Windows 10 保持了 2009 年首次推出的 Windows 7 的要求。这是因为 Windows 10 与之前的任何版本都有着不同的目的，显然自那以后也是如此。目标是让每个人都使用单一版本的 Windows。当时，微软有一些非常雄心勃勃的计划。在两到三年内，Windows 10 设备将超过 10 亿台，这些设备将包括个人电脑、手机、游戏机、增强现实耳机、物联网设备等。

显然，大部分都没有成功，而且花了很长时间才达到 10 亿台设备。今天，Windows 10 安装在 13 亿台设备上，几乎所有设备都是 PC。但是信息的一个关键部分是微软不想再和自己竞争了。该公司曾面临“Windows XP 问题”,不希望这个问题继续下去。

你看，在 21 世纪初，个人电脑达到了足够好的程度。在 Windows XP 发布十多年后，对它的支持结束时，仍有大量的个人电脑使用旧的操作系统。毕竟，人们真的没有理由升级他们的电脑。它仍然有效。这让微软陷入了困境，因为它想出售 Windows Vista，这是一个巨大的失败，但 Windows 7 也是如此。

无论如何，这就是为什么 Windows 10 没有改变 2009 年首次亮相的系统要求。这些要求包括 x86 或 x64 的 1 GHz 处理器、32 位的 2GB RAM 和 64 位的 2GB RAM，等等。然而，2007 年的 Windows Vista 只需要 800MHz 处理器和 512MB 内存。在此之前的 2001 年，Windows XP 需要 233MHz 奔腾或兼容处理器和 64MB 内存。

我的第一个观点是，这些年来，Windows 系统需求已经发生了很大的变化，如果它们再次发生变化，应该不是什么大问题。

## 我们都被 Windows 10 宠坏了

如果我告诉你，即使你有一台符合 Windows 11 系统要求的全新 PC，你仍然需要支付 100 美元进行升级，会怎么样？你会有什么感觉？你甚至会觉得 TPM 或 CPU 需求不那么令人头疼，因为你知道无论如何都要付费升级。

自 Windows 10 发布以来的过去六年里，我们已经免费获得了一切。不要争论什么都不是免费的，这是以牺牲隐私为代价的。我们不是来谈这个的。

Windows 10 对任何运行 Windows 7 或 Windows 8.1 的人来说都是免费升级。这意味着，如果你在 2009 年至 2015 年期间购买了一台电脑，你就可以免费升级到 Windows 10。如果你在 2009 年之前购买了一台电脑*，并将其升级到 Windows 7，你仍然可以获得免费升级。*

这是史无前例的。在此之前，你总是可以指望为升级支付大约 100 美元，也许更少，这取决于版本、购买时间和其他因素。此外，微软继续为 Windows 10 增值。在 Windows 10 周年更新一年后，微软为该操作系统添加了一系列笔功能。迄今为止，微软已经发布了 11 个 Windows 10 功能更新，今年还会有一个。它们都是免费的。

当你将免费升级的想法与承诺的与过去六年中建立的每个系统的兼容性结合起来时，这是非常令人印象深刻的。但这里有一个关键点——微软不欠我们任何东西。如果它想将 Windows 11 限制在现有电脑的一个子集上，这样你就可以购买一台新电脑，它完全有权利这样做。大多数人会继续使用 Windows 10。

微软没有义务永远为现有的个人电脑提供服务。自 2016 年以来，TPM 2.0 一直是新电脑的要求，第八代英特尔芯片于 2017 年开始出货。

## Windows 10 还有几年的寿命

我们不要忘记微软并没有抛弃你。Windows 10 支持到 2025 年 10 月 14 日。如果你不能在这个假期将你的电脑升级到 Windows 11，四年内你都不会有事。我知道你想要新的闪亮的东西。我们都是。但是 Windows 11 实际上是如何提升你的体验的呢？它能做哪些你在 Windows 10 上做不到的事情？它如何让你的生活更轻松？

即使你在 2018 年年中买了那台 Surface 笔记本电脑——你知道，因为笔记本电脑 2 的库存正在清仓，所以折扣真的很好——你仍然可以从中获得六年的寿命。我知道你想要更多。我知道 Windows 10 的升级给了你更多，但就像我说的，从微软的角度来看，Windows 10 有一个不同的目标。我们的目标是让所有人都使用同一版本的 Windows，但 Windows 11 并非如此。微软真的不希望 Windows 7 支持终止，也不希望 Windows XP 出现同样的问题。

此外，请记住，Surface 笔记本电脑是最糟糕的情况(好吧，Surface Studio 2 是最糟糕的情况；微软还把它当新的卖，不可原谅)。

今年晚些时候会有一个新的 Windows 10 功能更新，[称为版本 21H2](https://www.xda-developers.com/microsoft-windows-10-21h2/) 。微软还没有确认这是否会是最后一个，但这真的不重要。你可以打赌，Windows 10 无论如何真的不会获得新功能。该公司可以继续通过支持包推出较小的更新，或者只是继续通过累积更新服务到 2025 年。

无论哪种方式，当 Windows 11 出现时，你都不会被甩在后面。您的电脑暂时仍受支持。

## Windows 11 系统要求可能会改变

当微软开始解释为什么 Windows 11 的系统要求是这样的时候，它[也说他们可以改变](https://www.xda-developers.com/windows-117th-gen-intel-1st-gen-ryzen-cpus/)。这篇博客文章明确表示，英特尔第六代和更老的处理器，以及 AMD pre-Zen 处理器将不被支持。不过英特尔 7 代和 AMD Zen 1 还是有可能的。此外，TPM 需求似乎也有变通办法。

我毫不怀疑他们会改变。微软一直在做这样的事情。它宣布了一个产品，有一些非常酷的新功能，有奇怪的要求，有很大的反弹，它又退缩了。回顾一下最初的 Xbox One 发布会，当时游戏机原本需要互联网连接，或者微软希望[提高 Xbox Live Gold](https://www.xda-developers.com/xbox-live-gold-price-increase/) 的价格。

问题是微软实际上会后退多少。很可能只是增加了英特尔第七代和 AMD Zen 处理器。可能会更多。事实上，在微软发布解释新要求的博客文章之前，我就有一种感觉，它一直在计划走回头路。

如果微软一开始就说第六代和更新的英特尔处理器可以工作，那将会引起公愤。当然，对于第八代 CPU 的需求也有很多愤怒。也许，如果该公司先宣布第八代需求，然后退回到第六代，这似乎表明微软正在让步。

当然，这只是一个随机的想法，仅此而已。我只是认为，等到这个假期到来，Windows 11 开始发货的时候，需求会有一些变化。

## 结论:Windows 11 系统要求不是世界末日

这一切归结为两个主要选择——你可以购买一台运行 Windows 11 的新电脑，或者你可以继续使用 Windows 10 [四年](https://www.xda-developers.com/when-windows-11-releases-heres-how-much-longer-windows-10-could-be-supported/)。微软不会丢下你不管，这一切都是前所未有的。

我理解反对意见。最大的问题是这会产生电子垃圾，这是一个非常合理的问题。但是你真的需要明白一些事情。像[宏碁](https://www.xda-developers.com/best-acer-laptops/)、[苹果](https://www.xda-developers.com/best-macs/)、华硕、[戴尔](https://www.xda-developers.com/best-dell-laptops/)、[惠普](https://www.xda-developers.com/best-hp-laptops/)、[联想](https://www.xda-developers.com/best-lenovo-laptops/)、LG、[微软](https://www.xda-developers.com/best-microsoft-surface-pcs/)、摩托罗拉、一加、雷蛇、[三星](https://www.xda-developers.com/best-samsung-galaxy-laptops/)等硬件制造商都有一些共同点——他们希望你购买新设备，电子垃圾见鬼去吧。这是他们的事。指责微软想要销售更多的 Windows PCs 就像指责斑马有条纹一样。

我知道没有人喜欢买电脑。这就是为什么在疫情开始之前，个人电脑市场一直在下滑。我们定期升级我们的手机，但当需要一台新的笔记本电脑时，只要你现有的东西还能用，就很容易拖延。但事实就是如此。即使是不支持 Windows 11 系统要求的最新设备，微软仍然提供 7-10 年的稳定服务。你有足够的时间升级。*