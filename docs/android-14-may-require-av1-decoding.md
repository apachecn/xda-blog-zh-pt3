# Android 14 可能要求智能手机支持 AV1 解码

> 原文：<https://www.xda-developers.com/android-14-may-require-av1-decoding/>

AV1 是由开放媒体联盟开发的一种编解码器，它是一种免版税的编解码器，与 VP9 和 H264 相比节省了大量带宽。脸书工程公司在 2018 年进行了测试，结论是 AV1 参考编码器的数据压缩率分别比 libvpx-vp9、x264 High profile 和 x264 Main profile 高 34%、46.2%和 50.3%。对于那些可能依赖较慢连接的人来说，这是一个巨大的进步，或者如果你是一家运营 YouTube 等主要视频服务[的公司，这可以转化为大量的成本节约。这就是为什么](https://www.xda-developers.com/google-new-video-chip-youtube-support-av1-encoding/) [Android 14](https://www.xda-developers.com/android-14) 可能要求设备支持 AV1 解码的事实并不令人惊讶。

通过 AOSP Gerrit 上的两次提交，可以证明 AV1 被授权在使用 Android 14 的设备上发布。我们发现的第一个提交将 AV1 编码添加到 Android 兼容性测试套件(CTS)的 VideoCodecTest 中。CTS 是一组自动测试，用于验证与 Android 操作系统版本的兼容性。如果一台设备不能满足 Android 兼容性定义文件(CDD)中概述的要求，那么它可能无法通过谷歌的 CTS——这反过来可能导致无法访问谷歌的应用程序套件。

此外，*斯珀*发现的第二次提交将 AV1 添加到编解码器列表中，设备必须能够解码才能通过。这个提交特别有趣的是，它直接引用了尚未发布的 Android 14 CDD，这是一个谷歌尚未发布的文件，直到 Android 14 发布前不久才会发布。

> 根据 android cdd 14，sec 2.2.2 和 sec 2.6，
> 
> 手持和平板设备实现必须支持解码 AV1

仍有大量旗舰智能手机不支持 AV1 解码，例如任何带有[骁龙 8 Gen 1](https://www.xda-developers.com/qualcomm-snapdragon-8-gen-1/) 的设备。有趣的是，三星 Galaxy S22 的 Exynos 版本可以解码 AV1，但骁龙版本不能，谷歌基于 AV1 兼容性阻止原始设备制造商将其设备更新到 Android 14 将是奇怪的，特别是最近一代现成的旗舰芯片不支持 AV1，除了不太普遍的选项，如联发科和 Exynos。

关于所有这些意味着什么，有两个可能的要点，假设谷歌肯定会以某种方式推进 AV1 解码和编码。要么是只有搭载 Android 14 的设备才需要支持 AV1(这是有道理的，因为 AV1 的长期支持者高通甚至通过[骁龙 8 第二代](https://www.xda-developers.com/qualcomm-snapdragon-8-gen-2/)支持 AV1)，要么是设备可以通过软件解码和编码。正如*斯珀*解释的那样，解码测试只检查设备是否能解码 AV1 视频的单个帧，而不是它使用的是硬件还是软件解码器。

不管怎样，这为 AV1 流媒体在移动设备上的广泛应用奠定了基础。随着智能手机越来越多地支持编解码器，流媒体平台将能够自信地实现它，不仅节省他们端的带宽成本，还可以帮助那些数据连接有限的用户。我们已经联系了谷歌进行评论，如果有回音，我们会更新这篇文章，我们会关注并等待事态的发展。

* * *

**来源:**AOSP·格里特( [1](http://android-review.googlesource.com/c/platform/cts/+/2319612) )， [2](http://android-review.googlesource.com/c/platform/cts/+/2206980) 途经 [*斯珀*](http://blog.esper.io/android-14-deep-dive/) )