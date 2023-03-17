# 谷歌 Pixel 7 和 Pixel 7 Pro 是首款仅支持 64 位应用的安卓手机

> 原文：<https://www.xda-developers.com/google-pixel-7-64-bit-only-apps/>

如果你一直在关注[谷歌 Pixel 7 系列发布](https://www.xda-developers.com/google-pixel-7-hands-on/)，那么已经有很多*事件*发生了。这两款设备的[内核资源](https://www.xda-developers.com/google-pixel-7-7-pro-factory-images-kernel-source-code/)刚刚下降，还有[一个似乎耗尽电池寿命的显示问题](https://www.xda-developers.com/google-pixel-7-pro-display-problem/)，以及[评论](https://www.xda-developers.com/google-pixel-7-pro-camera-review/)开始慢慢渗入。随着人们接触到设备，用户开始测试它们，并在幕后进行调查。事实证明，谷歌 Pixel 7 系列似乎是第一套仅支持 64 位应用程序的 Android 智能手机。

拉赫曼后来[更正自己](https://twitter.com/MishaalRahman/status/1580586113328025600)说这是一个 64 位的合子，但却是 32 位和 64 位的用户空间，*而不是最初报道的仅 64 位版本的 Android 13。不过，这无疑证明了谷歌 Pixel 平板电脑可能只搭载 64 位版本的 Android 13 的说法。*

这意味着，对于任何没有 64 位库的应用程序，您将无法安装它们。这包括 Jetpack Joyride 等旧版本的应用程序，甚至包括 Flappy Bird 等旧的、完全失效的应用程序。张量 G2 也不是不支持——它的三个不同核心都支持 AArch32 执行。谷歌本可以像以前的智能手机一样支持 32 位。

列出 Android 二进制接口(ABI)返回“armeabi-v7a”或“armeabi”不存在。列出了“arm64-v8a”支持，但是[根据 Android 文档](https://developer.android.com/ndk/guides/abis)，它只支持 AArch64 指令集。

```
 [ro.product.cpu.abi]: [arm64-v8a]
[ro.product.cpu.abilist]: [arm64-v8a]
[ro.product.cpu.abilist32]: []
[ro.product.cpu.abilist64]: [arm64-v8a]
[ro.vendor.product.cpu.abilist]: [arm64-v8a]
[ro.vendor.product.cpu.abilist32]: []
[ro.vendor.product.cpu.abilist64]: [arm64-v8a] 
```

这是什么意思，有什么好处吗？消费者不会真正看到大多数好处，因为这些改进主要体现在增强的安全性、更好的性能以及由于缺少额外的 ABI 而降低的处理成本。自 2019 年 8 月以来，谷歌 Play 商店上的所有应用[必须拥有 64 位支持，该公司](https://www.xda-developers.com/google-play-stop-serving-native-apps-without-64-bit-cpu-support/)[去年停止提供不具备任何 64 位支持的 32 位应用](https://www.xda-developers.com/google-play-stop-serving-native-apps-without-64-bit-cpu-support/)。

对于任何拥有 Pixel 7 系列设备的人来说，没有什么可担心的。你很难找到没有任何 64 位库的应用程序，到目前为止，Flappy Bird 似乎是最受瞩目的。如果你发现了更多，请在评论中告诉我们！