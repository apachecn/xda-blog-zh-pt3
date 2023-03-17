# Android 14 可以让你在你的像素上创建一个表情壁纸

> 原文：<https://www.xda-developers.com/android-14-emoji-wallpaper/>

今天早些时候，谷歌推出了 Android 14 第二个开发者预览版[，](https://xda-developers.com/android-14)[带来了](https://www.xda-developers.com/android-14-developer-preview-2-is-here-with/)我们[之前告诉你的](https://www.xda-developers.com/android-14-photo-picker-forced/)精选照片访问功能。与往常一样，新版本中的许多新功能在默认情况下是不可见的，这就是为什么我们要煞费苦心地梳理每个版本以记录新功能。我们的最新发现是一个似乎是 Pixel 手机独有的功能:表情壁纸。

早在一月份，*纽约时报* [发表了一篇文章](https://www.nytimes.com/2023/01/20/technology/google-chatgpt-artificial-intelligence.html)详细描述了谷歌计划如何对抗 ChatGPT 带来的威胁。在信中，他们还展示了该公司正在进行的一些图像和视频项目，包括“Pixel 智能手机的壁纸制造商”在 Android 14 DP2 中，我们在/product 分区中发现了一个新的“表情壁纸”应用程序。正如我刚才提到的，这个应用程序似乎是像素专用的，因为它的包名称是“com . Google . Android . apps . emojiwallpaper”，并且它需要声明功能标志“com . Google . Android . feature . Pixel _ EXPERIENCE”。

默认情况下，表情壁纸选择器是不活动的，但在切换了调试标志后，我可以在壁纸&选择器应用程序中显示它。一旦启用，壁纸列表中就会出现一个新的“表情实验室”选项。点击它打开了一个用户界面，让我用各种表情符号创建一个新的壁纸。在创建壁纸时，你可以选择多达 14 个表情符号来包含在设计中，从像“马赛克”、“莲花”、“堆栈”、“喷洒”、“棱镜”这样的图案中进行选择，并在各种颜色之间进行选择。如果你不知道你想要什么样的设计，你可以点击“随机化”按钮，让应用程序创建一个随机化的表情符号壁纸。

创建表情壁纸后，您的作品会被保存，并显示在壁纸&样式>壁纸>表情实验室下。该应用程序可以保存你创建的多个表情壁纸，你可以在列表中点击它们，然后点击“设置壁纸”，在它们之间切换你也可以点击铅笔图标来编辑你已经创建的表情壁纸。你也许可以分享你创建的表情壁纸，但是在我最初的挖掘中，我还没有能够展示这个功能。

正如我之前提到的，这个功能在 Android 14 DP2 中是默认不启用的。因此，当 Android 14 的稳定版本发布用于 Pixel 手机时，不能保证它会可用。