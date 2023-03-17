# MIUI 可能很快会让你在后台预下载游戏内容

> 原文：<https://www.xda-developers.com/miui-predownload-game-data-feature/>

不管你喜欢它还是讨厌它，毫无疑问 MIUI 是功能最丰富的 Android 皮肤之一。它提供了过多的定制选项和工具，让您完全控制软件。很快，它甚至可以在后台更新你最喜欢的游戏。

在最新版本的 Mi 安全应用程序中，XDA 高级成员 [*kackrz*](https://forum.xda-developers.com/m/kacskrz.8240900/about) 发现了一个新的 MIUI 功能的证据，该功能将在新游戏更新可用时自动在后台下载它们。

```
 <string name="gb_predownload_dialog_message_china"><Data>"Updated content for this game can be downloaded to this device automatically after you connect to WLAN and turn the screen off. Thus, you'll be able to use the new version as soon as it's released.&lt;br>&lt;br>Read and agree to the &lt;a href=\"%1$s\">Statement on background updates&lt;/a> before using this feature."</Data></string>
<string name="gb_predownload_dialog_title">Background updates are available now</string> 
```

启用后，该功能可以在手机连接 Wi-Fi、屏幕关闭的情况下自动下载新的游戏内容。我们不确定字符串中的“predownload”具体指的是什么。基本的解释是，该功能将简单地下载新的游戏更新时，他们被释放。如果是这样的话，那就没那么重要了，考虑到 Play Store 早就提供应用自动更新了。但是看看下面的字符串，似乎“predownload”实际上意味着能够提前下载新的游戏内容——在开发者实际上在 app store 上发布更新之前。这样，用户就不必浪费时间下载新的更新，并可以在最新版本上线后立即开始播放。

```
 <string name="gb_predownload_noti_message">"%2$1.2f GB of updated content is already on this device. You'll be able to use it as soon as the new version is released."</string>
<string name="gb_predownload_noti_title">Updated %s in the background successfully</string> 
```

似乎后台下载功能只适用于特定的游戏，而且可能只适用于从小米应用商店下载的游戏。

```
 <string name="gb_predownload_message">"Update King of Glory, Game for Peace, and other compatible games in the background while you aren't using this device"</string> 
```

目前还不清楚后台游戏更新功能将仅限于中国版 MIUI 还是全球可用。我们也不知道小米计划何时向用户推出。