# Android 13 来到树莓 Pi 4，由第三方 ROM 提供

> 原文：<https://www.xda-developers.com/raspberry-pi-4-b-pi-400-compute-model-4-android-13-port/>

就在几天前，谷歌向其 Pixel 手机推出了稳定的 [Android 13](https://www.xda-developers.com/android-13/) 更新，并将发布的源代码上传到 AOSP，但 XDA 的一名开发人员已经为 Raspberry Pi 4 单板计算机及其衍生产品制作了首张 [Android 13 定制 ROM](https://www.xda-developers.com/android-13-custom-rom-list/) 。

XDA 资深成员 KonstaT 为这款流行的信用卡大小的电脑制作了一个纯基于 Android 13 的 AOSP ROM。这里的一个主要好处是，这种构建也与 Raspberry Pi 400 兼容，这是一种便携式 ARM PC，全部包含在迷你键盘形状因素中。甚至可以在 Raspberry Pi 计算模块 4 上启动该版本，但您可能需要一个额外的载板。

虽然它是为高级用户设计的，但 Android 13 版本似乎可以很好地支持大多数功能，包括:

*   音频(HDMI、3.5 毫米插孔、USB 麦克风、蓝牙扬声器/耳机等。)
*   音频 DAC(使用 GPIO DACs，例如 HiFiBerry DAC+)
*   蓝牙(和蓝牙共享)
*   摄像头(使用官方 Pi 摄像头模块和 UVC USB 网络摄像头)
*   GPIO
*   GPS(使用外部 USB 模块，如 U-blox 7)
*   以太网
*   硬件加速图形(V3D、OpenGL 和 Vulkan)
*   HDMI 显示器(和 HDMI-CEC)
*   I2C
*   红外遥控器(使用外部 GPIO 红外模块，如 TSOP4838)
*   RTC(使用外部 GPIO I2C 模块，如 DS3231)
*   传感器(使用外部 GPIO I2C 模块，例如 MPU6050、LSM6DS3、LSM303DLHC、BME280/BMP280 和 APDS9930 加速度计、陀螺仪、磁力计、温度、压力、湿度、环境光和接近度)
*   串行控制台(使用外部 GPIO 串行控制台适配器，例如 PL2303)
*   精力
*   触摸屏/多点触控(官方 7 英寸触摸屏、USB 触摸屏、Waveshare SPI 触摸屏)
*   USB(鼠标、键盘、存储等。)
*   USB-C(亚洲开发银行、MTP、PTP、USB 网络共享)
*   无线网络(和无线网络共享)

安装也很容易。此端口可作为磁盘映像使用，因此您可以在恢复后从 microSD 卡启动它。你也可以通过特制版本的 TWRP 安装后续更新，尽管这个过程需要几个额外的步骤。

请记住，这与在大屏幕上运行类似 Android TV 的东西截然不同——后者是为媒体消费而定制的，而不是积极和定期的互动。正如你所料，树莓 Pi 4 平台的 Android 端口在传统意义上并不完美。缺乏硬件支持的视频编码和解码意味着您必须依赖基于软件的编解码器，性能会明显下降。此外，许多官方的 Raspberry Pi 相机配件都没有正常工作。SElinux 也处于许可模式。

虽然这对于大多数人来说并不十分有用，但如果你有树莓 Pi 4 并且喜欢摆弄 Android 13，这可能是一个有趣的实验。请务必跟随论坛上的 ROM 线程开始。

**[下载 AOSP 13.0 为树莓 Pi 4 型号 B，Pi 400，计算模块 4](https://forum.xda-developers.com/t/4481977/)**