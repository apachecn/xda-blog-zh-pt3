# Android 11 测试版为谷歌 Pixel 手机提供设备控制 API、气泡通知等功能

> 原文：<https://www.xda-developers.com/android-11-beta-1-update-live-google-pixel-2-3-3a-4-xl-device-controls-api-quick-settings-media-controls/>

Android 11 是下一个主要的 Android 版本更新，该更新的第一个公共测试版[计划在 2020 年 6 月 3 日](https://www.xda-developers.com/google-android-11-beta-june-3-2020-developer-preview-4-live-release/)的在线活动后发布。由于目前美国的内乱，谷歌选择推迟在线发布活动，尽管第一个测试版意外地[最终出现在一些用户的手机上](https://www.xda-developers.com/android-11-beta-1-rolled-out-early-some-google-pixel-4-users-whats-new-changes-features/)。现在，谷歌宣布全面取消在线发布活动。但不用担心，Android 11 Beta 1 仍在向前发展。谷歌正式发布了谷歌 Pixel 手机的第一个测试版，带来了几个围绕人、控制和隐私等关键主题的新变化。

**[安卓 11 XDA 新闻](https://www.xda-developers.com/tag/android-11/)**

第一个 Android 11 测试版今天推出，包括最终的 SDK 和 SDK and，以及应用程序中可以尝试的新功能。如果

如果您有 Pixel 2、Pixel 3、Pixel 3a 或 Pixel 4 设备，您可以向 Google 注册，直接通过无线方式将 Android 11 Beta 更新下载到您的设备上。和往常一样，如果你想下载最新的更新，也可以下载 Pixel 和 Android 模拟器。

谷歌也在重新设计 Play 控制台，并为 Android Studio、Kotlin 和 Jetpack 添加新功能。你可以在我们的另一篇文章中读到所有这些变化。

## 为谷歌 Pixel 设备下载 Android 11 Beta 1

在我们进入 changelog 之前，您可以从以下链接下载适用于受支持的 Google Pixel 设备的 Android 11 Beta 1:

### 谷歌像素

### GSI 下载

为了让事情变得更简单，你可以使用 [Android 闪存工具](https://developer.android.com/preview/download#flashtool)安装测试版，而不是通过恢复或快速启动手动刷新。

*注意:随着下载链接的上线，我们将更新此图表。*

* * *

## Android 11 Beta 1 的变化

谷歌的新闻稿没有独立列出 Android 11 Beta 1 中引入的所有变化。相反，新闻稿缩小了下一个 Android 操作系统版本的变化。记住我们已经接入了 [Android 11 开发者预览版 1](https://www.xda-developers.com/android-11-developer-preview-1-google-pixel/) 、[预览版 2](https://www.xda-developers.com/android-11-developer-preview-2-changes/) 、[预览版 3](https://www.xda-developers.com/android-11-developer-preview-3-changes/) 、[预览版 4](https://www.xda-developers.com/google-android-11-beta-june-3-2020-developer-preview-4-live-release/) ，最近[甚至是今天发布](https://www.xda-developers.com/android-11-beta-1-rolled-out-early-some-google-pixel-4-users-whats-new-changes-features/)之前的 Beta 1。因此，如果你一直密切关注我们的报道，以下所有变化对你来说可能并不陌生。

**[Android 11 Beta 1 向部分 Pixel 4 用户提前推出:以下是最新消息](https://www.xda-developers.com/android-11-beta-1-rolled-out-early-some-google-pixel-4-users-whats-new-changes-features/)**

谷歌专注于 Android 11 的三个关键主题:**人、控制和隐私**。

### 人

我们的智能手机已经发展到提供多种功能，但它的主要功能之一仍然是与人建立联系和保持沟通。因此，Android 11 将试图重新调整操作系统，使其更加以人为本，更具表现力。

#### **对话通知**

Android 11 将在通知阴影的顶部有一个专门的部分，专门用于对话。据说这种设计是“以人为本”的，通知本身将提供特定于对话的操作，如以气泡形式打开对话，在主屏幕上创建对话快捷方式，或设置提醒。

*来自开发者预览版 1 的对话通知*

对话通知最早出现在 Android 11 开发者预览版 1 。除了实际对话的常见上下文回复，我们还可以发现打盹、静音、收藏的动作区域，并在气泡中查看对话。

#### **气泡**

说到泡泡，Android 11 在消息聊天头上使用了泡泡 API。消息和聊天应用“应该”使用 Bubbles API 进行通知，以允许用户在多任务处理时查看和访问他们的对话。

Android 10 中引入了气泡作为开发者选项，但我们知道谷歌打算用它们做更多的事情。自 Android 11 开发者预览版 1 起，气泡通知已默认启用，如中所示，您不再需要在开发者选项中启用该选项。

在 Android 11 Beta 1 中，谷歌增加了启用气泡通知的新子菜单。此子菜单位于“设置”>“应用程序与通知”>“通知”>“气泡”。

在 Android 11 Beta 1 中，谷歌增加了启用气泡通知的新子菜单。此子菜单位于“设置”>“应用程序与通知”>“通知”>“气泡”。

**综合键盘建议**

#### 这使得自动填充应用程序和输入法编辑器(IME)可以直接在 IME 的建议条中安全地提供特定于上下文的实体和字符串，这对于用户来说是最方便的。

从声音上看，统一键盘建议将被允许直接向键盘应用的单词建议栏提供其存储的条目。我们将很快更详细地探讨这个特性是如何工作的。

从声音上看，统一键盘建议将被允许直接向键盘应用的单词建议栏提供其存储的条目。我们将很快更详细地探讨这个特性是如何工作的。

**语音接入**

#### 很容易认为触摸屏交互是理所当然的，但是有一部分用户发现触摸屏的使用很麻烦、很困难或者不可能。这些用户依靠辅助功能命令通过语音命令来导航他们的智能手机。Android 11 现在包括一个设备上的视觉皮层，它可以理解屏幕内容和上下文，并为可访问性生成标签和访问点。

控制

* * *

### 本节重点介绍互联家庭生态系统，将 Android 置于所有其他智能设备的指挥中心。

本节重点介绍互联家庭生态系统，将 Android 置于所有其他智能设备的指挥中心。

**设备控制 API**

#### 设备控制 API 是 Android 11 的亮点功能之一。在这个 Android 版本中，用户只需长按电源按钮，就可以快速轻松地访问和控制他们的连接设备。

控件 API 让开发者[将家庭自动化快捷方式放入电源菜单](https://www.xda-developers.com/android-11-quick-control-shortcuts-power-menu/)。在 Android 11 的早期预览版中，顶部电源菜单项下方有一个“快速控制”部分，而电源菜单的其余部分是透明的。

在 Android 11 开发者预览版 4 中，电源菜单背景是深色的，包括顶部的电源菜单项。此外，“快速控制”现在说“设备控制”，并且当字段为空时有一个描述文本，说“为您连接的设备添加控制”。当您从支持的应用程序添加控件时，此文本会消失，以便为您喜爱的控件腾出空间。

Android 11 Beta 1 为所有人带来了新的“电源菜单”设置，这将控制卡和通行证，并控制电源菜单内的功能。

Google Home 应用[已经支持 Android 11 的设备控制 API](https://www.xda-developers.com/google-home-android-11-device-controls/) 。用户已经能够从 Google Home 应用程序中让设备显示在开发者预览版 4 的电源菜单中，你应该也能够在 Beta 1 上做到这一点。

Google Home 应用[已经支持 Android 11 的设备控制 API](https://www.xda-developers.com/google-home-android-11-device-controls/) 。用户已经能够从 Google Home 应用程序中让设备显示在开发者预览版 4 的电源菜单中，你应该也能够在 Beta 1 上做到这一点。

**媒体控制**

#### 媒体控制使用户能够快速方便地切换音频或视频内容的输出设备，让他们在连接的设备之间进行选择，如设备扬声器、耳机、外部扬声器、电视等。这一功能可以在 Beta 1 的开发者选项中启用，Google 承诺在即将到来的 Beta 版本中将默认启用该功能。

我们[在开发者预览版 2](https://www.xda-developers.com/android-11-multi-device-media-output-wired-headset-audio-switching/) 中发现了多设备音频切换的暗示。而现在，谷歌也正式宣布了同样的消息。请注意，某些 Android 皮肤已经允许您选择输出设备，现在，这一功能已经在 stock Android 上实现。

隐私

* * *

### 谷歌对全操作系统隐私的关注在 Android 11 中得以延续。

谷歌对全操作系统隐私的关注在 Android 11 中得以延续。

**一次性权限**

#### 顾名思义，Android 11 允许用户对请求访问设备麦克风、摄像头或位置的应用程序授予一次性使用权限。下次应用程序需要访问这些设备功能时，它需要再次请求这些权限。

这个特性最初是在开发者预览版 1 中发现的，它允许用户临时授予一个应用程序访问权限，只要这个应用程序在前台。一旦用户离开应用程序，应用程序将失去访问权限，必须再次请求。这与 Android 10 的行为不同——在 Android 10 上，用户可以在“应用程序正在使用时”向应用程序授予位置权限，这意味着人们只能为位置权限而这样做，并且应用程序每次打开时都可以访问位置。一次性权限是一个更窄的工作区域，涵盖了更多的权限。

这个特性是[在开发者预览版 1](https://www.xda-developers.com/android-11-developer-preview-privacy-security-features-changes/) 中首次发现的，它允许用户临时授予一个应用程序访问权限，只要这个应用程序在前台。一旦用户离开应用程序，应用程序将失去访问权限，必须再次请求。这与 Android 10 的行为不同——在 Android 10 上，用户可以在“应用程序正在使用时”向应用程序授予位置权限，这意味着人们只能为位置权限而这样做，并且应用程序每次打开时都可以访问位置。一次性权限是一个更窄的工作区域，涵盖了更多的权限。

**权限自动重置**

#### 基于一般用户在使用后不记得撤销应用程序权限的想法，Android 11 将自动重置应用程序的所有运行时权限，并在应用程序“长时间”未使用时通知用户。下次使用该应用程序时，该应用程序可以再次请求权限。

这一特性是在开发者预览版 3 中首次发现的，看起来将会包含在未来的测试版中。

这个新特性是在开发者预览版 3 中首次发现的[，看起来将会包含在未来的测试版中。](https://www.xda-developers.com/android-11-developer-preview-3-changes/)

**背景位置**

#### 谷歌发现，许多应用程序在后台访问位置数据，而实际上并没有任何真正的需求。因此，2020 年 2 月，[谷歌宣布](https://www.xda-developers.com/android-apps-background-location-google-approval/)寻求后台位置访问的应用开发者需要获得谷歌的批准，以防他们想在 Play Store 上列出他们的应用。因此鼓励开发者评估他们的应用是否真的需要访问后台位置，以及这种需求是否有正当理由。

此前，谷歌已经宣布了实施这一新变化的时间表。从 2020 年 8 月起提交的所有新应用和从 2020 年 11 月起提交的所有现有应用都需要获得后台位置访问批准，否则应用列表将不会上线/会被移除。谷歌现在延长了时间表，但只是为了对现有应用执行政策，让开发者在 2021 年之前有时间在他们的列表被删除之前获得批准。

这一变化实际上独立于 Android 11，因为应用程序将从谷歌 Play 商店中完全删除。但它确实与这个 Android 版本中隐私和权限管理的总体主题相联系。

Google Play 系统更新—项目主线模块

### Android 10 对新推出的设备的最大变化之一是引入了[项目主线](https://www.xda-developers.com/android-q-project-mainline-security/)。Project Mainline 的目的是让 Google 从原始设备制造商手中夺取对安全性和维护开发一致性至关重要的框架组件和系统应用程序的控制权。每个主线模块都被封装成一个 APK 或者一个 [APEX 文件](https://www.xda-developers.com/android-q-apex-biggest-thing-since-project-treble/)，并且可以由 Google 通过 Play Store 更新。用户在他们的设备上将更新视为“Google Play 系统更新”(GPSU)，更新以火车的形式定期发布(即它们是同时下载和安装的)。

谷歌要求包含特定的主线模块，在谷歌 I/O 2019 时，包括 13 个。在 Android 11 开发者预览版 1 中，谷歌强制要求总共 20 个主线模块。

现在，随着 Android 11 Beta 1 的推出，除了 Android 10 上现有的模块之外，谷歌还授权了总共 12 个主线模块。现在总共有 25 个模块。

Android 11 测试版中对开发者友好的变化

* * *

### 这不是 Android 11 中变化的主要焦点之一，但它形成了测试版的一个焦点，因为更新是专门针对应用程序开发人员的。这些变化如下:

在开发人员瞄准 Android 11 之前，这些变化是有限制的，所以在您明确更改清单之前，这些变化不会生效。

*   在开发者选项中增加了一个新的 UI，让你可以切换这些应用测试的突破性变化(2020 年 1 月发现的)。
*   添加了一个新的平台稳定性发布里程碑，在该里程碑中，所有 API 和行为更改都将完成，因此应用程序开发人员可以在了解平台本身稳定的情况下完成应用程序更新。
*   无线 ADB 调试([预计 2019 年 10 月](https://www.xda-developers.com/android-11-native-wireless-adb/)，然后[如开发者预览 2](https://www.xda-developers.com/android-11-developer-preview-2-changes/) 所见)
*   ADB 增量，用于更快安装大型 apk([见开发者预览版 4](https://www.xda-developers.com/android-11-developer-preview-3-announced/) )
*   平台 API 上更多的可空性注释，用于在构建时而不是运行时捕捉问题。
*   这些只是谷歌在公告中提到的变化，但肯定会有更多他们没有指明的变化。当 [Android 11 Beta 1 意外推出](https://www.xda-developers.com/android-11-beta-1-rolled-out-early-some-google-pixel-4-users-whats-new-changes-features/)时，我们已经挖出了一些，例如公告中没有提到的快速设置媒体控件。现在，随着 Pixel 智能手机上的更新可供我们使用，我们将能够更好地定位更多的变化。敬请期待！

* * *

这些只是谷歌在公告中提到的变化，但肯定会有更多他们没有指明的变化。当 [Android 11 Beta 1 意外推出](https://www.xda-developers.com/android-11-beta-1-rolled-out-early-some-google-pixel-4-users-whats-new-changes-features/)时，我们已经挖出了一些，例如公告中没有提到的快速设置媒体控件。现在，随着 Pixel 智能手机上的更新可供我们使用，我们将能够更好地定位更多的变化。敬请期待！

**[安卓 11 XDA 新闻](https://www.xda-developers.com/tag/android-11/)**

**[Android 11 XDA 新闻](https://www.xda-developers.com/tag/android-11/)**