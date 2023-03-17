# 适用于 Android TV 的 Android 13 发布了性能改进和附加功能

> 原文：<https://www.xda-developers.com/android-13-for-android-tv-releases/>

# 适用于 Android TV 的 Android 13 发布了性能改进和附加功能

Android TV 的 Android 13 现已上市，不过目前你只能在 ADT-3 和 Android 模拟器上使用它。

Android 是世界上最大的操作系统。它为全球超过 25 亿部智能手机提供支持，并且每年都会收到一个新的升级版本，对之前的版本进行了改进。它也支持 Chromecasts 等电视设备，并且可以像智能手机一样运行应用程序。安卓电视的最新版本是安卓 12，但现在谷歌正在为安卓电视推出安卓 13。

如果你是一个想尝试一下的开发者，Android 13 for Android TV 现在可以用于 ADT-3 和 Android TV emulator，它主要关注性能和可访问性。开发者在测试他们的应用程序时，将可以在 Android TV 和 Google TV 界面之间进行选择。

Android 13 为电视用户带来了新的 API，这将帮助开发人员为不同设备类型的用户提供高质量的体验。这些变化包括:

*   对 [AudioManager](https://developer.android.com/reference/android/media/AudioManager) API 的改进允许开发人员预测对活动音频设备的音频属性支持，并在不开始播放的情况下选择最佳格式。
*   用户现在可以在支持的 HDMI 源设备上更改默认的[分辨率和刷新率](https://developer.android.com/guide/topics/media/frame-rate)，以获得更可靠的播放体验。
*   HDMI 状态变化现在出现在 [MediaSession](https://developer.android.com/reference/android/media/session/MediaSession) 生命周期中，允许电视加密狗和其他 HDMI 源设备省电并暂停内容以响应 HDMI 状态变化。

Android 13 带来了新功能，使与电视的交互变得更具适应性和易用性，适合在导航电视时需要额外帮助的人，例如:

*   [输入设备 API](https://developer.android.com/reference/android/view/InputDevice#getKeyCodeForKeyLocation(int)) 现在支持不同的键盘布局。游戏开发者也可以通过按键的物理位置来引用按键，以支持物理键盘的不同布局。
*   在 [AccessibilityManager](https://developer.android.com/reference/android/view/accessibility/AccessibilityManager#isAudioDescriptionRequested()) 中新创建的音频描述 API 允许您的应用程序查询新的系统范围的音频描述偏好设置，帮助开发人员自动提供符合用户偏好的音频描述。

[其他功能包括](https://developer.android.com/tv/release/13/preview)用户控制刷新率和分辨率偏好、[电源管理改进](https://www.xda-developers.com/android-13-adds-a-new-low-power-standby-mode-for-android-tv-devices/)，以及更好的 HDMI 处理。目前还不清楚这一更新何时会推广到其他设备，鉴于[谷歌的 Chromecast 和谷歌电视最近才更新到 Android 12](https://www.xda-developers.com/chromecast-with-google-tv-android-12-update-rollout/) ，它可能需要一段时间才能更新到 Android 13。