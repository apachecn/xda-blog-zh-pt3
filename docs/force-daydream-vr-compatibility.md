# 如何在不支持的 Android 设备上强制兼容 Daydream VR

> 原文：<https://www.xda-developers.com/force-daydream-vr-compatibility/>

[谷歌 Daydream VR](https://vr.google.com/daydream/smartphonevr/) 是[谷歌针对移动设备的虚拟现实解决方案](https://forum.xda-developers.com/mobile-vr/google-daydream-vr)。设备需要得到谷歌的官方许可才能被贴上兼容 Daydream 的标签，其中一些要求相当严格。大多数要求只是保证在官方支持的设备上有良好的 VR 性能，但也有一些设备，如 OnePlus 3、OnePlus 3T 或 OnePlus 5，应该可以运行 Daydream VR。

为了支持高性能虚拟现实模式(官方 Daydream VR 支持所必需的)，您的设备必须支持带有 Open GL ES 3.2 的 Vulkan Graphics API，屏幕分辨率至少为 1080p，最低刷新率为 60Hz，理想情况下显示延迟不超过 3 毫秒，持续时间不超过 5 毫米。屏幕尺寸也应该在 4.7 英寸到 6 英寸之间，设备应该支持蓝牙 4.2 LE，并具有温度传感器来读取手机的体温。你可以在这里查看技术要求[的完整列表。](https://source.android.com/compatibility/android-cdd#7_9_virtual_reality)

如果你现有的、不支持 Daydream VR 的设备或多或少符合上述要求，那么你应该能够享受 Daydream VR 体验——只要你**拥有 root 权限**！本教程将向您展示如何通过 Magisk 或修改/system 来无系统地启用 Daydream VR。

* * *

## 强制 Daydream VR 兼容(系统模式)

首先，如前所述，您需要在您的设备上获得 root 访问权限。如果你的设备的引导程序已经解锁，你可以通过自定义恢复比如 TWRP 来刷新 [SuperSU](https://forum.xda-developers.com/apps/supersu) 或者 [Magisk](https://forum.xda-developers.com/apps/magisk) 来得到这个。一旦你有了，安装一个文件浏览应用程序，它将允许你编辑/system 中的文件。我推荐 [MiXplorer](https://forum.xda-developers.com/showthread.php?t=1523691) 或者流行的 Solid Explorer。

### 第一步

打开 MiXplorer，授予它 root 访问权限，导航到/system/etc/permissions，找到名为 handheld_core_hardware.xml 的文件。

注意:我在这里使用的是 Solid Explorer，但是使用 MiXplorer 的步骤是一样的。

### 第二步

打开名为“handheld_core_hardware.xml”的文件，在最后一行前添加以下内容:

```
 <feature name="android.software.vr.mode" />  
```

```
 <feature name="android.hardware.vr.high_performance" /> 
```

保存文件。

### 第三步

接下来，您需要打开位于/system 中的 build.prop 文件。该文件用于识别设备的许多系统属性。我们感兴趣的行是 **ro.product.device** 条目，它定义了您的设备的产品名称。将列出的设备更换为“**旗鱼**”。这是谷歌 Pixel，它被认为是 Daydream VR 兼容手机。该行应读作:

```
 ro.product.device=sailfish 
```

### 第四步

重启手机，安装谷歌 Play 商店的 Daydream 应用程序、谷歌虚拟现实服务和 Daydream 键盘。如果你在 Play Store 中看不到这些，试着从下面的 APKMirror.com 安装它们。

你现在应该可以在你的 Android 设备上使用 Daydream VR 耳机了！如果你还没有，你可以在亚马逊上买一个。

* * *

## 强制 Daydream VR 兼容性(无系统模式)

遵循这些步骤将需要安装 MagiskSU 而不是 SuperSU，因此请确保您已经安装了 Magisk。这个文件有点冗长，因为它是特定于设备的，所以您需要制作自己的 Magisk 模块。**这需要 Linux，因为它使用 shell 脚本。**首先，你需要[下载这个模板](https://github.com/topjohnwu/magisk-module-template)并解压。你还需要使用 Vim 或 Nano。

### 第一步

首先，您需要提取自己的 handheld_core_hardware.xml 文件，只需从/system/etc/permissions 中复制出来即可。把这个拷贝到你的电脑上。导航到 Magisk 模块模板文件夹，并输入名为 system 的文件夹。删除占位符文件，创建一个名为“ **etc** 的文件夹，然后输入并创建一个名为“ **permissions** 的文件夹。在您的权限文件夹中是您想要复制 handheld_core_hardware.xml 文件的位置。文件层次结构应该如下所示。

### 第二步

现在打开您的 handheld_core_hardware.xml 文件，在之前添加这些行

```
 <feature name="android.software.vr.mode" />  
```

```
 <feature name="android.hardware.vr.high_performance" /> 
```

保存并导航回 Magisk 模块模板文件夹的根目录。

### 第三步

剩下的你可以简单地按照 GitHub 页面上的说明来命名你的模块并使它独一无二！一旦完成，运行 config.sh 文件，刷新你新创建的 zip 文件，也刷新[这个 Magisk 模块](https://forum.xda-developers.com/attachment.php?attachmentid=4122637&d=1492899137)，它改变你的 build.prop，由 [XDA 成员 4k4n](https://forum.xda-developers.com/member.php?u=4152720)在[这个线程](https://forum.xda-developers.com/mobile-vr/google-daydream-vr/spoofing-daydream-compatible-device-t3534943)中创建。

就是这样！你可以走了！

* * *

## 说明

只需编辑一个首选项文件，列出您的设备支持的功能即可。我们编辑它以欺骗应用程序认为它支持谷歌 Daydream VR。然而，这对于一些应用程序来说还不够，因为一些 Daydream 应用程序在启动之前会根据官方支持的设备列表先检查设备类型。这就是我们的 build.prop 编辑有望进入的地方，它告诉应用程序我们的设备实际上是一个 Google Pixel。

现在，走出去，在手机上享受虚拟现实的世界吧！以下是一些帮助您入门的应用程序:

查看 Daydream VR XDA 论坛，了解与新兴 VR 平台相关的新闻和讨论！