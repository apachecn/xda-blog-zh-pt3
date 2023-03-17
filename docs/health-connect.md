# 什么是健康连接:谷歌如何结合三星、Fitbit 和其他公司的健身数据

> 原文：<https://www.xda-developers.com/health-connect/>

如果你曾经在智能手机上使用过多个健康和健身跟踪应用程序，那么你就会知道在看似没有互联性的多个应用程序之间进行跟踪的痛苦。像 MyFitnessPal 这样的应用程序有时可以与其他健康应用程序接口来收集数据，但这取决于个人开发者是否支持其他个人平台。比如 MyFitnessPal 没有 Mi Fit 集成，但是支持 Google Fit，所以你把 Mi Fit 连接到 Google Fit，然后 Google Fit 再连接到 MyFitnessPal。对于任何使用多个应用程序的人来说，这都是一场噩梦，但谷歌有一个解决方案:健康连接。

Android 上有无数的健康追踪应用程序，但并不是每一个应用程序都会涵盖你可能想要追踪的每一个重要信息。应用程序可以也确实选择与其他应用程序单独共享数据，但在以前，没有一个健康应用程序可以利用的 API 来共享数据。Health Connect 是谷歌对这一问题的回答，因为它充当了这些跟踪应用程序相互共享数据的中介。如果 MyFitnessPal 想要从 Samsung Health、Fitbit 和 Google Fit 获取数据，它以前需要直接与这些应用程序进行交互。在这种情况下，它只需要连接到 Health Connect，Health Connect 将为它处理所有这些连接。

健康连接是在谷歌 I/O 上宣布的，最近已经向谷歌 Play 商店的用户推出。它由一个开发人员可以集成到他们的应用程序中的 SDK 和一个控制权限和数据管理的面向用户的应用程序组成。

## 哪些应用支持 Health Connect？

健康连接仍处于测试阶段，但[支持 API](https://play.google.com/store/apps/collection/promotion_all__health_connect) 的应用程序正在慢慢增加。下面的列表是在撰写本文时支持 Health Connect 的所有应用程序的列表。

*   健康生活
*   Fitbit
*   三星健康
*   Google Fit
*   MyFitnessPal
*   乌拉
*   菲欧
*   生命总和
*   户外活动
*   证明洞察力

支持 Health Connect API 的应用程序[也必须遵守严格的数据规则](https://support.google.com/googleplay/android-developer/answer/9888170?hl=en#:~:text=Health%20Connect%20by%20Android%20Permissions)来处理和处理个人用户数据。

## Health Connect 是如何工作的？

Health Connect 通过创建健康应用程序需要连接的单一 SDK 来工作，而不是与单独支持的应用程序共享数据。任何支持 Health Connect 的应用程序都可以理解从它选择收集的任何其他应用程序收集的数据，只要这些应用程序已被授予通过 Health Connect API 共享和读取数据的权限。

由于 Google 在 Google I/O 上有自己的文档，理解 API 的工作原理相当简单。

根据上面的图表(取自谷歌在谷歌 I/O 上对健康连接的介绍)，收集数据的应用程序可以与健康连接接口，并允许它控制用户手机上其他应用程序之间共享的所有权限和数据。这意味着，例如，你可以使用一个专门用于睡眠跟踪的应用程序和另一个专门用于锻炼训练的应用程序，然后在另一个、第三个应用程序中以整体方式组合这些数据，让你对所有生命体征有一个概览。它不是现在还存在的东西，但它是以前不能存在的现在可以存在的东西。

例如， [MyFitnessPal 表示](https://support.myfitnesspal.com/hc/en-us/articles/10553948248973-Google-Health-Connect-FAQ-and-Troubleshooting)它目前正在同步以下信息，以便其他应用程序也能够读取和处理:

*   卡路里消耗
*   步伐
*   有氧运动
*   耗水量

例如，在有氧运动的情况下，如果您将有氧运动输入应用程序，MyFitnessPal 将与 Health Connect 分享您的有氧运动。如果您在另一个应用程序中输入您的有氧运动，则该数据将从 Health Connect 共享到 MyFitnessPal。关于 Health Connect，所有数据都存储在本地，并且由利用 SDK 的应用程序决定它们随后如何处理数据。

## 我何时可以使用 Health Connect？

用户已经可以使用 Health Connect，您可以将它与上述任何受支持的应用程序配合使用。据[斯珀](https://blog.esper.io/health-connect-in-android-14/)*最近的一份报告称，目前它还处于测试阶段，虽然它已经运行得很好，但看起来谷歌的目标是在安卓设备上预装健康连接，并且可能尽快在[安卓 14](https://www.xda-developers.com/android-14/) 上安装。谷歌已经表示，它将预装在一些 Android 设备上，随着谷歌像素上的 Android 13 QPR2，谷歌包括了一个健康连接存根包。*

 *正如*斯珀*所解释的，在 AOSP Gerrit 上发现的一个[提交表明，Health Connect 可能会变成一个](https://android-review.googlesource.com/c/platform/system/sepolicy/+/2218681)[项目主线](https://www.xda-developers.com/android-project-mainline-modules-explanation/)模块。一名谷歌员工在 system_server 中将“com.android.healthconnect”显示为 APEX 模块(Mainline 使用的格式),这一事实证明了这一点。谷歌将如何在未来的 Android 版本中整合健康连接还没有确定，但看起来我们可能会以某种方式在 Android 14 中看到它。*