# 如何在 Android Studio 中找到 Android 版本分布统计

> 原文：<https://www.xda-developers.com/android-version-distribution-statistics-android-studio/>

# Android 版本分布统计现在只在 Android Studio 中可用

谷歌不再在网络上显示安卓版本分布统计。相反，你会在 Android Studio 中找到它们。

有很长一段时间，谷歌会在一个专门的网页上发布 Android 版本分布统计数据。然而，该图表自 2019 年 5 月起就没有更新过[，即使如此，5 月的更新也发生在*距离上次更新*6 个月之后。现在很明显，谷歌不再计划更新该图表，但今天我们了解到谷歌有另一个地方显示版本分布统计数据:Android Studio(via](https://www.xda-developers.com/google-hasnt-published-updated-android-distribution-statistics-last-6-months/)[*9 to 5 Google*](https://9to5google.com/2020/04/10/google-kills-android-distribution-numbers-web/))。

开发者可以在 Android Studio 中新建一个项目，然后在 minimum SDK 下拉菜单下选择“帮我选择”，就可以找到最新的 Android 平台/API 版本分布统计。

该图表将帮助开发人员为他们的应用确定正确的最低 SDK 版本。例如，如果您选择“Android 6.0 棉花糖”作为最低 SDK 版本，那么 Android Studio 会通知您，您的应用程序将在所有设备的 84.9%上运行。同样，如果你选择“Android 8.0 Oreo”作为最低 SDK 版本，那么 Android Studio 会通知你，你的应用可以在所有设备的 60.8%上运行。

基于这些数据，我们可以构建一个表格，显示 Android OS 版本的分布情况。

| 

Android 平台版本(API 级别)

 | 

分配(截至 2020 年 4 月 10 日)

 |
| --- | --- |
| 安卓 4.0“冰淇淋三明治”(15) | 0.2% |
| 安卓 4.1“果冻豆”(16) | 0.6% |
| 安卓 4.2“果冻豆”(17) | 0.8% |
| 安卓 4.3“果冻豆”(18) | 0.3% |
| 安卓 4.4“奇巧”(19) | 4% |
| 安卓 5.0“棒棒糖”(21) | 1.8% |
| 安卓 5.1“棒棒糖”(22) | 7.4% |
| 安卓 6.0“棉花糖”(23) | 11.2% |
| 安卓 7.0“牛轧糖”(24) | 7.5% |
| 安卓 7.1“牛轧糖”(25) | 5.4% |
| 安卓 8.0“奥利奥”(26) | 7.3% |
| 安卓 8.1“奥利奥”(27) | 14% |
| Android 9“馅饼”(28) | 31.3% |
| 安卓 10 (29) | 8.2% |

Android 版本分布显示在 Android Studio 中是有意义的，因为这些数据实际上只对开发者有用。