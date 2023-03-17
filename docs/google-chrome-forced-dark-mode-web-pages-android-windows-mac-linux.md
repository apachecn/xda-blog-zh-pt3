# 谷歌 Chrome 在所有平台上的网页都强制进入黑暗模式

> 原文：<https://www.xda-developers.com/google-chrome-forced-dark-mode-web-pages-android-windows-mac-linux/>

随着有机发光二极管智能手机显示屏的日益普及，黑暗模式在各种平台上也越来越受欢迎。Android Q 带来了[原生黑暗模式](https://www.xda-developers.com/android-q-toggle-dark-theme/)，这使得许多开发者在他们的应用中涉足原生黑暗模式。谷歌本身已经在其许多应用程序中添加了单独的黑暗模式切换，包括[谷歌搜索](https://www.xda-developers.com/google-app-dark-theme-search-discover/)、[照片](https://www.xda-developers.com/google-photos-dark-theme-roll-out/)、[保存](https://www.xda-developers.com/google-keep-notes-dark-mode/)、[文件](https://www.xda-developers.com/files-by-google-dark-theme/)和[许多其他](https://www.xda-developers.com/tag/dark-theme/)。与此同时，已经有几次尝试在谷歌 Chrome 上以黑暗模式呈现网站，由于整个网络的 UI 元素范围更广，与应用程序相比，这似乎需要更长的时间。

早在 4 月，谷歌在测试版浏览器中添加了一个 [Chrome 标志来启用黑暗模式](https://www.xda-developers.com/google-chrome-android-dark-mode/)。这实际上是通过简单地改变 Chrome 版用户界面的颜色来实现的。最终，随着 Chrome 77 的更新，[黑暗模式明显变得更好了](https://www.xda-developers.com/google-chrome-77-improves-dark-mode-web-pages/),图像在黑暗模式下不再反转。但现在，有一个新的 Chrome 标志，用一个成熟的选项取代了早期的黑暗模式，强制所有网站进入黑暗模式。此选项在所有网站上启用背景，而不会还原颜色或破坏图像的可读性。

## 如何在谷歌浏览器中启用网页强制黑暗模式

1.  下载 Chrome Canary，这是一个正在开发的浏览器版本，每天都有新的实验性功能更新。
2.  在地址栏输入 **chrome://flags** 。在这里，你会发现 Chrome 的实验功能的标志或开关。
3.  在页面的搜索栏中，查找 ****对网页内容强制黑暗模式****
4.  点击下拉菜单，选择默认选项，并将其设置为启用。我发现“启用非图像元素的选择性反转”选项在我的 Android 上效果最好。
5.  系统将提示您重新启动浏览器。点击重新启动查看应用的更改。

这最有可能将网页的背景改为黑色，文本改为白色，同时保持其余的彩色元素不变。正如你在上面看到的，除了背景和文本，所有的颜色都保持不变。

如果您希望反转 UI 元素的颜色，您还可以从 HSL 和 CIELAB 中选择颜色配置文件，颜色反转将基于这些文件发生。

该功能适用于所有平台，包括 Android、Windows、Mac、Linux 和 ChromeOS。对我来说，这个功能在 Android 和 Mac 上都很稳定和一致，我希望它能很快转移到 Chrome 的开发频道。

* * *

**Via:[Techdows](https://techdows.com/2019/08/force-dark-mode-for-web-in-chrome-canary-on-desktop.html)**