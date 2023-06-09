# 谷歌助手准备让你用手机支付油费

> 原文：<https://www.xda-developers.com/google-assistant-pay-for-gas-from-phone/>

还记得 CES 吗？似乎世界上最大的科技事件发生在很久以前，所以很容易忘记有这么多新产品和服务在那里宣布。举个例子，亚马逊为 Alexa 新推出的“[支付汽油](https://www.amazon.com/b?tag=xda-3hi2p3q-20&ascsubtag=UUxdaUeUpU30324&asc_refurl=https%3A%2F%2Fwww.xda-developers.com%2Fgoogle-assistant-pay-for-gas-from-phone%2F&asc_campaign=Short-Term)”服务。该功能允许司机要求 Alexa 在全美超过 11，000 个加油站处理燃料支付。你所要做的就是开到加油站，启动 Alexa，说“支付汽油”，然后按照指示激活泵为你的汽车加油。根据最新版本的谷歌应用程序(准确地说是 11.33.5.29 版)中的代码，看起来谷歌正准备为谷歌助手添加一个类似的功能。

**APK 的拆卸通常可以预测应用程序未来更新中可能出现的功能，但有可能我们在这里提到的任何功能都不会在未来的版本中出现。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。**

在最新版本的谷歌应用程序中，有一个名为“aa_pay_for_gas_query”的新字符串这是谷歌助手可以识别的硬编码查询之一，还有其他几个查询，比如播放平静声音的查询。

```
 <string name="aa_pay_for_gas_query">Pay for gas.</string> 
```

深入挖掘 APK，我们发现有证据表明这一新功能可以通过另一种方式启动:通过启动器上的概览小部件。当您到达一个加油站时，一览窗口小部件将更新为“At [station name]。”点击该小工具将发送一个意图，以查看带有几个 URI 参数的 https://pay.google.com/gas/payment(可能会被 Google Pay 应用程序识别)，包括品牌和商店 ID。据推测，这意味着你将能够在多个不同的加油站连锁店用谷歌助手支付汽油费。例如，亚马逊 Alexa 可以让你在埃克森和美孚的 11，500 多个地点付款。

谷歌应用程序中没有多少代码详细介绍这项功能，我们自己也还不能激活它。这意味着你应该半信半疑地看待这个消息，但鉴于亚马逊已经为 Alexa 推出了类似的功能，谷歌效仿 Assistant 是完全合理的。

*感谢 PNF 软件为我们提供使用许可**[JEB Decompiler](https://www.pnfsoftware.com/?aid=xdadev)**，这是一款针对 Android 应用的专业级逆向工程工具。*