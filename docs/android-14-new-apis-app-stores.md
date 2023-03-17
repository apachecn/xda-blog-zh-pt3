# Android 14 增加了新功能，使第三方应用商店更加出色

> 原文：<https://www.xda-developers.com/android-14-new-apis-app-stores/>

Google Play 是 Android 用户中最受欢迎的应用商店，但有些人可能会认为它没有公平地赢得冠军。谷歌一直受到世界各地监管机构和立法机构的审查，因为它如何保持其应用商店的主导地位，而且没有迹象表明这种压力会很快放松。这也许是谷歌主动在 Android 14 中引入新功能的原因，这些新功能可以改善第三方应用商店的用户体验。

Android 上的大多数第三方应用商店都没有真正与 Google Play 竞争，这不仅仅是因为他们的应用选择。虽然第一方的预装应用程序商店一直都有自动更新应用程序的能力，但第三方应用程序商店直到最近才能够进行无人值守更新。谷歌在 Android 12 中为[添加了一个 API，让第三方应用商店无需用户操作即可更新应用，减少了](https://www.xda-developers.com/android-12-alternative-app-stores-update-apps-background/)[使用第三方应用商店](https://blog.esper.io/distribute-apps-without-google-play/)的摩擦。

然而，这仍然让第三方应用商店在功能方面处于主要劣势，因为他们不容易知道*何时*进行自动更新是安全的。这就是谷歌试图在 Android 14 中通过一个新的 API 来解决的问题，该 API 使第三方应用商店能够进行“温和更新”。

## 温和更新

Android 14 增加了一个新的 API，让第三方应用商店在自动更新应用程序之前检查是否满足某些条件。[包安装程序。应用商店可以使用 InstallConstraints API](https://developer.android.com/reference/android/content/pm/PackageInstaller.InstallConstraints) “在不中断用户体验的情况下提供自动更新(称为温和更新)——例如，当应用商店发现要更新的应用程序正在与用户交互时，它可能会推迟更新。”

这个新的 API 允许第三方应用商店检查他们准备更新的应用是否有活动的前台服务(isRequireAppNotForeground)，是否以某种方式与用户交互(isRequireAppNotInteracting)，或者是否在屏幕上(isRequireAppNotTopVisible)。第三方应用商店也可以检查设备是处于打盹模式(isRequireDeviceIdle)还是处于通话状态(isRequireNotInCall)。

虽然 API 允许指定要检查的条件，但文档建议使用预设的约束，因为“系统最知道如何做”这是合乎逻辑的，因为谷歌有足够的时间来开发如何最好地处理自己应用商店的自动更新。使用预置也是有益的，正如文档所指出的，因为如果 Google 给 API 添加更多的约束，温和更新的准确性和效率可能会在未来的版本中得到提高。

PackageInstaller 的每个条件。InstallConstaints API 支持检查，可以通过现有的 API 进行检查，但是让系统处理这些检查要容易得多，而且干扰性更小。例如，第三方应用商店想要检查他们更新的应用程序是否被用户主动使用，目前必须使用 UsageStats 或 AccessibilityService 等 API，这两个都是敏感权限。但是，如果他们使用这个新的 Android 14 API，他们就不需要这些权限来完成他们的工作。

## 更新所有权

启用“温和更新”并不是 Android 14 对第三方应用商店的唯一改进。还有一个新的“更新所有权”机制，让第三方应用商店成为他们首次安装的应用程序未来自动更新的唯一来源。这将意味着，如果你使用第三方应用商店，因为通过它提供的应用程序是由社区审查的，那么通过其他应用商店提供的未经审查的更新不会自动推送到你的设备。

现在，当你通过第三方应用商店安装应用程序时，没有什么可以阻止第一方应用商店更新该应用程序。虽然 Android 12 的无人值守更新 API 只允许第三方应用商店静默更新他们首次安装的应用，但第一方应用商店不受影响，因为他们拥有特权 [INSTALL_PACKAGES](https://developer.android.com/reference/android/Manifest.permission#INSTALL_PACKAGES) 权限。

Android 14 上的第三方应用商店可以使用 [PackageInstaller 中新的](https://developer.android.com/reference/android/content/pm/PackageInstaller.SessionParams)[setRequestUpdateOwnership](https://developer.android.com/reference/android/content/pm/PackageInstaller.SessionParams#setRequestUpdateOwnership(boolean))方法。然而，SessionParams 告诉系统，他们声称对即将安装的应用程序拥有更新所有权。一旦为应用程序启用了更新所有权强制，所有其他应用程序商店(即使是具有 INSTALL_PACKAGES 权限的应用程序商店)都需要用户执行操作来更新应用程序。更新所有权只能在应用的初始安装期间启用，因此另一个应用商店将无法接管更新，除非从该商店卸载并重新安装有问题的应用。通过新的[install source info # getUpdateOwnerPackageName()](https://developer.android.com/reference/android/content/pm/InstallSourceInfo.html#getUpdateOwnerPackageName())API，应用商店可以检查应用程序是否启用了更新所有权，如果是，哪个应用程序是更新所有者。

第三方应用商店必须持有新的 [ENFORCE_UPDATE_OWNERSHIP](https://developer.android.com/reference/android/Manifest.permission#ENFORCE_UPDATE_OWNERSHIP) 权限才能使用更新所有权强制 API，但由于该权限的保护级别为“正常”，因此它将在安装时由系统授予。不过，Google Play 是否会对这个权限/API 的使用进行审计，还有待观察。

## 安装预批准

我想强调的最后一个新的 Android 14 API 是 [PackageInstaller。会话#requestUserPreapproval](https://developer.android.com/reference/android/content/pm/PackageInstaller.Session#requestUserPreapproval(android.content.pm.PackageInstaller.PreapprovalDetails,%20android.content.IntentSender)) 。该 API 允许第三方应用商店在提交安装会话之前请求用户批准。我想这对于有意想在后台更新应用程序之前提示用户的第三方应用程序商店会很有用。

例如，想象一个以安全为中心的应用程序商店想要让它的用户知道什么时候一个应用程序更新添加了新的权限；app store 可以在更新之前提示用户，而不是自动更新该应用，从而在保护级别为“正常”时自动授予该权限。目前，如果用户在自动更新期间不在场，第三方应用商店将不得不跟踪安装会话并在稍后提示他们。这个 API 简化了这个过程。

* * *

Android 14 将在今年晚些时候向公众发布，届时将引入大量新功能和 API。虽然这些新的 API 不像我们发现的其他一些变化那样被隐藏，但不能保证这些 API 将在稳定版本中对开发人员可用。这是因为在 2023 年 6 月 Android 14 达到 Beta 3 的“平台稳定性”之前，API 冻结不会发生，而我们目前只在 DP1 上。我们将密切关注未来的 Android 14 DP 和 Beta 版本，看看这些 API 是否会继续存在，或者是否会添加任何与第三方应用商店相关的新 API。