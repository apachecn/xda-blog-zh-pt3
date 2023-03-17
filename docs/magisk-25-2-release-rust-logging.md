# Magisk v25.2 标志着项目生锈的开始

> 原文：<https://www.xda-developers.com/magisk-25-2-release-rust-logging/>

回到 2021 年，我们看到了将内存管理的 Rust 编程语言引入 Android 代码库的第一步[。吴炯，也就是 XDA 资深知名开发商](https://www.xda-developers.com/google-developing-android-rust/)[托普约翰吴](https://forum.xda-developers.com/m/topjohnwu.4470081/)，显然也在为 Magisk 项目考虑同样的问题。据吴介绍，[在通过稳定渠道发布 Magisk v 25.0 build 后，已经开始了](https://twitter.com/topjohnwu/status/1538462758332575744)的实验。现在，topjohnwu 以 v25.2 的形式推出了 Magisk 的新的稳定版本，整个日志记录基础设施都过渡到了 Rust。

Magisk 的大多数低级组件都是用 C++编写的。然而，作为一种非内存管理的语言，它使程序员面临内存泄漏和缓冲区溢出。另一方面，Rust 提供了 C++所能提供的速度、灵活性和大部分直接映射到硬件功能的能力，同时提供了一个内存安全的环境。尽管我们并不期望很快在 Rust 中看到 Magisk 的完全实现，但是将 Rust 代码集成到项目的日志基础设施中的早期工作可能非常重要。

**[Magisk XDA 论坛](https://forum.xda-developers.com/f/magisk.5903/)**

值得注意的是，v25.1 中间版本在 v25 发布后仅 12 天就发布了，但这只是一个小的 bug 修复更新。然而，Magisk 的最新稳定版本是一个成熟的维护更新，它还具有许多与 MagiskInit 相关的改进。

以下是 Magisk v25.2 的完整变更日志:

*   [MagiskInit]修复了使用存根 cpio 时的潜在问题
*   [MagiskInit]修复了使用存根 cpio 时重新启动以进行恢复的问题
*   [MagiskInit]修复 rootfs 设备的 sepolicy.rules 符号链接
*   [常规]更好的数据加密检测
*   [常规]将整个日志记录基础结构移入 Rust

如果您想了解 v25.2 版本的全部细节，请从下面的链接下载到您的设备上。如果您碰巧遇到了最新版本的任何问题，请确保在项目的 [GitHub 库](https://github.com/topjohnwu/Magisk/issues)的“问题”部分提交一份错误报告。

**[下载 Magisk v25.2](https://github.com/topjohnwu/Magisk/releases/tag/v25.2)**

* * *

**来源:** [吴炯在推特上](https://twitter.com/topjohnwu/status/1549956443469557760)