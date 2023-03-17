# Android 14 将允许你限制应用程序可以访问的照片，即使它们不使用照片选择器

> 原文：<https://www.xda-developers.com/android-14-photo-picker-forced/>

Android 13 的亮点之一是照片选择器，这是一个新的系统组件，让用户选择哪些照片和视频可以让应用程序访问。应用程序不需要请求任何权限来访问用户通过照片选择器选择的项目，这使得它成为一种保护隐私的方式来与应用程序共享照片和视频。自 Android 4.4 以来一直存在的系统文件选择器提供了比照片选择器更多的功能，但相比之下，它的用户界面已经过时了。

照片选择器(及其之前的系统文件选择器)允许您限制应用程序可以访问的照片和视频，从而保护您的隐私。不幸的是，许多应用程序不支持照片选择器，尽管它的向后兼容版本可用于 Android 4.4+。应用程序必须使用意图来专门调用照片拾取器，但许多应用程序出于这样或那样的原因选择不使用它。幸运的是，这在 [Android 14](https://www.xda-developers.com/android-14/) 中可能不再重要，它正在测试一种方法，让用户选择哪些照片和视频应用程序可以通过照片选择器访问，不管这些应用程序是否实际使用该 API。

许多应用程序通过[媒体商店 API](https://developer.android.com/training/data-storage/shared/media) 访问媒体文件。该系统根据文件的类型(称为媒体商店收藏)对文件进行索引，并维护一个应用程序可以使用媒体商店 API 查询的数据库。使用 media store API 的应用程序不需要请求权限来读取或修改它们自己的文件，但是它们需要用户授予权限来访问其他应用程序拥有的文件。

从 Android 10 开始，针对 API 级别 29 或更高的应用程序必须由用户授予 READ_EXTERNAL_STORAGE 权限，才能使用媒体商店 API 访问其他应用程序拥有的文件。在 Android 13 中，READ_EXTERNAL_STORAGE 权限被分为三个不同的权限(READ_MEDIA_AUDIO、READ_MEDIA_VIDEO 和 READ_MEDIA_IMAGES)，每个权限都授予面向 API 级别 33 的应用程序使用 media store API 分别访问其他应用程序拥有的音频、视频和图像文件的能力。

Android 14 通过将 READ_MEDIA_VIDEO、READ_MEDIA_IMAGES、ACCESS_MEDIA_LOCATION 合并为一个名为 READ _ MEDIA _ VISUAL _ USER _ SELECTED 的新权限，再次改变了媒体访问权限。根据其描述，该权限允许以 API 级别 34 为目标的应用程序“从共享存储中读取用户选择的图像和视频文件”。然而，Android 14 可能会将这一新行为追溯应用到现有的以 API 级别 33 为目标的应用程序(即 Android 13)并请求 READ_MEDIA_VIDEO 或 READ_MEDIA_IMAGES。

当一个以 API 级别 33 为目标的应用程序触发运行时权限对话框，要求用户授予他们 READ_MEDIA_VIDEO 或 READ_MEDIA_IMAGES(或两者都有)时，Android 14 可能会在权限对话框中插入一个新条目，上面写着“选择照片”。点击此条目将启动新版本的照片选择器，允许用户选择他们希望授予应用程序访问权限的照片或视频。该应用随后只能访问用户特别选择的那些媒体项目，除非用户选择扩展对附加媒体项目的访问，或者授权该应用访问图像和视频的整个媒体商店集合。

权限对话框中的这个条目在 Android 14 DP1 中默认不显示，因为它的可见性由我必须切换的开发者标志控制。然而，如果这项功能得以发布，这将是隐私方面的一大胜利，因为这意味着用户将始终有能力决定一个应用程序应该访问哪些照片或视频。

很少有应用程序像现在这样使用照片拾取器 API，这促使谷歌尝试用[拦截应用程序用来启动系统文件拾取器的现有意图](https://blog.esper.io/android-photo-picker-rollout/),以便它们转而启动照片拾取器。虽然照片拾取器有一些缺陷，例如还不能显示来自云媒体提供商的文件(也许随着[扩展 SDK](https://www.xda-developers.com/google-releases-extension-sdk/) 版本 5 的推出，它很快就会显示出来了！)和[只在设备上显示某些相册](https://twitter.com/MishaalRahman/status/1615059118003306496)，这比旧的系统文件选择器要好，当然也比每个应用程序都能访问图库中的每张照片和视频更好。

有兴趣实现 Photo Picker API 的开发者应该升级到最新版本的[Jetpack 活动库](https://twitter.com/ianhlake/status/1618380694702657536)，它处理调用通过 Android 4.4-Android 10 上的 Google Play 服务提供的向后兼容版本或者通过[media provider 主线模块](https://blog.esper.io/android-photo-picker-backport/)提供的框架提供的版本。