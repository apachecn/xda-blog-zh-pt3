# Android 14 内置了对谷歌和三星健康连接平台的支持

> 原文：<https://www.xda-developers.com/android-14-health-connect-built-in/>

如果你真的想减肥、健身或注意饮食，那么你的智能手机可以成为你健康和健身武库中一个无价的工具。然而，许多人发现一个应用程序不足以跟踪他们需要的一切。然而，使用多个健康和健身应用程序可能是一件痛苦的事情，因为它们之间的互联性可能不存在或非常有限。为了解决这个问题，谷歌和三星合作开发了一个名为 [Health Connect](https://www.xda-developers.com/health-connect/) 的平台，它可以成为所有运行 [Android 14](https://www.xda-developers.com/android-14/) 的设备的开箱即用体验的一部分。

谷歌在去年的 I/O 2022 上宣布了健康连接[。这是一个让应用程序更容易分享健康和健身数据的平台。它标准化了应用程序记录健康和健身数据的方式，因此开发人员无需为他们想要同步数据的每个服务编写不同的集成代码。Health Connect 平台由两部分组成:开发人员调用的 API 和允许用户管理其数据并控制哪些服务可以访问该数据的应用程序。](https://www.xda-developers.com/google-samsung-health-connect-api/)

Health Connect 应用程序是该平台的重要组成部分。毕竟，它实际上负责安全地存储和管理用户的健康和健身数据，其他应用程序通过 API 利用这些数据。如果没有该应用程序，其他应用程序就无法同步数据。幸运的是，健康连接应用程序只需轻点几下，就可以安装在任何运行 Android 9 或更高版本、带有 Google Play 服务的设备上。

幸运的是，安装 Health Connect 需要点击几下，这立即限制了它的覆盖范围，因为用户必须知道它的存在，才能去下载它。Health Connect 的用户基础有限(该应用程序已在 100 万至 500 万台设备上下载),这意味着一些开发人员可能看不到支持该平台的价值，尽管幸运的是，谷歌与许多公司密切合作，在推出之前增加了支持。尽管如此，如果有更多的用户了解它，对该平台的长期健康会更好。

一种解决方案是将 Health Connect 植入操作系统，这样它就可以在所有 Android 设备上使用，这正是谷歌在 Android 14 中可能会做的事情。Android 14 DP1 附带了一个新的 APEX 文件，包名为 com。如果你还记得的话，【谷歌】. android.healthconnect. APEX 是[一种 android 特有的文件格式](https://blog.esper.io/what-is-project-mainline/#the-structure-of-apex-packages)，用于[项目主线](https://www.xda-developers.com/android-project-mainline-modules-explanation/)。项目主线将系统组件模块化为 APK 或 APEX 格式，以便它们可以通过 Google Play 进行更新，这是一种更新交付机制，您可能听说过称为“Google Play 系统更新”

Health Connect APEX 中有一个版本的 Health Connect 应用程序，它具有不同的包名(com。而不是通过 Google Play(com . Google . Android . apps . health data)获得。不同的包名称在这里是有意义的，因为 Android 不允许你安装与已经安装的应用程序具有相同包名称的应用程序，并且许多升级到 Android 14 的用户将已经从 Google Play 安装了 Health Connect。

对于那些已经安装了 Google Play 版本的应用程序并填充了数据的用户，Android 14 可能会让他们将数据迁移到系统版本。拥有新的 MIGRATE_HEALTH_CONNECT_DATA 权限的应用程序将能够将数据从 Google Play 版本的 Health Connect 迁移到系统版本。MIGRATE_HEALTH_CONNECT_DATA 的保护级别为“knownSigner|signature”，因此它只能授予使用平台证书签名的应用程序或使用数组“config _ healthconmigrationknownsigners”中定义的[已知签名证书](https://developer.android.com/guide/topics/permissions/defining#grant-signature-permissions)签名的应用程序

健康连接的系统版本具有不同的包名称的一个缺点是应用程序需要更新才能知道它。目前，使用 Health Connect API [的应用程序会检查](https://developer.android.com/guide/health-and-fitness/health-connect/get-started#step_2_get_health_connect_client)是否安装了 Play Store 版本的应用程序，但如果没有安装该版本的应用程序，就不再适合假设该 API 不可用。然而，谷歌可能会更新[健康连接支持库](https://developer.android.com/jetpack/androidx/releases/health-connect)，这样开发者就不必担心弄清楚安装的是哪个版本的应用程序。健康连接意图动作，例如，[正在被更新](https://android-review.googlesource.com/c/platform/frameworks/support/+/2417359)以打开安装在设备上的健康连接的正确版本的设置。

鉴于我们目前所知的情况，有理由认为健康连接将成为 Android 14 中一个新的项目主线模块。如果是这样，这意味着谷歌将能够通过 Play 系统更新直接向其推送更新，前提是 OEM 厂商必须分发谷歌的签名版本。即使它们不是，但它现在在 APEX 文件中的事实应该意味着，除非它在 Android 14 发布前被废弃，否则它的源代码将在 AOSP 发布时公开。事实上，一个名为“ [HealthFitness](https://android.googlesource.com/platform/packages/modules/HealthFitness/) ”的新存储库已经在 AOSP 的 Android/platform/packages/modules 位置下出现，这表明这确实会发生。