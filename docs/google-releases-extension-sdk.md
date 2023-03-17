# 谷歌发布扩展 SDK，为旧版本 Android 带来新功能

> 原文：<https://www.xda-developers.com/google-releases-extension-sdk/>

# 谷歌发布扩展 SDK，为旧版本 Android 带来新功能

扩展 SDK 使得像照片选择器这样的功能在旧的 Android 版本上成为可能。

[项目主线](https://www.xda-developers.com/android-project-mainline-modules-explanation/)是谷歌通过 Google Play 服务框架和谷歌 Play 商店向一些关键系统组件提供更新的一种方式。每个主线模块都以 APK 文件、APEX 文件或 APEX 中的 APK 文件的形式交付。当主线模块正在更新时，用户会在他们的设备上看到“Google Play 系统更新”(GPSU)通知。实际上，为了向关键组件提供更新，谷歌已经绕过了等待 OEM 厂商推出更新的需要，选择自己完成这项任务。该公司现在已经发布了扩展 SDK 的第一个公共版本，并通过系统模块交付给设备。

扩展 SDK 对开发者最大的效用是能够将新的照片拾取器 API 带到运行 Android 11 和更新版本的设备上，尽管这是随着 [Android 13](https://www.xda-developers.com/android-13) 推出的一项功能。谷歌还表示，开发者将能够实现广告服务 API，为测试预计将于今年晚些时候推出的[安卓隐私沙箱](https://www.xda-developers.com/android-privacy-sandbox-developer-preview-5/)做好准备。这是一个如何使用扩展 SDK 将功能移植到旧的 Android 版本而不需要整个系统更新的例子。

开发人员可以通过在运行时查询扩展版本来检查用户设备上安装的扩展 SDK 的版本，就像他们检查其他设备属性一样，比如内部版本。AdServices API 已经被添加到 Extension SDK 版本 4 中，但是 Photo Picker 从版本 2 就已经存在了。

对于使用 Android Studio Flamingo 或更新版本的开发人员来说，他们将能够为通过扩展 SDK 启动的 API 自动生成正确的版本检查。它完全是可选的，但是可以帮助开发人员实现新的可用特性。你可以阅读更多关于 [SDK 扩展](https://developer.android.com/sdkExtensions)和关于[隐私沙盒测试版](http://developer.android.com/design-for-safety/privacy-sandbox/program-overview?version=beta)和[照片拾取器](https://developer.android.com/training/data-storage/shared/photopicker)的文档。