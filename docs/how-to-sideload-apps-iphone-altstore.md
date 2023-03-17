# 如何使用 AltStore 在任何 iPhone 上轻松下载应用程序

> 原文：<https://www.xda-developers.com/how-to-sideload-apps-iphone-altstore/>

苹果的[iphone](https://www.xda-developers.com/best-iphone/)以封闭而闻名，越狱是大多数人能够想象的侧装应用程序的唯一方式。然而，*还有其他方式将应用下载到 iPhone 上，最简单的方式是通过 AltStore。*

AltStore，顾名思义，是 iOS 设备的替代应用商店。由 [Riley Testut](http://rileytestut.com/blog/2019/09/25/introducing-altstore/) 制造，这是在你的 iPad 或 iPhone 上下载应用程序最简单、最安全的方式。它不依赖于苹果一直在打击的企业证书，而是利用了苹果推出的一项功能，允许你使用你的 Apple ID 免费安装最多三个应用程序。

如果你觉得这听起来不错，这里有你需要知道的关于它如何运行和如何安装的一切。

## AltStore 如何工作

AltStore 需要 Apple ID 和密码，但如果你不信任它，可以创建一个一次性帐户。开发者说它从来没有被发送到任何第三方服务器。它只会被直接发送到 Apple 进行鉴定，然后安全地储存在设备的钥匙串中，因此其他任何东西都无法检索它。然而，你完全有权利对将你的主要苹果 ID 放入应用程序感到不舒服，因此有了一次性账户。

然后 AltStore 用你的 Apple ID 给应用签名，这样应用就可以运行了。你需要在你的设备设置中信任开发者证书，但当你这样做时，你通过 AltStore 安装的任何应用都将有效...七天了。苹果公司设置了一些限制，尽可能地使这个过程变得困难，但开发者设法绕过了这些限制。随着七天期限的临近，AltStore 将刷新应用程序上的签名密钥，以便您可以获得额外的七天使用时间。这也可以在后台运行。

AltStore 利用了苹果推出的一项功能，允许你使用 Apple ID 免费安装最多三个应用程序。

然而，AltStore 依赖于运行 AltServer 的同一网络上的电脑，因此您需要在该设备上安装 iTunes 和 iCloud。AltServer 是一个配套的应用程序，它会等待 AltStore 连接，应用程序只能通过 AltServer 安装和刷新。

AltServer 之所以有必要，是因为对免费苹果开发者账户的限制。不能使用免费的 Apple ID 通过无线方式分发应用程序。这意味着应用程序不能在本地安装，但可以使用 iTunes Wi-Fi sync 安装。AltServer 最初也需要安装 AltStore，但一旦安装完毕，AltStore 就可以向 AltServer 发送命令进行应用安装。你只需要确保你在同一个网络上。

## 如何安装 AltStore

你需要一台 Windows 或 Mac 电脑才能在你的 iOS 设备上安装 AltStore。你还需要安装 iTunes 和 iCloud，它们**不能**来自 Windows Store。它们需要直接从苹果下载。

现在，您可以开始 AltStore 安装过程。方法如下:

1.  **通过[山寨商店的网站](http://altstore.io/)下载山寨服务器**。
2.  将你的 **iPhone** 连接到电脑。
3.  说你**信任**你接入的电脑。
4.  启动 **AltServer** 并让它在后台运行。

接下来，您需要将它指向 iCloud 安装。

1.  打开 **iTunes。**
2.  在 iPhone 的设置中启用通过 Wi-Fi 与此 iPhone 同步**。**
3.  拔掉你的 iPhone。
4.  单击通知区域中的 AltServer 图标。
5.  点击**安装 AltStore**
6.  选择你的手机。

然后会提示您输入 Apple ID 和密码。如前所述，您可以使用一次性帐户。稍等片刻，AltStore 应该会安装在您的 iPhone 上。

## 使用 AltStore

AltStore 是一个相当简单的应用程序。它带有安装 Delta(一个模拟器)或 Clip(一个更高级的剪贴板管理器)的能力。您也可以安装您在线下载的自定 IPA 文件。

若要安装应用程序，您需要确保您与运行 AltServer 的电脑在同一个 Wi-Fi 网络上，以便在安装应用程序时(它需要由 AltServer 签名和分发)。应用程序会尝试在后台自动刷新，但当你在同一个网络上时，如果应用程序尝试在后台刷新或不刷新，那就是运气。

Testut 建议偶尔在后台启动 AltStore 应用程序，以确保它可以更频繁地检查本地服务器，因为你的手机会识别出这是一个你经常使用的应用程序。

你可以安装和试用很多应用程序，如果你[成为 Testut 赞助人](https://www.patreon.com/rileytestut)，你还可以获得 Delta 和 AltStore 的测试版。成为赞助人的最大吸引力是能够向 AltServer 添加第三方源，你可以在谷歌或 Reddit 上查找它们，找到一些添加到你的 iPhone 上。

我一直在使用 AltStore 的 Delta 来模拟一些复古游戏，我也在尝试让 Dolphin 工作。一些应用程序还不能在 iOS 15 上运行，但随着时间的推移，很多应用程序可能会更新。

你用什么自定义应用？请在下面的评论中告诉我们！