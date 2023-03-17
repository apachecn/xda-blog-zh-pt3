# Android 14 可能会集成 Google Play 的数据安全部分，向你展示为什么应用程序需要位置访问

> 原文：<https://www.xda-developers.com/android-14-data-safety-section/>

你总是能够在通过 Google Play 安装应用程序之前查看它请求了什么权限(嗯，除了[一小段时间](https://www.xda-developers.com/google-play-store-hides-permissions/))，但是总是由开发者来告诉你为什么他们的应用程序需要那些权限。即使推出了 [Google Play 的数据安全部分](https://www.xda-developers.com/google-play-store-safety-section-rolling-out/)，这一点也没有改变，因为其中的信息是基于开发者披露的内容。虽然更大的透明度总是好的，但这些信息只显示在应用程序的 Play Store 列表上这一事实意味着许多用户可能会错过它。此外，用户没有简单的方法来判断应用程序的数据安全信息何时发生了变化。幸运的是，谷歌准备在 [Android 14](https://www.xda-developers.com/android-14/) 中解决这些问题。

用谷歌自己的话说，Google Play 的数据安全部分“向用户提供了一个应用程序如何收集、分享和保护用户数据的简化视图。”谷歌在 2021 年 I/O 上宣布了数据安全部分，并在几个月后开放了 Play 控制台供开发者提交信息。数据安全部分于 2022 年 4 月推出，但开发者必须在 2022 年 8 月前填写表格。2022 年 8 月之后提交到 Google Play 的所有新应用和应用更新都必须有一个完整的数据安全表，这意味着开发者需要真正考虑他们应用的每个功能和他们收集的数据。

数据安全表格要求开发者披露他们的应用程序是否收集或共享广泛的[数据类型](https://support.google.com/googleplay/android-developer/answer/10787469?hl=en#in_play_console&zippy=%2Cpurposes%2Cdata-types)以及他们使用这些数据的[目的](https://support.google.com/googleplay/android-developer/answer/10787469?hl=en#in_play_console&zippy=)的声明。例如，一个收集位置数据的应用程序可能会将它用于核心功能，如跟踪用户的户外锻炼，而另一个应用程序可能会收集这些数据以显示更个性化的内容。现在，你必须查看应用程序的 Play Store 列表才能找到这些信息，但在 Android 14 中，这些信息可能会由操作系统本身显示。

在 Android 14 DP1 中，我在各种应用的“位置许可”页面中启用了新的“数据隐私”部分，如下面嵌入的截图所示。当一个应用程序报告它收集位置数据作为 Google Play 数据安全表单的一部分时，就会出现这一部分。该文本声明“您的位置可能会被共享”，因为“该应用程序声明它可能会与第三方共享您的位置。”点击文本会打开一个对话框，列出应用程序收集位置数据的原因(从 Google Play 的应用程序数据安全部分获取)。

此对话框也可从权限提示中访问，以授予应用程序位置访问权限，如下所示。在“精确”和“近似”选择器的上方，有一段新的文字说，“这个应用程序声明它可能会与第三方共享位置数据。”点击文本启动与之前相同的对话框。

Android 14 DP1 目前只显示“位置”类别的数据安全信息，但我不明白为什么其他类别的信息不能显示。事实上，这个特性的代码表明所有的数据安全类别——不仅仅是“位置”——都是受支持的。然而，我不知道谷歌是否打算将这一功能限制为仅显示应用程序的“位置”数据安全信息，或者他们是否计划扩展这一功能。当被问及对这项功能的评论时，谷歌的一位发言人让我看了该公司的 Android 14 DP1 博客帖子。

关于这项功能的另一个趣闻是，它可能无法在 Android Automotive、Wear OS 或 Android TV/Google TV 上使用。有代码明确检查设备是否运行 Android 的其他版本，如果是，记录“数据共享更新”功能不可用。

说到“数据共享更新”，这是一个新的设置页面，可以在设置>安全与隐私>隐私下找到，它让你“查看改变了他们共享位置数据方式的应用程序。”在这里，您可以查看应用程序更新后应用程序的数据共享信息何时被修改，如下所示。

在上面的截图中，你可以看到应用程序“DataSafetyLabelTest”已被注明为“现在[分享]位置用于广告”，这表明该应用程序已经更新了其使用位置数据的原因列表，以包括广告。“DataSafetyLabelTest”当然不是 Google Play 上真正的 app 这是我创建的一个应用程序，用于触发系统写入测试数据安全信息。

当 real app 的数据安全信息发生更改时，您可能会收到通知，要求您查看“数据共享更新”页面上的更改。不过，我没有分享这个通知的截图。

系统以 XML 的形式跟踪应用程序的数据安全信息，但我不确定系统是如何确定应用程序的数据安全信息何时发生变化的。系统从 Google Play 中提取这些数据是有意义的，但我也看到了系统将使用新的 API 读取应用元数据的暗示。这个[元数据可以由安装程序设置](https://developer.android.com/reference/android/content/pm/PackageInstaller.Session#setAppMetadata(android.os.PersistableBundle))，在大多数情况下是 Google Play。由于 Google Play 已经保存了开发人员通过数据安全表单提交的所有信息，我想它可以在安装应用程序时轻松地将这些信息保存为应用程序元数据的一部分。

无论如何，谷歌似乎正在努力将数据安全标签直接集成到 Android 14 中。开发者应该准备好他们提交给 Google Play 的信息会在设置应用和权限对话框中出现在用户面前。用户应该留意应用程序报告他们收集了哪些数据，收集的原因是什么。

如果这一变化出现在 Android 14 的稳定版本中，我会很欢迎，因为这将迫使应用程序解释为什么他们使用某些权限来收集数据，以及他们收集这些数据的目的是什么。开发者已经被鼓励[解释他们](https://developer.android.com/training/permissions/explaining-access)[请求某些敏感权限](https://developer.android.com/training/permissions/requesting#explain)的理由，但是许多应用不这么做。另一方面，Google Play 已经迫使开发者解释他们为什么使用特定权限来收集特定类型的数据，因此找到一种直接在 Android 中显示这些信息的方法是一个伟大的举措。