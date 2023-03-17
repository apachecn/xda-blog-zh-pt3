# PSA:你不能在谷歌最新的 Pixel 手机上从 Android 13 降级

> 原文：<https://www.xda-developers.com/android-13-downgrade-protection-pixel-6-series/>

Android 13 刚刚为谷歌的 Pixel 智能手机发布，你可以通过进入手机的设置并检查更新来立即安装它。然而，如果你有一台谷歌 Pixel 6、谷歌 Pixel 6 Pro 或谷歌 Pixel 6a，那么请注意:更新后试图回滚到 Android 12 将会触发你手机的防回滚保护。这意味着对 Android 13 的更新本质上是永久的。

我们在 Android 13 工厂图像页面上发现了警告，内容如下:

> “Pixel 6、Pixel 6 Pro 和 Pixel 6a 的 Android 13 更新包含 bootloader 更新，增加了防回滚版本。在这些设备上刷新 Android 13 版本后，您将无法刷新旧的 Android 12 版本。”

这种防回滚保护与小米等公司过去采用的机制并无不同。作为背景，小米通过软件更新在红米 Note 5 上意外实现了防回滚保护。当用户进行降级时，他们会把智能手机变成砖头，因为他们不知道自己需要小心。

如果你正常使用手机，不在不同的系统镜像之间闪烁，那么你就没什么好担心的。然而，如果你是那种喜欢在不同版本之间跳跃的人，也许应该稍微推迟一下。目前还不清楚在更新到 Android 13 后，你是否会通过降级来损坏你的手机，但安全比遗憾好，等待并看看会发生什么。如果你使用的是老款谷歌 Pixel 手机，你也不需要担心这个问题。

至于为什么这只影响最新的 Pixel 手机，还不清楚。然而，所有这三种设备都由 Google Tensor 驱动，这意味着它可能是 Tensor 独有的东西，也可能是 Google 实现它的原因。防回滚保护是通过验证引导实现的[，将确保安全漏洞不会被恶意行为者用来安装旧版本的 Android 系统。](https://source.android.com/docs/security/verifiedboot/verified-boot#rollback-protection)

* * *

**来源:[安卓工厂图片页面](https://developers.google.com/android/images)**