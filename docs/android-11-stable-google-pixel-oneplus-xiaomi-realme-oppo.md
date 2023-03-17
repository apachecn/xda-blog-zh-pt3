# Android 11 现已为谷歌 Pixel 提供稳定版，并为一加、小米、Realme 和 OPPO 手机提供测试版

> 原文：<https://www.xda-developers.com/android-11-stable-google-pixel-oneplus-xiaomi-realme-oppo/>

Android 11 是世界上最受欢迎的智能手机操作系统的最新更新，首批稳定版本终于推出，以支持谷歌 Pixel 智能手机。我们经历了四次开发者预览( [DP 1](https://www.xda-developers.com/android-11-developer-preview-1-google-pixel/) 、 [DP 2](https://www.xda-developers.com/android-11-developer-preview-2-google-pixel-announcement-changelog/) 、 [DP 3](https://www.xda-developers.com/android-11-developer-preview-3-announced/) 和 [DP4](https://www.xda-developers.com/google-android-11-beta-june-3-2020-developer-preview-4-live-release/) )和三次测试版( [Beta 1](https://www.xda-developers.com/android-11-beta-1-update-live-google-pixel-2-3-3a-4-xl-device-controls-api-quick-settings-media-controls/) 、 [Beta 2](https://www.xda-developers.com/android-11-platform-stability-beta-2-available-google-pixel-2-3-3a-4-xl/) 、 [Beta 3](https://www.xda-developers.com/android-11-beta-3-here-remove-location-requirement-covid-19-contact-tracing-apps-exposure-notification-system/) )才走到这一步，我们已经尽我们所能[跟踪了一路上的每一个小细节](https://xda-developers.com/tag/android-11)。现在随着 Android 11 的稳定发布，我们终于可以期待谷歌的愿景到达世界各地的消费者手中了！

**[XDA 所有 Android 11 新闻](https://www.xda-developers.com/tag/android-11/)**

Android 11 有相当多的变化，但谷歌强调了一些主要的变化。

## Android 11 上的通信

### 通知阴影中的对话部分

跨消息应用的对话现在被移到通知部分的专用空间。这将更容易管理与人的持续对话，而不是让这些通知淹没在各种应用程序通知的洪流中。谷歌提到，如果你愿意，你也可以对关键人物的对话进行优先排序。这个对话部分最早出现在开发者预览版 1 中。

### 气泡

去年，我们曾指出 Android 10 中引入的 [Bubbles API 将如何在未来的 Android 版本中取代 overlay API。随着 Android 11 的推出，谷歌正在推动消息和聊天应用的开发者向气泡过渡，以便当用户在手机上进行多任务处理时，可以看到和访问对话。](https://www.xda-developers.com/android-q-system-alert-window-deprecate-bubbles/)

作为用户，你现在可以回复重要的对话，而不必在手机上的消息应用和其他应用之间来回切换。

### 内置屏幕录制

虽然你可以在 Android 早期截屏，但如果不需要第三方应用，你就无法在谷歌 Pixel 手机上真正记录你屏幕上的内容。谷歌 Pixel 的 Android 11 终于添加了一个内置的屏幕记录器，所以你可以轻松地捕捉和分享你的 Pixel 上发生的事情。您可以使用来自麦克风、设备(内部音频)或两者的声音进行录制。你不需要任何第三方应用就可以做到这一点。

Android 中的屏幕记录器最初是在 Android 10 开发者预览版中发现的，但在稳定版中用户无法使用该功能。它在 Android 11 开发者预览版 1 中再次被发现，[功能在开发者预览版 2](https://www.xda-developers.com/android-11-screen-recorder-internal-audio/) 中得到了更多的润色。

* * *

## Android 11 中的设备控件

Android 11 获得了新的电源菜单，允许您快速访问连接的智能设备。只需长按电源按钮即可进入新菜单，只需轻轻一按即可控制恒温器和智能锁等连接设备，无需打开多个应用程序。

有了这个新的补充，它终于感觉到[谷歌已经把智能手机带到了智能家居](https://www.xda-developers.com/android-11-power-menu-device-controls-smart-home-dream/)！

Android 11 上的媒体控件已经重新设计，现在在快速设置菜单中获得了一致的位置。您还可以使用快捷方式将媒体播放快速切换到另一台设备。

当[在开发者预览版 1](https://www.xda-developers.com/android-11-music-player-quick-settings-panel/) 中首次被发现时，快速设置面板中的新媒体播放器引起了不小的轰动。在开发过程中，用户界面得到了改进，功能本身也得到了升级，能够存储多达五个以前的媒体会话。

### 无线安卓汽车

Android 11 现在允许所有设备通过 Android Auto 无线工作，只要你有一个兼容的主机或售后接收器。[我们已经听说了](https://www.xda-developers.com/wireless-android-auto-works-android-11-devices-5ghz-wi-fi/)这一变化，谷歌正在确认无线 Android Auto 将需要支持 5GHz Wi-Fi 网络。因此，在欧盟、日本和俄罗斯的一些地区，由于对汽车中使用的 5GHz Wi-Fi 的特定要求，此功能将不可用。

* * *

## Android 11 上的隐私和数据

### 一次性权限

顾名思义，Android 11 允许用户对请求访问设备麦克风、摄像头或位置的应用程序授予一次性使用权限。下次应用程序需要访问这些设备功能时，它需要再次请求这些权限。

这个特性最初是在开发者预览版 1 中发现的，它允许用户临时授予一个应用程序访问权限，只要这个应用程序在前台。一旦用户离开应用程序，应用程序将失去访问权限，必须再次请求。这与 Android 10 中引入的行为不同，在 Android 10 中，当应用程序正在使用时，用户可以向应用程序“*”授予位置权限。*“一次性权限让用户能够更好地控制敏感权限。

### 权限自动重置

普通用户可能不记得在使用后撤销对敏感权限的访问，因此 Android 11 将自动重置应用程序的所有运行时权限，并通知用户该应用程序是否已超过*使用时间*。下次使用该应用程序时，该应用程序可以再次请求权限。

这一特性是在开发者预览版 3 中首次发现的，我们很高兴看到它在稳定版中出现。

### Google Play 系统更新—项目主线模块

Android 10 对于新推出设备最大的变化之一就是引入了[项目主线](https://www.xda-developers.com/android-q-project-mainline-security/)。Project Mainline 的目的是让 Google 从框架组件和系统应用程序的原始设备制造商手中夺走控制权，这些组件和应用程序对安全性和维护开发一致性至关重要。每个主线模块都封装在一个 APK 或一个 APEX 文件中，可以由 Google 通过 Play Store 更新。用户在他们的设备上将更新视为“Google Play 系统更新”(GPSU)，更新以火车的形式定期发布(即它们是同时下载和安装的)。

谷歌要求包含特定的主线模块，在谷歌 I/O 2019 时，包括 13 个。在 Android 11 开发者预览版 1 中，谷歌强制要求总共 20 个主线模块。现在，随着 Android 11 ( [从 Beta 1](https://www.xda-developers.com/android-11-beta-1-update-live-google-pixel-2-3-3a-4-xl-device-controls-api-quick-settings-media-controls/) 开始)，除了 Android 10 上现有的模块之外，谷歌还授权了总共 12 个主线模块。现在总共有 25 个模块。

### Android 企业变革

Android 11 为 Android 企业用户带来了一些变化，工作配置文件现在为组织的 IT 部门提供了管理设备的工具，而无需监控他们的个人配置文件数据或活动。谷歌的声明省略了大部分细节，但你可以在这里查看这些变化。

* * *

## Pixel 用户的专属功能

谷歌 Pixel 设备保留了一些新功能，可能会通过闭源 [Pixel Launcher](https://www.xda-developers.com/google-pixel-launcher-new-features-test-android-11/) 、设备个性化服务和其他 Pixel 专属应用程序提供。谷歌提到，受支持的 Pixel 设备将获得额外的工具来组织和管理手机，如基于日常事务的应用建议，选择文本和图像以及截图的新操作。

* * *

## Android 11:下载和推广

Android 11 将于今天开始在 stable 推出，适用于所有追溯到 Pixel 2 的 Pixel 设备，但测试版现在也适用于部分一加、小米、OPPO 和 Realme 智能手机。一加 8、一加 8 Pro、小米 10、小米 10 Pro、OPPO Find X2、OPPO Find X2 Pro、OPPO Ace2、OPPO Reno3 4G、OPPO Reno3 Pro 4G 和 Realme X50 Pro 是今天获得新 Android 11 测试版的设备。

### 为谷歌 Pixel 设备下载 Android 11

Android 11 更新应该会通过 OTA 更新到达您支持的 Google Pixel 设备。但如果它没有，你可以从以下链接下载支持谷歌 Pixel 设备的 Android 11，并非常容易地下载它:

**谷歌像素**

**GSI 下载**

您可以通过访问我们的 [Android 11 更新跟踪器](https://www.xda-developers.com/android-11-update-tracker/)文章来跟踪其他获得更新的手机。如果你想一窥内幕，谷歌也开始向 AOSP 上传 Android 11 源代码。我们当然会亲自挖掘 AOSP，所以请继续关注 Android 11 的更多新闻！

* * *

**你对 Android 11 有什么想法？你在你的设备上试过吗？请在下面的评论中告诉我们！**