# 随着最终测试版推出像素，Android 离公开发布又近了 13 英寸

> 原文：<https://www.xda-developers.com/android-13-final-beta-google-pixel/>

随着谷歌刚刚宣布下一个主要 Android 平台的最终测试版终于到来，Android 13 即将到来。谷歌没有强调任何新功能，但这个版本特别特别——Android 13 Beta 4 是谷歌 Pixel 设备和 Android 模拟器的发布候选版本。这意味着它主要包含错误修复和其他修饰，尽管我们想象会有一些尚未突出的变化。

## Android 13 什么时候发布？

对于 Android 更新，谷歌通常会揭示一个“平台稳定性”里程碑，以便开发者可以知道谷歌打算何时交付最终的 SDK/NDK API，以及最终的内部 API 和面向应用的系统行为。Android 13 Beta 3 为我们带来了平台稳定性，让我们很快就能获得稳定的公开发布。作为背景，Android 12 在 2021 年 8 月达到平台稳定性，最终版本是同年 10 月发布的[。这个版本是一个候选版本，这意味着如果您迫不及待地想尝试它，它应该是相当稳定的。](https://www.xda-developers.com/android-12-launched/)

## Android 13 Beta 4 有什么新功能？

老实说，谷歌没有突出任何表面水平。该公司表示，这一版本为开发人员提供了“完成测试所需的一切”。它主要是为了修复错误和软件抛光，虽然你可能会注意到稳定性的改善，但不太可能有任何重大变化。谷歌表示，开发者尤其应该为以下变化做好准备:

*   **通知的运行时权限:**最新版本的 Android 引入了从应用程序发送通知的新运行时权限。确保你了解新权限是如何工作的，并尽快计划以 Android 13 (API 33)为目标。[此处更](https://developer.android.com/about/versions/13/changes/notification-permission)。
*   **剪贴板预览:**确保你的应用在 Android 13 的新剪贴板预览中隐藏了敏感数据，比如密码或信用卡信息。[更多在此](https://developer.android.com/about/versions/13/behavior-changes-all#copy-sensitive-content)。
*   **JobScheduler 预取:** [JobScheduler](https://developer.android.com/reference/android/app/job/JobScheduler) 现在会尝试预测应用程序的下一次启动时间，并在该时间之前运行任何相关的预取作业。如果使用预取作业，请测试它们是否按预期工作。[更多在此](https://developer.android.com/about/versions/13/behavior-changes-all#prefetch-job-handling)。

谷歌还宣布，关于 Android 13 最终版本的信息将在“未来几周”发布。

## 如何在你的谷歌 Pixel 设备上下载并安装 Android 13 Beta 4

你可以轻松地[为你的 Pixel 设备下载 Android 13 Beta 4](https://www.xda-developers.com/how-to-download-android-13/#beta4) ，并按照我们的指南[如何安装 Android 13](https://www.xda-developers.com/how-to-install-android-13/) 进行设置。谷歌正式发布了 Pixel 6 Pro、Pixel 6、Pixel 5a 5G、Pixel 5、Pixel 4a (5G)、Pixel 4a、Pixel 4 XL 或 Pixel 4 的测试版更新。您可以在 Android Studio 的 Android 模拟器中使用 64 位系统映像，也可以使用 GSI。

要了解更多关于第四个也是最后一个测试版的信息，请访问 Android 开发者博客上的官方博客文章。