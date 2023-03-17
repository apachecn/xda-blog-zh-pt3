# 让 Android 10 的隐藏桌面模式更有用

> 原文：<https://www.xda-developers.com/make-android-10-desktop-mode-useful/>

# 让 Android 10 的隐藏桌面模式在一加 7/7T 和 Essential 手机上更有用

如果你有一部运行 Android 10 的智能手机，那么你可能不知道还有一个隐藏的桌面模式。以下是让它更有用的方法。

在 Android 10 发布之前，人们谈论最多的功能之一[就是桌面模式。当我们第一次听说谷歌的下一个主要 Android 操作系统将原生支持桌面模式时，我们希望它会类似于三星 DeX 或华为 Easy Projection。可悲的是，它](https://www.xda-developers.com/android-q-dark-theme-desktop-mode-permission-revamp/)[绝不是](https://www.xda-developers.com/android-q-desktop-mode/)。谷歌为外部显示器[建立了一个准系统启动器，这样开发者可以测试](https://www.xda-developers.com/google-more-information-desktop-mode-android-q/)他们的应用在大显示器上可能会是什么样子，但他们甚至没有费心在 Pixel 4 上添加显示输出支持[。可悲的是，这意味着 Android 10 的隐藏桌面模式在最新的 Pixel 智能手机上无法使用，但如果你有 Essential Phone，一加 7/7 Pro，一加 7T/7T Pro，或任何其他通过 USB-C 输出视频的手机，那么有一种方法可以让它更有用。](https://www.xda-developers.com/google-pixel-4-what-you-missed/)

首先，您必须满足以下一些要求:

**要求:**

1.  你的安卓智能手机必须运行安卓 10。
2.  您的 Android 智能手机需要支持 [DisplayPort Alt 模式。](https://vesa.org/featured-articles/vesa-highlights-growing-adoption-of-displayport-over-usb-c-new-codec-for-handheld-device-specific-display-interface-compression-at-mobile-world-congress/)这里是[部分支持](https://en.everybodywiki.com/List_of_devices_with_video_output_over_USB-C)的手机列表。如果您的智能手机带有高通骁龙 835、高通骁龙 845 或高通骁龙 855 以及 USB 3.1 Type-C 端口，那么您的智能手机应该支持 DisplayPort Alt 模式，除非手机供应商故意禁用它。例如，谷歌在 Pixel 4 上禁用了它。
3.  你需要一个 USB 3.1 Type-C 转 HDMI 适配器。我在亚马逊上买了这个。如果你想要更愉快的体验，你还需要一个蓝牙鼠标和键盘。

接下来，下面是如何设置它:

1.  在手机上启用开发者选项。进入设置>关于电话，并点击“建立号码”7 次。
2.  进入“设置”>“开发者选项”,向下滚动直到你看到“应用程序”部分。打开“启用自由形式窗口”和“强制桌面模式”
3.  重启你的手机。
4.  [安装这个 APK](https://github.com/farmerbb/libtaskbar-Lawnchair-Example/releases/download/libtaskbar/Lawnchair-quickstep-lawnchair-dev-debug.apk) 。这是流行的 [Lawnchair](https://play.google.com/store/apps/details?id=ch.deletescape.lawnchair.plah) 启动器的定制版本，集成了[任务栏](https://play.google.com/store/apps/details?id=com.farmerbb.taskbar)。这款 APK 由 XDA 资深会员 [farmerbb](https://forum.xda-developers.com/member.php?u=4289533) 制作，作为概念验证，向定制启动器开发者展示他们如何添加桌面模式支持*。
5.  前往“设置”>“应用与通知”>“默认应用”,将 Lawnchair 设置为默认启动器。
6.  使用适配器将手机插入显示器/电视。
7.  几秒钟后，你应该会看到自定义的 Android 10 桌面界面出现在屏幕上。你必须按照要求授予任务栏“在其他应用上显示”的权限，才能显示底部栏。如果你也想让任务栏在底部显示你最近的应用，你也应该按照要求授予它“使用访问”权限。

我敢打赌，现在你的显示器/电视上所有的东西看起来都太大了。那是因为 Android 10 中桌面模式的默认 DPI 是 320，这让一切看起来都很巨大。此外，导航栏/Android 10 手势导航药丸在您的显示器上可能看起来不雅观。有一种方法可以解决这个问题，但需要 farmerbb 安装另一个应用程序。

1.  断开手机与显示器/电视的连接，并将其连接到 PC。
2.  [在您的电脑上下载并安装 ADB](https://www.xda-developers.com/install-adb-windows-macos-linux/)。
3.  从谷歌 Play 商店安装[第二屏](https://play.google.com/store/apps/details?id=com.farmerbb.secondscreen.free)。确保你的应用程序版本为 2.9.1，支持 Android 10 桌面模式(如 changelog 中所述。)
4.  按照应用程序的指示，从您的电脑上运行以下命令:

    ```
     adb shell pm grant com.farmerbb.secondscreen.free android.permission.WRITE_SECURE_SETTINGS 
    ```

5.  现在，您可以使用此应用程序控制外部显示器的用户界面！它使用隐藏的[WindowManagerShellCommand](https://android.googlesource.com/platform/frameworks/base/+/master/services/core/java/com/android/server/wm/WindowManagerShellCommand.java)来调整密度以使 UI 元素看起来更小，过扫描以隐藏导航栏，和/或分辨率以匹配外部显示器的分辨率。摆弄这些值，直到你得到你满意的东西。

就是这样！在 Android 10 智能手机上享受桌面模式。我们不确定谷歌为什么在 Pixel 4 上禁用了 DisplayPort Alt 模式功能，所以我们寻求评论，如果有回音，我们会更新你的信息。如果你是一个对将任务栏集成到你的启动器感兴趣的定制启动器开发者，你可以在这里找到说明。

* * *

*更新 1(美国东部时间 11/1/19 @下午 2:17):这篇文章被更新以简化如何调整外部显示器 UI 的说明。*