# Google 列出了哪些 Firebase SDKs 需要 Google Play 服务

> 原文：<https://www.xda-developers.com/google-list-firebase-sdk-require-google-play-services/>

# Google 列出了哪些 Firebase SDKs 需要 Google Play 服务

考虑在你的应用中实现一个或多个 Google 的 Firebase SDKs？查看此列表，了解他们是否依赖 Google Play 服务！

谷歌在 Android 领域是一个相当普遍的名字。该公司不仅拥有并维护 Android 开源项目本身，还负责 Android 上最大的分发平台:谷歌 Play 商店和底层的谷歌移动服务(GMS)套件。GMS 是这里的重要部分。Firebase 是谷歌的跨平台工具包，用于分析和崩溃检测等，它使用 GMS 来提供许多功能。

如果你的目标设备预装了 Google apps，那当然很好，但如果没有呢？如果用户解锁了他们的引导加载程序，并刷新了一个谷歌免费的 ROM，会怎么样？如果有人正在使用华为设备，或者他们从中国进口了一部手机，该怎么办？你的应用程序中依赖于 Firebase 的部分会不会不起作用？

令人欣慰的是，如果你试图在你的应用中实现 Firebase，你不需要猜测哪些 SDK 可以在无谷歌的设备上工作，哪些不能。谷歌已经发布了一份清单，列出了所有当前的 Firebase SDKs，以及它们是否依赖 GMS。您可以使用它来快速判断哪些 SDK 可以安全实现，哪些 SDK 需要补充或避免。

下表列出了 Firebase SDKs 以及它们是否具有 GMS 依赖性:

| 

图书馆

 | 

GMS 状态

 |
| --- | --- |
| 播放服务广告 | 需要 |
| 分析学 | 被推荐的 |
| 应用程序索引 | 需要 |
| 证明 | 需要 |
| Firestore | 不需要 |
| 功能 | 不需要 |
| 信息发送 | 需要 |
| 储存；储备 | 不需要 |
| 碰撞分析 | 不需要 |
| 动态链接 | 需要 |
| ML 视觉 | 需要 |
| ML 模型解释程序 | 需要 |
| 应用内消息 | 不需要 |
| 应用内消息显示 | 不需要 |
| 装置 | 不需要 |
| 表演 | 需要 |
| 数据库ˌ资料库 | 不需要 |
| 配置 | 不需要 |

数量惊人的 Firebase SDKs 在没有安装 GMS 的情况下也能正常工作。通过正确的实现，即使没有 GMS 也可以使用身份验证 SDK。

请记住，这个列表仅在 9 月 6 日这篇文章发表时才是准确的。随着 SDK 在 Firebase 中的添加、更新或删除，未来可能会有所改变。要了解最新信息，以及在没有 GMS 的情况下使用 Firebase 身份验证的变通方法，[请查看 Google 的页面](https://firebase.google.com/docs/android/android-play-services)。