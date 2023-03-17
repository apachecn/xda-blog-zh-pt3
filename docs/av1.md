# AV1 是什么，为什么它对谷歌 Chromecast HD 很重要？

> 原文：<https://www.xda-developers.com/av1/>

如果你一直在关注围绕谷歌 Chromecast HD 发布的任何泄漏，你可能已经看到了许多关于 AV1 编解码器支持的传言。虽然这确实是从 H264 和 VP9 等编解码器向前迈出的一大步，但故事远不止于此。AV1，也称为 AOMedia Video 1，于 2018 年 3 月首次发布，在整个行业的采用过程中，这是一条缓慢的道路。这是 AV1 的全部故事，它如何优于 VP9 和 H.264，以及它为什么如此重要。

## AV1 是什么？

AV1 是由开放媒体联盟(Alliance for Open Media)开发的一种编解码器，该联盟由技术领域的许多不同公司组成。它的主要好处是免版税(因此，公司可以在他们的软件中免费实现它)，并且它比 VP9 和 H264 等有一些巨大的节省。脸书工程公司在 2018 年进行了测试，结论是 AV1 参考编码器的数据压缩率分别比 libvpx-vp9、x264 High profile 和 x264 Main profile 高 34%、46.2%和 50.3%。这意味着，对于网速较慢的用户，你可能会享受到比以往更高的质量，而对于网速较快的用户，在相同的网速下，你可以获得更高的比特率。

第一个支持 AV1 解码的智能手机芯片组是联发科 Dimenisty 1000，它支持高达 4K 60 FPS。Nvidia Geforce 3000 系列支持解码，[新的 Nvidia Geforce 4000 系列](https://www.xda-developers.com/nvidia-geforce-rtx-40-series-launch-release-date-price/)支持编码和解码，三星的 Exynos 2100/2200 也支持 AV1 解码。业界的支持正在慢慢增长，Chromecast HD 中的芯片组也支持 AV1 解码。我们联系了谷歌进行评论，被告知搭载谷歌电视(HD)的 Chromecast 支持 AV1。

不仅如此，桌面上的 YouTube 还支持 AV1、[，只要你使用兼容的浏览器，你就可以在你的账户设置](https://www.youtube.com/account_playback)中启用它。事实上，该公司已经设计了自己的芯片用于编码 AV1 视频，这将用于 YouTube 的数据中心。该芯片代号为“Argos”，是第二代视频(trans)编码单元(VCU)，可以将上传到平台的视频转换为各种压缩格式，并针对不同的屏幕尺寸进行优化。谷歌声称，其新的 Argos VCU 处理视频的效率比传统服务器高 20-33 倍。

## AV1 的历史

AV1 背后的背景以及为什么创建它也很重要。VP9 是由 Google 开发的免版税编解码器，任何人都可以使用，因为它是免版税的，所以它可以在任何需要它的平台或服务上实现。YouTube 在任何支持编解码器的设备上使用它(由于带宽减少，这对谷歌来说意味着巨大的节省)，它甚至被视频点播服务所采用，如、Twitch 和 Vimeo。

然而，因为谷歌在采用更好的压缩算法以减少其数据中心的带宽使用方面有既得利益，所以它开始致力于 VP10——VP9 的继任者。当你计算数十亿分钟的视频时，每段视频的视频压缩量的微小增加可以导致巨大的成本节约和用户体验的重大改善。谷歌宣布，他们计划在 2016 年发布 VP10，然后每 18 个月发布一次更新，以确保稳定的进展。谷歌甚至开始发布 VP10 的代码，但该公司宣布取消 VP10，并成立了开放媒体联盟(AOMedia)。

开放媒体联盟包括所有人，从处理器设计者(AMD、Arm、Broadcom、Chips&Media、Intel、Nvidia)到浏览器开发者(Google、Microsoft 和 Mozilla)，到流媒体和视频会议服务(Adobe、Amazon、BBC R&D、Cisco、网飞、Youtube)。所有这些公司都一直在为 AV1 提供某种形式的支持，无论是通过芯片组中引入的硬件解码器、浏览器中解码器的实现，还是在流媒体服务上使用编解码器。

## AV1 对 HEVC/H265

AV1 和 HEVC(高效视频编码，也称为 H.265)的最大区别在于授权。为了提供 HEVC 支持的产品，您需要从至少四个专利池(MPEG LA、HEVC Advance、Technicolor 和 Velos Media)以及许多其他公司获得许可，其中许多公司不提供标准许可条款，而是要求您协商条款。

对于谷歌 Chrome、Opera、网飞、亚马逊视频、思科 WebEx Connect、Skype 等产品来说，这些高额版税已经是个问题，而且它们完全排除了 Mozilla Firefox 等项目选择 HEVC 的可能性。这是因为它违背了 Firefox 项目的多个核心价值:Firefox 需要免版税才能发布到许多自由/开源软件项目中，而 HEVC 的使用会阻止它；Mozilla 相信自由开放的网络，如果你推广专利保护的标准，这是不可能的。即使忽略这两个问题，Mozilla 也不能在版税和必要的许可协议谈判上浪费数亿美元。

一个有趣的事实是，直到几年前，这些问题也阻止了 Firefox(和 Chromium)在许多平台上包含原生 H.264 回放...而且它仍然需要一个 Linux 上的插件。火狐不太可能在 21 世纪 30 年代(或者更晚)专利到期前支持 HEVC。即使到今天，Firefox 也只支持 H.264，这要归功于思科通过 OpenH264 支付 Mozilla 的所有许可费用，以便在下一代编解码器准备就绪之前，在整个市场上实现 H.264 的标准化。在 Mozilla 视频编解码器指南上，该公司称“当 HEVC 受到专利的阻碍时，Mozilla 不会支持它。”迄今为止，只有 Edge 和 Internet Explorer 支持原生 HEVC 播放，并且仅在支持解码的特定硬件上。

在效率方面，这两种编解码器针锋相对。它们的效率通常不相上下(尽管测试显示 AV1 略微领先)，但有一个问题，由于缺乏硬件编码功能，AV1 通常需要更长的时间来编码。滑铁卢大学在 2020 年发现，虽然 AV1 在编码 4K 视频时比 HEVC 节省了 9.5%的比特率，但 AV1 视频的编码时间也是 AVC 的 590 倍。相比之下，HEVC 只花了 4.2 倍的时间。显然，这些测试是在 AV1 生命周期的早期进行的，当时硬件支持并不真正可用。

## AV1 的未来

随着越来越多的设备支持硬件解码，AV1 似乎将为高质量压缩视频播放开辟道路。鉴于 HEVC 只被桌面上的一个浏览器支持(不管怎样，既然 Internet Explorer 已经死了，AV1 显然是未来 VP9 的继任者。随着支持的增长，越来越多的设备将最终使用它。已经有[的一些实验标志](https://aomedia.googlesource.com/aom/+/experimental/build/cmake/aom_config_defaults.cmake)指向 AOM 仓库中的 AV2，以及去年[提交给仓库的“AV2 研究的开始锚”](https://aomedia.googlesource.com/aom/+/refs/tags/research-v1.0.0),这表明我们也将在未来看到迭代。

## 为什么 AV1 对谷歌 Chromecast HD 很重要？

如果你想买谷歌 Chromecast HD，你可能会关心 AV1 的一个重要原因是你的网络能力。如果你买的是高清版而不是 4K 版，可能有几个原因会让你这么做，其中之一可能是你的互联网没有 4K 流媒体的带宽。如果是这样的话，那么你很可能会对带宽很敏感，AV1 意味着你可以从 Chromecast 中获得更高比特率的视频。这将在您的互联网已经支持的相同数据速率下带来更好的整体视频质量。

 <picture>![The new Chromecast with Google TV is a simple and relatively affordable streaming device for casual users.](img/b55c50b2ed3d50990422e0d31898bd3e.png)</picture> 

Chromecast with Google TV

##### 带谷歌电视的谷歌 Chromecast(高清)

配备谷歌电视(HD)的 Chromecast 是一款更便宜的 Chromecast，只能进行 1080p 播放，但对很多人来说，这就是你需要的全部。

不仅如此，这可能是一个更大的原因，它是第一个真正支持 AV1 的*[主流电视加密狗](https://www.xda-developers.com/best-android-tv-box/)。Roku 在一定程度上是主流，但在一些地区更难获得，而 Fire TV Stick 4K Max 是目前唯一的其他选择。谷歌的电视加密狗生态系统是迄今为止所有生态系统中最丰富的，因此 AV1 的加入也是一件大事。这使得 AV1 作为一种选择合法化，并可能推动其他公司以其他方式支持 AV1。*