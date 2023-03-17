# 谷歌发布 Pixel 7 和 Pixel 7 Pro 工厂图片和内核源码

> 原文：<https://www.xda-developers.com/google-pixel-7-7-pro-factory-images-kernel-source-code/>

谷歌 Pixel 7 和 Pixel 7 Pro T1 比之前所有的 Pixel 手机都有所进步。他们很快，[拍出了很棒的照片](https://www.xda-developers.com/google-pixel-7-pro-camera-review/)，并且拥有全新的 Tensor G2 SoC 为他们的内核提供动力，这使他们在 Android 人群中脱颖而出。现在，谷歌已经发布了 Pixel 7 系列的工厂图像和内核源代码，并向公众开放，让那些想要对新购买的产品进行额外控制的人可以使用。

 <picture>![The Pixel 7 packs the second-gen Tensor SoC, a brighter display, and improved cameras.](img/8b31c0e15e95c3f8bf719fbd3ebefc29.png)</picture> 

Google Pixel 7

Pixel 7 包含第二代 Tensor SoC、更亮的 90Hz 显示屏和改进的摄像头。

## 谷歌 Pixel 7 系列的工厂图片

一直在等待 Pixel 7 的股票应用程序和其他系统文件的开发者，工厂图像让你可以访问这些设备上的一切。对于普通用户来说，工厂图像是非常重要的，因为它们使软件的实验在思想上更加容易。

例如，现在对修补者来说，尝试[修复设备](https://www.xda-developers.com/root/)是安全的。modding 社区一直在等待这些，因为没有启动映像备份，就没有办法从一个拙劣的 Magisk 安装中恢复。简而言之，您知道万一出现问题，您可以选择恢复到正常工作的设备。

**下载出厂图片:[谷歌 Pixel 7(代号:“黑豹”)](https://developers.google.com/android/images#panther) ||| [谷歌 Pixel 7 Pro(代号:“猎豹”)](https://developers.google.com/android/images#cheetah)**

目前有三组出厂图像可用: **TD1A.220804.009.A5** 用于日本变型，而 **TD1A.220804.009.A2** 和 **TD1A.220804.031** 用于解锁单元。发布的软件包包含 2022 年 10 月的 Android 安全补丁

 <picture>![The Pixel 7 Pro is Google's top-of-the-line flagship of the year, featuring the second-gen Tensor SoC, a 120Hz LTPO display, a telephoto sensor, and a bigger battery.](img/26bf32dcd1e54473d448d9be3b56170c.png)</picture> 

Google Pixel 7 Pro

##### 谷歌 Pixel 7 Pro

Pixel 7 Pro 是谷歌今年的顶级旗舰产品，具有第二代张量 SoC，120Hz LTPO 显示屏，附加的长焦传感器和更大的电池。

## 内核源代码和设备树

谷歌也已经开始上传内核源代码和设备树源代码，因此开发人员很快就可以开始为设备二人组构建定制内核和移植流行的定制 rom。对于其他 Android 爱好者来说，Pixel 7 的内核源代码是研究谷歌如何让新 Pixel 如此高性能的一个好方法。

| 

设备

 | 

内核源代码

 | 

设备树

 | 

SE 政策

 |
| --- | --- | --- | --- |
| 谷歌 Pixel 7/7 Pro 统一版(代号:“pantah”) | [链接](https://android.googlesource.com/device/google/pantah-kernel/) | [链接](https://android.googlesource.com/device/google/pantah/) | [链接](https://android.googlesource.com/device/google/pantah-sepolicy/) |
| 常见 SoC 元件(代号:“gs201”) | 不适用的 | [链接](https://android.googlesource.com/device/google/gs201/) | [链接](https://android.googlesource.com/device/google/gs201-sepolicy/) |

在编写本报告时，上面链接的存储库似乎是空的，但是它们很快就会被填充。

**[谷歌 Pixel 7 XDA 论坛](https://forum.xda-developers.com/f/google-pixel-7.12607/) ||| [谷歌 Pixel 7 Pro XDA 论坛](https://forum.xda-developers.com/f/google-pixel-7-pro.12609/)**