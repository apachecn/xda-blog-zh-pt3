# Android 14 可能会添加一个高级内存保护功能，以保护您的设备免受内存安全漏洞的影响

> 原文：<https://www.xda-developers.com/android-14-advanced-memory-protection/>

最近，内存安全一直是谷歌的首要任务，因为内存安全漏洞往往是软件开发中最严重的漏洞。事实上，在 2022 年之前，内存安全漏洞一直占 Android 严重漏洞的大多数，这是谷歌用 [Rust 编程语言](https://www.xda-developers.com/google-developing-android-rust/)而不是 C/C++编写 Android 新本机代码的重要部分。谷歌一直致力于支持其他方法来缓解 Android 中的内存安全漏洞，其中一种方法称为内存标记。在运行 [Android 14](https://www.xda-developers.com/android-14) 的支持设备上，可能会有一个新的“高级内存保护”设置可以切换该功能。

内存标记扩展(MTE)是 Arm v9 CPUs 的一项强制性硬件功能，通过提供有关内存违规的详细信息来防止内存安全错误(运行时性能开销很小)。[正如谷歌解释的](https://source.android.com/docs/security/test/memory-safety/arm-mte)，“在一个高层次上，MTE 用额外的元数据标记每个内存分配/释放。它将一个标记分配给一个内存位置，然后这个标记可以与引用该内存位置的指针相关联。在运行时，CPU 会在每次加载和存储时检查指针和元数据标签是否匹配。

谷歌已经在几个版本的 Android 软件栈中支持 MTE 了。在 Android 12 中，Android 的堆分配器 scudo 在兼容设备上增加了对三种 MTE 操作模式的支持:同步模式、异步模式和非对称模式。Google 还使得在构建时或通过系统属性和/或环境变量为系统进程启用 MTE 成为可能。应用程序可以通过 [android:memtagMode](https://developer.android.com/reference/android/R.attr#memtagMode) 属性选择支持 MTE。当 Android 中的进程启用 MTE 时，诸如释放后使用和缓冲区溢出等一系列内存安全错误会触发崩溃，而不是无声的内存崩溃。

在 [Android 13](https://www.xda-developers.com/android-13) 中，谷歌为用户空间添加了一个 ABI，将请求的 MTE 操作模式传达给引导加载程序。这可用于在默认情况下未启用 MTE 的兼容设备上启用它，或者也可用于在默认情况下启用它的兼容设备上禁用它。在 Android 13 中将 ro . arm 64 . memtag . bootctl _ supported 系统属性设置为“true”会告诉系统引导加载程序支持 ABI，并且还会触发一个按钮出现在开发者选项菜单中，允许用户在下次重启时启用 MTE。这是针对那些希望在启用 MTE 的情况下测试其应用程序行为的开发人员。

不过，在 Android 14 中，在兼容设备上启用 MTE 可能需要更多开发者选项。如果设备具有支持 MTE 的 Arm v8.5+ CPU，设备实现支持用于将所请求的 MTE 操作模式传达给引导加载程序的 ABI，并且新的系统属性“ro . Arm 64 . memtag . bootctl _ Settings _ toggle”被设置为 true，则新的“高级内存保护”页面可能会出现在“设置>安全与隐私>更多安全设置”中。这个页面也可以通过新的[动作 _ 高级 _ 内存 _ 保护 _ 设置](https://developer.android.com/reference/android/provider/Settings#ACTION_ADVANCED_MEMORY_PROTECTION_SETTINGS)意图动作来启动。

值得注意的是，[谷歌 Pixel 7](https://forum.xda-developers.com/f/google-pixel-7.12607/) 系列中的张量 G2 芯片组使用 Arm v8.2 CPU 内核，因此它们不支持 MTE。如果即将推出的谷歌 Pixel 8 系列像许多其他旗舰 Android 设备一样使用新的 Arm v9 CPU 核心，那么他们将拥有支持 MTE 的硬件。然而，这种“高级内存保护”功能是否会在稳定版中实现还有待观察。

*感谢安全研究员 [@flawedworlddev](https://twitter.com/flawedworlddev) 对本文的帮助！*