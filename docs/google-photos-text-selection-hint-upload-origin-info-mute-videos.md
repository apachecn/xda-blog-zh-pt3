# [更新:截图]谷歌照片在手机上增加了文本选择提示，在网上上传来源信息，并准备让你静音视频

> 原文：<https://www.xda-developers.com/google-photos-text-selection-hint-upload-origin-info-mute-videos/>

**更新 1 (4/20/2020 @美国东部时间下午 6:00):**在谷歌照片应用程序的 4.48 版本中，视频中的静音功能现在已经完全可用，尽管它还没有推出。

许多人认为谷歌照片是该公司最好的服务。如果你需要一个*免费的*功能丰富的照片和视频备份解决方案，很难击败谷歌照片。该公司正在[不断调整](https://www.xda-developers.com/google-photos-redesign-removes-hamburger-menu-moves-search/)用户界面和[添加新工具](https://www.xda-developers.com/google-photos-adds-private-messaging-share-photos/)。由 [*AndroidPolice*](https://www.androidpolice.com/2020/03/23/google-photos-text-selection-prompt-upload-information/) 发现的最新添加内容包括通过谷歌镜头在手机上进行文本选择提示，以及在网络上显示上传来源信息。我们还发现了一些迹象，表明你很快就可以在编辑视频时静音。

首先，Google Photos 移动应用程序中出现了一个新的文本选择提示。当您打开包含文本的图像时，会弹出提示建议“从图像中拷贝文本”点击它会将你带到谷歌镜头界面，在那里你可以选择文本并采取行动，如谷歌搜索，翻译或复制文本。你可以通过手动点击谷歌镜头按钮来实现这一点，但现在这款应用程序实际上会向你建议。

接下来是谷歌照片网页版的一个功能。你终于可以在“信息”部分看到上传的图片和视频来自哪里了。“你会看到“从电脑上传，从安卓设备上传，从 Google Drive 上传”等。这仅适用于你自己上传的图片，而不适用于其他人分享的图片。

最后，我们发现谷歌正准备增加静音功能。谷歌照片 4.44 APK 包括提到“静音音频”和“静音视频”的字符串，以及其他与静音相关的字符串。这意味着您可以在编辑时关闭视频中的音频。如果你曾经有过视频被音频毁了，你知道这是一个伟大的功能。

```
 <string name="photos_videoeditor_a11y_mute_audio">Mute audio</string>
<string name="photos_videoeditor_a11y_mute_disabled">Mute button is disabled for silent videos</string>
<string name="photos_videoeditor_a11y_unmute_audio">Turn audio on</string>
<string name="photos_videoeditor_action_mute">Mute</string>
<string name="photos_videoeditor_cpe_mute_applied">Muted</string>
<string name="photos_videoplayer_mute_button">Mute video</string>
<string name="photos_videoplayer_unmute_button">Unmute video</string>

```

前几个功能现在似乎可以在各自平台的 Google 相册中使用。静音功能还没有上线，但看起来谷歌准备很快加入这一功能。很高兴看到谷歌继续改进它最好的服务之一。

## 更新:静音视频现在可以了

当这篇文章在上个月首次发表时，我们只发现了暗示能够静音视频音频的字符串。现在，我们已经在最新版本的谷歌照片应用中启用了这一功能，继[简·满春·王今天早些时候做了同样的](https://twitter.com/wongmjane/status/1252291336788557825)之后。如下图所示，一个新的音量图标将出现在视频编辑器界面的左下角。轻按此按钮将使您当前正在编辑的视频中的音频静音。然后，您可以保存编辑过的视频的副本。

这项功能尚未向用户推出，但我们会密切关注，并在推出时通知您。