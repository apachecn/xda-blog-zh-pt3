# 谷歌通过测试版客户端加密提高 Gmail 在工作空间的安全性

> 原文：<https://www.xda-developers.com/gmail-client-side-encryption-test/>

具有兼容付费计划的精选 Google Workspace 管理员现在有了另一种方法来为他们的最终用户保护 Gmail。这是因为谷歌最近宣布在网络上为 Gmail 进行客户端加密测试，测试计划将持续到 2023 年 1 月 20 日。

这个新的测试版将 Gmail 套件的安全性(有时更重要)提升到了一个全新的水平。Gmail 已经允许在谷歌服务器之间移动时加密静态和传输中的数据，但客户端加密更安全，也更符合监管规定。无论是在公司域内还是域外，[电子邮件正文和附件以及内嵌图像现在都将在接收端和发送端完全加密。电子邮件的标题，包括主题、时间戳和收件人，则不会。请注意，这仅适用于 Google Workspace Enterprise Plus、Education Plus 和教育标准版计划，然而，个人 Google 帐户上的消费者帐户将看不到该功能。](https://www.xda-developers.com/best-email-apps-android/)

当然，要实现这一点，所有接收者都需要首先启用客户端加密，并打开该功能，以及有效的证书。目前，这是由 it 管理员通过申请测试程序来完成的。一旦管理员在 Google Workspace 上启用它，你可以点击电子邮件撰写框的右上角，选择**消息安全**。从那里，在**附加加密**下，用户可以选择**开启选项**并照常发送消息，或者登录到身份提供商。收到加密邮件的人将会看到原始 enders 姓名下方的**加密邮件**，并会被提示登录到身份提供商以在 Gmail 中解密。

对该功能感兴趣的 IT 管理员可以访问谷歌的支持页面寻求帮助。一旦一个组织进入测试版，该功能将被默认关闭。如果需要，可以在域、OU 和组级别启用它。

**来源:** [谷歌](https://workspaceupdates.googleblog.com/2022/12/client-side-encryption-for-gmail-beta.html)