# 如何在旧像素上启用谷歌 Pixel 6 的游戏仪表盘

> 原文：<https://www.xda-developers.com/how-to-enable-pixel-6-game-dashboard-older-pixels/>

随着谷歌 Pixel 智能手机的每一次发布，我们都会看到新设备独有的一些有趣的新功能。最终，这些功能中的一些通过官方更新或售后模块进入了旧款智能手机。同样，在 [Pixel 6](https://www.xda-developers.com/google-pixel-6/) 系列中，谷歌结合 [Android 12](https://www.xda-developers.com/android-12/) 的游戏模式 API 推出了一个专用的[游戏仪表盘](https://www.xda-developers.com/android-12-game-dashboard-gaming-mode-apis/)工具，可以快速访问一些有用的工具，以及用于向 YouTube Live 流媒体的小部件，[显示 Google Play 游戏的成就](https://www.xda-developers.com/google-play-games-integration-android-12-game-dashboard/)，并改变性能配置文件。据谷歌称，游戏仪表盘将在适当的时候在运行 Android 12 的“选定设备”上提供，但迄今为止，没有一款老一代 Pixel 手机获得该功能。

**[谷歌 Pixel 6 XDA 论坛](https://forum.xda-developers.com/f/google-pixel-6.12311/) ||| [谷歌 Pixel 6 Pro XDA 论坛](https://forum.xda-developers.com/f/google-pixel-6-pro.12313/)**

幸运的是，移植整个游戏仪表盘模块出奇的容易——至少对于搭载 Android 12 的谷歌 Pixel 设备来说是这样。事实是，所有与仪表板相关的代码都已经存在于谷歌的 SystemUI 版本中(但不是 AOSP 的 SystemUI 版本)，但是该功能的可用性是由一个参数控制的。正如**mishal Rahman**所指出的，人们可以很容易地从谷歌 Pixel 6/6 Pro 的固件包中提取相关的配置数据。如果你拥有一台[谷歌 Pixel 5a](https://forum.xda-developers.com/f/google-pixel-5a.12359/) 、 [Pixel 5](https://forum.xda-developers.com/c/google-pixel-5.11335/) 、 [Pixel 4a 5G](https://forum.xda-developers.com/c/google-pixel-4a-5g.11321/) 、 [Pixel 4a](https://forum.xda-developers.com/c/google-pixel-4a.10249/) 、 [Pixel 4](https://forum.xda-developers.com/c/google-pixel-4.9014/) 、 [Pixel 4 XL](https://forum.xda-developers.com/c/google-pixel-4-xl.9021/) 、 [Pixel 3a](https://forum.xda-developers.com/c/google-pixel-3a.8868/) 、 [Pixel 3a XL](https://forum.xda-developers.com/c/google-pixel-3a-xl.8875/) 、 [Pixel 3](https://forum.xda-developers.com/c/google-pixel-3.8236/) 或 [Pixel 3 XL](https://forum.xda-developers.com/c/google-pixel-3-xl.8243/)

为了方便读者，下面是配置数据的文本视图:

```
 <?xml version="1.0" encoding="utf-8"?>

<config>

        <!-- This feature is meant to be the feature identifying devices that support

             Game Dashboard 

        <feature name="com.google.android.feature.GAME_OVERLAY" />

</config> 
```

你需要将上面的代码片段保存为“game_overlay.xml”并放在你的 Pixel 设备的`/product/etc/sysconfig`处。我们还镜像了该文件的现成版本，可在下面找到:

**[下载 game_overlay.xml 摘自 Google Pixel 6](https://mega.nz/file/MpwXCahT#41wQlIqxjNpYvAyPqfstvLKx1CjYqw75eGIb77uvgyc)**

请记住，将 XML 文件复制到上述位置需要 [root 访问权限](https://www.xda-developers.com/root/)。如果您对 [Magisk 模块](https://www.xda-developers.com/best-magisk-modules/)并不陌生，您也可以创建一个简单的模块来完成这项工作。我们希望旧的谷歌 Pixel 设备将在他们即将到来的 Pixel 功能下降中获得游戏仪表盘，但在此之前，这是值得手机游戏玩家尝试的事情。

 <picture>![The Pixel 6 comes with Google's new Tensor chip, a modern design, and flagship cameras.](img/7343f77af84019bd24844d3d2e495f29.png)</picture> 

Google Pixel 6

Pixel 6 配备了谷歌新的张量芯片、现代设计和旗舰相机。

 <picture>![The Pixel 6 Pro is the larger sibling that comes with Google's new Tensor chip, a modern design, and an extra telephoto camera.](img/5c825565a61d24d571df294787f045fc.png)</picture> 

Google Pixel 6 Pro

Pixel 6 Pro 是较大的兄弟，配有谷歌的新张量芯片、现代设计和额外的远摄相机。