# 你的安卓手机可以无缝地作为网络摄像头工作，并有即将到来的软件更新

> 原文：<https://www.xda-developers.com/android-continuity-camera-gerrit-commits/>

虽然此时细节匮乏，但我们知道 [Android 14](https://www.xda-developers.com/android-14/) 即将到来。虽然你目前可以使用智能手机和成熟的摄像头作为网络摄像头，但大多数需要[一些额外的软件甚至硬件](https://www.xda-developers.com/how-to-use-android-phone-as-webcam-for-pc/)才能做到这一点。这就是为什么[苹果的连续性相机](https://www.xda-developers.com/apple-shows-how-continuity-camera-will-work-with-your-iphone-and-mac/)如此伟大，因为它允许你拿现有的产品，并通过软件的魔力将它们配对在一起。当然还有[一些要求](https://www.xda-developers.com/how-to-use-continuity-camera-macos/)，但是极其方便。现在，一个 Android 的等价物可能即将出现，因为新发现的对 Android 开源项目(AOSP) Gerrit 的承诺暗示这可能在不久的将来到来。

斯珀*的 mishal Rahman*发现了这一变化，推出了一项新的“[devices as web cam](https://android-review.googlesource.com/c/platform/system/sepolicy/+/2410788)”服务，允许 Android 设备充当网络摄像头。当然，并不是每一个设备都会得到支持，但拉赫曼认为，只要设备满足最低要求，到目前为止，看起来是对 UVC 小工具模式的内核支持，它应该允许像相机一样的连续性连接。拉赫曼对此进行了进一步的阐述，他说:“系统属性' [ro.usb.uvc.enabled](https://android-review.googlesource.com/c/platform/system/sepolicy/+/2410787) '将用于切换 Android 设备上的 uvc 小工具功能。它[只能由系统应用](https://android-review.googlesource.com/c/platform/system/sepolicy/+/2415830)读取，具体来说，设置应用和 USB 小工具 HAL 会读取它。”

这些变化可以在当前具有 root 访问权限的设备上看到和启用，但你无法让事情正常工作，因为目前没有办法从 Android 设备传输视频。虽然这一切听起来令人印象深刻，但拉赫曼警告说，他不知道这将如何进行，也不知道这一功能是否会在未来的 Android 版本中出现。这意味着我们可能要等一段时间才能真正发布，或者根本看不到它。但如果真的如此，这可能是人们即时升级网络摄像头的一个好方法，不需要额外的设备或软件。

苹果的连续性相机于去年推出，尽管它要求用户运行 [macOS Ventura](https://www.xda-developers.com/macos-ventura-review/) 和 [iOS 16](https://www.xda-developers.com/ios-16/) ，但它提供了一种非凡的体验，可以将你的 iPhone 变成一个高性能的网络摄像头。作为一个使用过连续相机的人，这是一个令人印象深刻的功能，改善了我笔记本电脑上糟糕的相机质量，效果非常好。希望 Android 用户能够很快体验到这种魔力，但如果不能，至少还有 DroidCam 这样的选项。

虽然有不同的应用程序和选项，但 DroidCam 是整体上最好的之一，为您提供高质量的图像，并提供相对平稳的设置过程。在大多数情况下，你只需要在你的智能手机和 PC 上下载应用程序，让这两个设备在同一个网络上，设置一些 IP 地址(显示在智能手机应用程序中)，就这样，它应该开始工作。您可以随时使用下面的链接下载试用该应用程序。

* * *

**来源** : [米沙勒·拉赫曼](https://t.me/MishaalAndroidNews/239)(电报)