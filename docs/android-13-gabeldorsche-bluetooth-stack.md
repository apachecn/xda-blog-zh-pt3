# Android 的 Gabeldorsche 蓝牙栈现在正在 Android 13 中使用

> 原文：<https://www.xda-developers.com/android-13-gabeldorsche-bluetooth-stack/>

长久以来，Android 的所有蓝牙功能都依赖于“氟化物”堆栈。但谷歌在 Android 11 上开始测试一个名为“Gabeldorsche”的新蓝牙堆栈。在它向 Pixel 设备推出第一个 Android 11 稳定版本后不久，我们[在版本](https://www.xda-developers.com/hidden-changes-android-11-source-code/#:~:text=what%20is%20gabeldorsche%3F)中发现了一个新的开发者选项，名为 *Enable Gabeldorsche* ，它帮助开发者测试新的蓝牙堆栈。该选项出现在所有 Android 12 和 Android 12L 版本中，也包含在 Android 13 的早期开发者预览版中。然而，谷歌在第二次 [Android 13](https://www.xda-developers.com/android-13/) 测试版中移除了它。那是因为谷歌在 Android 13 中默认启用了 Gabeldorsche 蓝牙栈。

对于不知道，蓝牙栈是负责处理蓝牙连接的软件。如前所述，Android 多年来一直使用氟化物蓝牙堆栈来实现所有蓝牙功能。但现在，经过多年的测试，谷歌已经用新的 Gabeldorsche 蓝牙堆栈取代了它的某些功能。Gabeldorsche 蓝牙栈是对 Android 蓝牙栈的完全重写，在 Android 13 中默认启用，但仅*“到扫描层。”*

根据*斯珀的*米沙·拉赫曼的说法，Android 13 将利用 Gabeldorsche 蓝牙栈进行*“BLE 扫描、BLE 广告、ACL 连接管理、控制器信息管理、HCI 层、HAL 接口层和其他所需的组件，如配置存储。”*

虽然谷歌尚未正式宣布 Android 13 的这一变化，但该公司[强调这是 Android Automotive 13](https://www.xda-developers.com/android-automotive-13-rollout/) 中连接更新的一部分。经过进一步调查，拉赫曼发现 Gabeldorsche 堆栈似乎也适用于 Android 13。

谷歌旨在通过 Gabeldorsche 提高蓝牙的安全性、可靠性、互操作性和自动化端到端测试。目前还不清楚这会给最终用户带来多少好处，但它可能会导致更低的延迟和一些稳定性的改善。

* * *

**Via:**斯珀