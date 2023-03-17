# 谷歌详细说明了它是如何保护安卓设备上的固件的

> 原文：<https://www.xda-developers.com/google-details/>

# 谷歌详细说明了它是如何保护安卓设备上的固件的

你的智能手机存储了大量重要数据，谷歌希望帮助保护这些数据的安全。

雪地中的 Pixel 7 Pro

我们的智能手机是我们生活的中心。我们与所爱的人交流，计划我们的日子，并通过他们组织我们的财务。对于那些可能想针对你或从你那里偷东西的人来说，它们是完美的攻击媒介，这就是为什么要花这么大力气来保护它们。谷歌现在已经详细说明了它如何保护 Android 平台，不仅是通过 Android 本身，还包括它如何防止对作为你的 SoC 的一部分运行的其他微处理器的固件的攻击。

谷歌一直致力于防止对应用程序处理器(AP)的攻击，比如在 Android 中构建基于编译器的缓解措施。该公司宣布，它正在几个领域与“生态系统合作伙伴”合作，旨在加强与 Android 交互的固件的安全性。他们正在探索基于编译器的杀毒软件，如 [BoundSan](https://source.android.com/docs/security/test/bounds-sanitizer) 和 [IntSan](https://source.android.com/docs/security/test/intsan) ，以及其他漏洞缓解措施。该公司还在研究额外的内存安全功能，[，我们知道这可能会随着](https://www.xda-developers.com/android-14-advanced-memory-protection/) [Android 14](https://www.xda-developers.com/android-14) 推出。

谷歌一直致力于通过引入对内存安全模块的原生 Rust 支持来提高 Android 12 和 Android 13 的安全性，Android 13 是第一个大部分新代码都用 Rust 编写的 Android 版本。对于运行比 AP 上可执行的固件小得多的固件的处理器，很难构建漏洞利用缓解措施，并且任何构建的缓解措施都可能反过来对性能产生负面影响。

随着 Android 13 的发布，谷歌更新了其[严重性指南](https://source.android.com/docs/security/overview/updates-resources#severity)，以进一步强调连接固件中可远程利用的漏洞。该公司还通过其[漏洞奖励计划](https://bughunters.google.com/about/rules/6171833274204160/android-and-google-devices-security-reward-program-rules)接受并奖励外部贡献。这有助于激励安全研究人员识别严重的漏洞并向谷歌报告。这提高了整个平台的安全性。重要的是不仅要保护运行在 AP 上的操作系统，还要保护运行在 SoC 其他部分上的其他较小的固件。