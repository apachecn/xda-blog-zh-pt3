# Android 隐私沙盒开发者预览版 5 为开发者提供了更多的控制

> 原文：<https://www.xda-developers.com/android-privacy-sandbox-developer-preview-5/>

# Android 隐私沙盒开发者预览版 5 为开发者提供了更多的控制

Android 的 Privacy Sandbox Developer Preview 5 已经发布，它为开发者在应用中使用 API 提供了更多的控制。

自今年二月发布以来，Android 的隐私沙盒一直在开发中。这是一项为期多年的计划，旨在向最终用户介绍更多的私人广告解决方案，这要归功于主题 API 和 FLEDGE。其目的是在默认情况下保护用户隐私，同时仍然支持依赖有效广告来维持免费和广告资助应用程序的移动生态系统。这是一种独特的 Android 方法，新的 SDK 与应用程序的其余代码相隔离，其目标是最终取代 Ad ID。最新的开发人员预览版现已发布，它增加了数据验证增强功能，并在隐私保护 API 和 SDK 运行时之间进行了 API 签名更改。

隐私沙盒开发者预览版 5 真的只是开发者测试隐私沙盒并向谷歌提供更多反馈的更新。谷歌表示，过去几个月的反馈已经带来了真正的变化，包括允许使用反射 API。由于开发者的反馈，额外的设计提案也已经在[羽翼未丰服务](https://github.com/privacysandbox/fledge-docs/blob/main/trusted_services_overview.md)、[中介](https://developer.android.com/design-for-safety/privacy-sandbox/fledge-mediation)和[应用到网络测量](https://developer.android.com/design-for-safety/privacy-sandbox/attribution-app-to-web)上发表。有一些变化需要开发者对他们的代码进行修改，这些在发行说明中有概述。

如果你想以开发者的身份开始测试隐私沙盒，[你可以查看官方说明](https://developer.android.com/design-for-safety/privacy-sandbox/setup)在 Android 虚拟设备仿真器或支持的 Pixel 设备上设置 SDK 和[下载系统映像](https://developer.android.com/design-for-safety/privacy-sandbox/download)。仍有一个测试版计划在今年年底推出，2023 年将开始大规模测试。这些预览版和测试版独立于 Android 13 的发布节奏，并在过去几个月中分别进行了测试。最终版本还将在设置应用中提供面向用户的控件。

Privacy Sandbox 中的新功能包括属性报告 API 中的跨应用程序和 web 测量，以及主题 API 中的移动应用程序分类的更新分类法。Android API 中还有一些开发者需要考虑的附加限制。

如果你是一个开发者，一定要查看官方发行说明和开发者预览版 5 公告博客文章。两者都包含支持 Privacy Sandbox SDK 的重要信息，以及您可能需要进行的更改，以包含对 Privacy Sandbox 的支持。

* * *

**来源:[谷歌](https://android-developers.googleblog.com/2022/09/privacy-sandbox-developer-preview-5-is-here.html)**