# Android 11 Beta 3 已经发布，取消了新冠肺炎联系人追踪应用的位置要求

> 原文：<https://www.xda-developers.com/android-11-beta-3-here-remove-location-requirement-covid-19-contact-tracing-apps-exposure-notification-system/>

谷歌上个月发布了 Android 11 Beta 2，将 Android 操作系统的新更新推向了“平台稳定”状态。随后是 [Beta 2.5 版本](https://www.xda-developers.com/android-11-beta-2-5-fixes-pixel-4-screen-flickering-and-more/)，这是一个更大的错误修复版本，而不是一个适当的增量。在每一次发布之间，spot 都会有很多宣布和未宣布的变化，就像我们在 [Beta 1](https://www.xda-developers.com/android-11-beta-1-rolled-out-early-some-google-pixel-4-users-whats-new-changes-features/) 和 [Beta 2](https://www.xda-developers.com/android-11-beta-2-new-features/) 中发现的一样。当我们摩拳擦掌期待预计在 9 月 8 日左右发布的稳定版时，谷歌现在已经发布了 Android 11 Beta 3，这是正式稳定版发布前的最后一个测试版。

**[安卓 11 XDA 新闻](https://www.xda-developers.com/tag/android-11/)**

Android 11 Beta 2 代表了平台稳定性的里程碑，这意味着所有面向应用的行为都是最终的，因为它们存在于版本中。因此，Android 11 Beta 3 专注于帮助开发人员在准备 Android 11 时对他们的应用程序进行最后的润色。这包括以官方 API 30 SDK 为目标，并通过 Android Studio 可用的新工具和更新进行构建。因此，这个 Beta 3 版本代表了你对第一个官方 Android 11 稳定更新的预期，减去了任何可能在这段时间内被发现和修复的主要错误。

如果你是 Android 应用开发者，现在是完成兼容性测试并尽快发布更新的好时机。对于 SDK、库、工具和游戏引擎开发者来说，发布一个兼容的版本更为重要，因为你所坚持的改变会耽误其他依赖你工作的开发者。

这个版本预计不会有任何重大的未宣布的变化，但我们仍将对他们保持警惕。

至于宣布的变化，Android 11 Beta 3 包括对[曝光通知系统(ENS)](https://www.xda-developers.com/google-apple-new-privacy-functional-improvements-exposure-notification-covid-19-contact-tracing-api/) 、谷歌和苹果的新冠肺炎联系人追踪 API 的更新。现在，用户可以使用 ENS 运行应用，而无需在 Android 11 上打开设备位置设置。谷歌表示，这一例外仅适用于使用曝光通知系统的应用程序，因为它的设计方式使得使用它的新冠肺炎追踪应用程序无法通过蓝牙扫描来推断设备位置。这应该解决了用户和开发者在这些应用环境中的一些隐私问题。虽然我们很欣赏这一变化，但我们确实需要看看有多少用户将在未来几个月内访问 Android 11，而不是 Android 用户的总数。请注意，为了保护用户隐私，所有其他应用程序仍将被禁止执行蓝牙扫描，除非设备位置设置已打开，并且用户已授予他们位置权限。

## 为谷歌 Pixel 设备下载 Android 11 Beta 3

如果你参加了测试计划，Android 11 Beta 3 更新应该会通过 OTA 更新到你支持的谷歌 Pixel 设备上。但如果它没有，你可以从以下链接下载支持谷歌 Pixel 设备的 Android 11 Beta 1:

### 谷歌像素

### GSI 下载

为了让事情变得更容易，你也可以使用 [Android 闪存工具](https://developer.android.com/preview/download#flashtool)安装测试版，而不是通过恢复或快速启动手动刷新。