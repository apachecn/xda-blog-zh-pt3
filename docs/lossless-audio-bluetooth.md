# 无损音频可以和蓝牙一起工作吗？

> 原文：<https://www.xda-developers.com/lossless-audio-bluetooth/>

苹果宣布苹果音乐将推出无损音频，这让很多消费者兴奋不已，尤其是音乐发烧友和音响发烧友。多年来，音频流媒体平台一直采用 MP3 和 AAC 格式，因为它们占用的存储空间较少。它们需要更少存储空间的原因是它们被压缩了，这意味着与原始主质量轨道相比，许多细节和清晰度在处理过程中丢失了。如果您还没有阅读我们关于[无损音频的专门讲解，以及它对您(最终消费者)意味着什么](https://www.xda-developers.com/lossless-audio/)，我们强烈建议您阅读一下，大致了解一下无损音频的概念，并更好地理解我们在本文中讨论的内容。

## 可以通过蓝牙听无损音频吗？

直接的答案是否定的。无损音频不能通过蓝牙工作。

作为一种技术，蓝牙只是不能以如此高的速度传输如此多的数据，这就是为什么缺乏对无损音频传输的支持。蓝牙工作在 2.4GHZ ISM 频谱上，主要用于短距离通信。这就是为什么通过 LDAC 的音频传输也不完美的原因。你可能会经历抖动，总的来说是不稳定的体验，有时会有音频中断。LDAC 的范围也很差，这不是一个非常精致的体验。

用于通过蓝牙传输音乐的编解码器都无法达到无损音频所需的正确比特率和采样速率。苹果自己澄清说，AirPods、AirPods Pro 和超高级 AirPods Max 都通过蓝牙工作，将无法从 Apple Music 无损播放音频。不仅仅是这些特定的耳机或头戴式耳机，而且没有一种真正的无线耳机选项能够处理无损音频，无论它们在功能和价格方面有多高端。

原因很简单，就所使用的编解码器而言，大多数蓝牙耳机和头戴式耳机的最大输出为 AAC、aptX 和 aptX HD，并且这些编解码器中没有一个能够实现 1，411kbps 的最小比特率，以将音轨分类为无损。不仅仅是耳机，你的手机也有必要通过蓝牙支持这些编解码器。例如，iPhone 只支持通过蓝牙播放音乐的 AAC，而不管耳机/头戴式耳机是否支持更好的编解码器。

## 蓝牙耳机方面最接近无损音频的选项是什么？

用于无损音频的两种流行格式是 FLAC 和 ALAC，这两种格式仅通过一对有线耳机或耳塞来支持。因此，通过蓝牙获得 1,411kbps 的真正无损音频体验几乎是不可能的。然而，有一种音频编解码器在比特率方面非常接近，那就是 LDAC。

许多最新的 Android 智能手机都支持 LDAC，但 iPhone 不支持它。因此，如果您使用正确的蓝牙耳机或支持 LDAC 的耳机，您可以体验最高比特率为 990kbps 的音频。虽然这离 1，411kbps 还很远，但这是使用一副无线耳机/耳塞可以获得的最佳体验。

如果您有一对无线耳机作为录音室监听设备，您也可以通过将 AUX 电缆插入耳机并将其用作有线耳机来使用它们。

如果你想在 LDAC 体验音频，你可以买一副 [1More 三重驱动颈带耳机](https://www.amazon.com/1MORE-Bluetooth-Earphones-Environmental-Isolation/dp/B0829NW67M/?tag=xda-6lfrmet-20&ascsubtag=UUxdaUeUpU4266&asc_refurl=https%3A%2F%2Fwww.xda-developers.com%2Flossless-audio-bluetooth%2F&asc_campaign=Short-Term)或者 [Soundcore Q35](https://www.amazon.com/Soundcore-Cancelling-Headphones-Bluetooth-Comfortable/dp/B08X3PRQTD/?tag=xda-6lfrmet-20&ascsubtag=UUxdaUeUpU4266&asc_refurl=https%3A%2F%2Fwww.xda-developers.com%2Flossless-audio-bluetooth%2F&asc_campaign=Short-Term) 如果你正在寻找耳机。包括 [Oppo Enco W51](https://www.amazon.co.uk/OPPO-W51-Bluetooth-Headphones-Cancellation/dp/B08DH9LVXW/?tag=xdadevelopers-21) 和新推出的[索尼 WF-1000XM4](https://www.amazon.com/Sony-WF-1000XM4-Industry-Canceling-Headphones/dp/B094C4VDJZ/?tag=xda-6lfrmet-20&ascsubtag=UUxdaUeUpU4266&asc_refurl=https%3A%2F%2Fwww.xda-developers.com%2Flossless-audio-bluetooth%2F&asc_campaign=Short-Term) 在内的一些 TWS 耳机也支持 LDAC。如果您想在 Apple Music 上体验最高层次的真正无损音频，您需要一对有线耳机或带 DAC 的耳机。不要担心，我们有一份所有[最佳 DAC 和耳机/头戴式耳机](https://www.xda-developers.com/best-wired-earphones-headphones-dac-lossless-audio/)的列表，您可以购买它们来体验智能手机和电脑上的无损音频。