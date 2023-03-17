# Galaxy Watch 3 固件:三星下一代智能手表有什么新功能

> 原文：<https://www.xda-developers.com/galaxy-watch-3-firmware-analysis-samsung-smartwatch-new-features/>

三星即将推出的产品往往会受到很多关注，因为它们会在现场引起多大的轰动。鉴于 Wear OS 和骁龙 Wear 处理器的糟糕状况，许多 Android 粉丝坚持等待基于 Tizen 的三星 Galaxy Watch 3 发布也就不足为奇了。由于最近的一次公开固件泄露，我们了解到了三星即将推出的智能手表的大量信息，包括大部分规格和功能。以下是我们目前为止发现的关于三星 Galaxy Watch 3 的一切。

但首先，简单回顾一下。三星 Galaxy Watch 3 将是 2018 年年中发布的原始 Galaxy Watch 的继任者。三星在 Galaxy Watch 和 Galaxy Watch 3 之间发布了几款智能手表，包括 Galaxy Watch Active 和 Galaxy Watch Active 2，但它们跳过了“Galaxy Watch 2”品牌。不过，别搞错了:除了名字，这是一款 Galaxy Watch 2。[三星的 Galaxy 可穿戴应用](https://www.xda-developers.com/galaxy-wearable-confirms-next-samsung-smartwatch-galaxy-watch-3-next-galaxy-buds-bean-shape/)证实了这个名字已经[提交了几份认证文件](https://www.xda-developers.com/first-look-samsung-galaxy-watch-3/)。我们已经[看到了智能手表](https://www.xda-developers.com/samsung-galaxy-watch-3-leak-display-on/)、[高质量(甚至 3D)渲染](https://www.xda-developers.com/samsung-galaxy-watch-3-leaked-render-clearest-look-upcoming-tizen-os-smartwatch/)和[部分规格表](https://www.xda-developers.com/samsung-galaxy-watch-3-specs-leak-battery-dimensions-ecg/)的照片。现在，我们准备为尚未发布的 Galaxy Watch 3 智能手表的公开固件添加更多燃料。

## Galaxy Watch 3 规格

|  | 

银河手表 3 41 毫米

 | 

Galaxy Watch 3 45mm 毫米

 |
| --- | --- | --- |
| 型号 | SM-R850 | SM-R840 |
| 社会学 | Exynos 9110 | Exynos 9110 |
| Tizen 版本 | 5.5.0.0 | 5.5.0.0 |
| 一个用户界面版本 | 2.0 | 2.0 |
| 充电器瓦特数 | 5W | 5W |
| 蓄电池容量 | 247 毫安时 | 340 毫安时 |
| 扬声器 | 是 | 是 |
| 国家足球联盟 | 是 | 是 |
| 显示分辨率 | 360x360 有机发光二极管 | 360x360 有机发光二极管 |
| 健康传感器 | TI AFE4930 | TI AFE4930 |

在我们为 Galaxy Watch 3 发送的固件转储中，我们能够为三星智能手表的两个主要变体编译上述规格表。我们预计这两款智能手表都将采用 Exynos 9110 SoC，这是与最初的 Galaxy Watch、Galaxy Watch Active 和 Galaxy Watch Active 2 相同的 10 纳米芯片。

41 毫米的 Galaxy Watch 3 应该有 247 毫安时的电池，而更大的 45 毫米型号应该有 340 毫安时的电池。虽然显示屏尺寸有 4 毫米的差异，但两款智能手表的显示屏分辨率是相同的，都是 360x360。当然，三星将在手表上使用他们自己的有机发光二极管面板。这两款手表都有扬声器，所以你可以打语音电话。在内部，两款智能手表都将支持 NFC，但不支持通过 Samsung Pay 支付的 MST。Galaxy Watch 3 中使用的健康传感器是德州仪器的 AFE4930。这是对 Galaxy Watch Active 2 中使用的 TI AFE4920 传感器的微小升级。

## 看脸

在固件中，我还能够找到三星 Galaxy Watch 3 将包含的新手表外观。有几个数字表盘和几个模拟表盘。每个人都有自己的风格。

随着三星 Galaxy Watch 3 上的表盘，我们获得了新的信息丰富的数字边缘。在前三张图片中，你可以看到手表外面有四个圆形的横条。这些信息边缘可以用许多选项来定制。这些选项包括世界时钟、语音备忘录、计时器、秒表、日程安排、提醒、PowerPoint 控制器、音乐、信息、电子邮件、通话记录、Bixby、气压计、闹钟、最近的应用程序、跑步、步行、骑自行车、徒步旅行、游泳、室外游泳、跑步机、健身车、椭圆、其他锻炼、女性健康、水、食物、呼吸、压力、心率、睡眠、卡路里、睡眠、步数、日常活动、日落、紫外线指数、空气质量、降雨概率、感觉温度、日期和天气、天气、字母组合、日历日、电池百分比或无。

信息丰富的边缘也将获得一个选项，有一个数字建议。从我对手表 face 文件的理解来看，它会自动在步数、电池、心率、卡路里或天气之间切换，这取决于手表软件在当时决定什么是最重要的。

另一个上面没有列出的表盘是一个新的天气表盘。手表的背景会显示一个模拟天气的动画。如果在下雪，背景会显示雪。在阳光明媚的日子，你会看到太阳。每当你看 Galaxy Watch 3 的显示屏时，另一个手表表面只会显示一朵动画花或气泡(由用户选择)。

## 应用程序更新

一个主要变化是 Galaxy Watch 3 上的电子邮件应用程序。三星电子邮件将不再包含在智能手表中。取而代之的是微软的 Outlook。微软和三星早在几年前就有了长期的合作关系，这并不奇怪。虽然我可以看到该应用程序预装在手表上，但它可能需要用户在他们的设备上使用 Outlook 应用程序，而不是三星电子邮件应用程序。对于 Galaxy 用户，它需要安装另一个应用程序，但对于其他 Android 用户，它将允许电子邮件功能工作。

## 不是来自固件的东西

我们已经看到了一些关于三星 Galaxy Watch 3 的不同泄漏，这些泄漏不是源于固件。Evan Blass 最近在推特上表示，三星 Galaxy Watch 3 将有 9 个不同的版本:41 毫米的青铜色和银色蓝牙型号，41 毫米的青铜色和银色 LTE 型号，45 毫米的银色和黑色蓝牙型号，45 毫米的银色和黑色 LTE 型号，以及 45 毫米的黑色钛蓝牙型号。你可以在[我们之前写的文章](https://www.xda-developers.com/samsung-galaxy-watch-3-leaked-render-clearest-look-upcoming-tizen-os-smartwatch/)中找到这些特定模型的图片。

最近来自 *[Gizmodo UK](https://www.gizmodo.co.uk/2020/07/exclusive-the-samsung-galaxy-watch-3-is-coming-next-month-with-some-questionable-gesture-control/)* 的一份报告也谈到了一些新的有趣的手势，我们还没有在固件中找到证据。三星显然将引入手腕手势来控制手表的不同方面。根据 *Gizmodo* 获得的泄露图片，表演拳头泵会接电话，而摇拳头会拒接电话。可能还会有一个手势让你把智能手表放到嘴边来激活 Bixby，类似于你在 Apple Watch 上激活 Siri 的一种方式。该报告还提到跌倒检测和心电图监测支持包括在内。目前，心电图和血压监测似乎只会在韩国推出，随后会在更多国家推出，这并不奇怪，因为他们已经在韩国测试 Galaxy Watch Active 2 上的[。报告最后提到，将有一个跑步教练，可以在你跑步时帮助你的速度，并在你完成后提供更多信息。](https://www.xda-developers.com/samsung-galaxy-watch-active-2-ecg-monitoring-approved-south-korea/)

*图片来源:[Gizmodo UK](https://www.gizmodo.co.uk/2020/07/exclusive-the-samsung-galaxy-watch-3-is-coming-next-month-with-some-questionable-gesture-control/)*

有证据表明，Galaxy Watch 3 可能会在本月晚些时候推出。埃文·布拉斯此前曾表示，他认为发布日期是 7 月 22 日，通常是新闻渲染上显示的日期。这意味着我们可以看到三星的新智能手表很快就会发布。不过，这个日期仍然有可能是错误的，Galaxy Watch 3 实际上是在 8 月 5 日的[发布的，仅在线的三星与](https://www.xda-developers.com/samsung-galaxy-note-20-fold-2-unpacked-online/) [Galaxy Note 20](https://www.xda-developers.com/tag/samsung-galaxy-note20/) 和 [Galaxy Z Fold 2](https://www.xda-developers.com/samsung-galaxy-z-fold-2-name/) 一起发布。无论如何，我们将密切关注 Galaxy Watch 3 和其他三星产品的更多信息，因此如果我们了解到任何新的信息，我们会让你知道。