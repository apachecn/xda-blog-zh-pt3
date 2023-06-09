# 谷歌将为 Pixel 平板电脑的手写笔使用快速配对低电量警报

> 原文：<https://www.xda-developers.com/fast-pair-battery-alerts-pixel-tablet-stylus/>

当谷歌在 2020 年 4 月推出第二代 Pixel Buds 时，[宣布了针对特定蓝牙配件的新快速配对功能](https://www.xda-developers.com/fast-pair-location-tracking-battery-notifications-new-settings/)。其中有一个方便的功能，在连接时弹出附件的电池电量通知，甚至在电池电量不足时共享警报。该功能目前适用于支持快速配对的 TWS 耳塞和智能手表，但谷歌正在努力增加对 Pixel 平板电脑有源手写笔的支持。

根据在 APK 拆除 Wear OS v23.02.13 的 Google Play 服务中发现的新字符串(通过 *9to5Google* )，快速配对电池警报将很快用于活动触控笔。字符串显示，该功能将为触控笔提供三种低电量警报:“电池电量低”、“低电量”和“非常低的电池电量”。“这些通知还会分别提示用户‘考虑马上充电’、‘马上充电’和‘现在充电’。

```
<string name=”fast_pair_stylus_battery_getting_low_description”>Battery getting low \u2022 Consider charging soon</string>

<string name="”fast_pair_stylus_low_battery_description”">电量低\u2022 充电快</string>

<string name="”fast_pair_stylus_very_low_battery_description”">电量极低，现在充电</string>

除了这些字符串，谷歌还在设置服务应用程序中添加了一个通用的“bt_stylus”图标，为 Pixel 的电池小部件供电。这意味着 Pixel Battery 小部件还将显示活动触控笔的当前电池电量。

*图片通过 9to 5 谷歌*

虽然字符串中没有明确说明，但这些添加很可能是为谷歌可能与即将推出的 Pixel 平板电脑一起推出的第一方主动触控笔做准备。早期的泄露表明，Pixel 平板电脑将支持 USI 手写笔，该公司提供无缝集成的第一方选项是有意义的。

然而，目前还不清楚即将推出的手写笔将如何充电。我们当然希望谷歌不会采取苹果对第一代 Apple Pencil 采取的相同方法，并提供类似于 [Apple Pencil 2](https://www.xda-developers.com/apple-pencil-2-isnt-magic-wand-editorial/#apple-pencil-2-the-yays) 的磁性无线充电支持。但我们必须等到该公司推出 Pixel 平板电脑后才能确定。

**来源:** [9to5Google](https://9to5google.com/2023/01/14/google-fast-pair-battery-stylus/) 

```