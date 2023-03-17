# 谷歌代号显示了两款 2020 像素的中端手机，分别是 5G 的骁龙 765 和 4G 的骁龙 730

> 原文：<https://www.xda-developers.com/google-pixel-2020-code-names-snapdragon-765-snapdragon-730/>

每年 10 月，我们预计谷歌将发布一款新的 Pixel 智能手机，竞争最佳安卓手机。2016 年，该公司推出了第一代 Pixel 和 Pixel XL。2017 年，我们看到了 Pixel 2 和 Pixel 2 XL。2018 年谷歌宣布 Pixel 3 和 Pixel 3 XL 时没有任何惊喜。然而，去年谷歌在 2019 年谷歌 I/O 大会上宣布了第一批中端 Pixel 手机 Pixel 3a 和 3a XL。虽然该公司后来在去年 10 月份发布了 Pixel 4 和 4 XL，但 3a 系列的推出让我们预计今年会有后续产品。事实上， *@ [Onleaks](https://twitter.com/OnLeaks)* ，一个著名的智能手机泄密者，[共享 CAD 渲染](https://www.xda-developers.com/google-pixel-4a-leaked-renders-punch-hole-display-headphone-jack/)很可能是 2020 年中期的 Pixel 4a。

今天早些时候，Twitter 用户@ [akes29](https://twitter.com/akes29) 向我们发送了一条提示，其中包含一些他认为与 2020 年新像素设备相关的代码名称。我们挖掘了 Android 开源项目(AOSP)，本月最新的 Pixel 4 固件转储，以及几个谷歌应用程序的最新版本，发现了 3 个新的设备代码名称以及它们所基于的 SoC 平台。这些代号表明，谷歌可能正在研究不止一个中端 2020 像素——其中一个很可能是 Pixel 4a。假设谷歌没有打破传统，为每一代新的 Pixel 推出更小的 XL 型号，那么我们预计也会有 Pixel 4a XL。然而，今年可能不会是这样了——YouTuber Dave Lee 声称不会有 4a XL 型号。不过，我们对这种说法有所保留，因为李没有引用任何具体的证据。此外，李的说法与谷歌早些时候关于存在 XL 型号的报道相矛盾。我们今天的发现支持了谷歌的报告，尽管遗憾的是，我们无法提前这么长时间将这些代号与实际产品直接联系起来。

*传闻中的谷歌 Pixel 4a。来源:[@ on leaks x 91 mobiles](https://www.91mobiles.com/hub/google-pixel-4a-design-renders-punch-hole-display-exclusive/)*

## 2020 年像素手机的新代号

如果你不熟悉，谷歌每款 Pixel(和 Nexus)智能手机的内部代号都与某种鱼有关。当我们第一次看到谷歌下一代 Pixel 设备的传言时，我们通常会从它们的代号开始。关于 2018 款像素的最早传言是关于它们的代号:blueline(作为 Pixel 3 推出)、crosshatch(作为 Pixel 3 XL 推出)、albacore(从未推出)和 wahoo(作为 Pixel 3 和 3 XL 的[统一内核)。甚至谷歌未发布的、](https://www.xda-developers.com/wahoo-google-pixel-2018/) [HTC 制造的 Pixel 2 XL](https://www.xda-developers.com/htc-u11-google-pixel-2-xl-muskie/) 也有一个可疑的代号( [muskie](https://www.xda-developers.com/unreleased-htc-google-pixel-2-with-3830-mah-battery/) )。)作为参考，这里列出了所有 Pixel 手机及其代号。

| 

营销名称

 | 

代号

 |
| --- | --- |
| 像素 | 旗鱼 |
| 像素 XL | 枪鱼 |
| 像素 2 | 斜视 |
| 像素 2 XL | 哲罗鱼 |
| 像素 3 | 蓝线 |
| 像素 3 XL | 以交叉线作出阴影 |
| 像素 3a | 萨尔戈 |
| 像素 3a XL | 鲣鱼 |
| 像素 4 | 火焰 |
| 像素 4 XL | 珊瑚 |

去年四月， *9to5Google* [发现](https://www.xda-developers.com/google-pixel-4-xl-mysterious-third-device-codename/)提到了一个代号为 needlefish 的谷歌设备。虽然我们已经在[多个](https://twitter.com/MishaalRahman/status/1206394771423584256)和[谷歌应用](https://www.xda-developers.com/google-pixel-4-camera-features-google-camera-leak/)中看到过，但是这种代号的设备还没有发布。Twitter 用户@akes29 向我们指出了 needlefish 可能只是谷歌基于骁龙 855 的开发板的证据，因为该设备似乎是基于“sm8150p”平台。Sm8150 是高通骁龙 855 的代号，而 sm8150p 似乎是骁龙 855 移动硬件开发套件的特定代号。虽然我们不能完全排除针鱼作为商业产品出现的可能性，但根据最近的证据，这种可能性似乎更小。这让我们发现了三个新的代号:**太阳鱼、红鳍金枪鱼和荆棘鱼**。

[**翻车鱼**](https://en.wikipedia.org/wiki/Ocean_sunfish)

我们在 AOSP 的一个库中发现了“sunfish”的代号，并直接表示它是基于 sm7150 平台的。这是高通骁龙 730 SoC 的代号，这是一款面向中端设备的 SoC。这种 SoC 可以在 Redmi K30、 [Realme X2](https://www.xda-developers.com/realme-x2-review-snapdragon-730g-gaming/) 和[三星 Galaxy A71](https://www.xda-developers.com/samsung-galaxy-a71-punch-hole-display-64mp-quad-rear-camera/) 等设备中找到，它不支持 5G 调制解调器。Sunfish 有两个开发分支:一个基于 Android 10，另一个基于 Android 11。由于我们还在谷歌应用程序的一个字符串中发现了 sunfish 的代号，以及其他 Pixel 设备，因此这个代号很可能属于 Pixel 4a。至少，它很可能是一个真实的设备，即使它最终是一个开发板。不过，如果它只是一个开发板，我们希望看到基于 sm7150 平台的器件有另一个代号。

[**雷德芬**](https://en.wikipedia.org/wiki/European_perch)

我们名单上的下一个代号是“红鳍”这个代号可能是正在 sm7250 或[高通骁龙 765](https://www.xda-developers.com/qualcomm-snapdragon-765-processor-specifications-features/) 移动平台上开发的设备(或开发板)。骁龙 765 是高通最新的中端 SoC，也是高通首款集成 5G 调制解调器的 SoC。“redfin”似乎是由 ODM 制造的，在这种情况下，是富士康的子公司 FIH 移动。它是用 Android 10 开发的。除了 AOSP，我们没有在任何其他来源上发现任何关于“redfin”的参考——无论是在线还是离线。

[**树莓**](https://en.wikipedia.org/wiki/Bramble_shark)

荆棘是我们发现的第三个代号。它在 AOSP 出现了多次，尽管最初我认为它是谷歌的骁龙 865 开发版本，因为它运行的是 Linux 内核版本 4.19。然而，这是一个错误的假设，因为高通的骁龙 765 也应该基于 Linux 内核版本 4.19。事实上，由于新的 AOSP 承诺，我们现在知道 bramble 和 redfin 一样，都是基于 sm 7250/骁龙 765 移动平台。然而，与 redfin 不同，我们还没有找到 bramble 是 ODM 设备的证据，它似乎正在与 Android 10 和 Android 11 一起开发。

* * *

虽然我们不能确定 redfin、bramble 和 sunfish 是否真的是中端像素设备，但在未来几周和几个月内，我们应该会在 AOSP 和谷歌应用程序中看到更多关于这些代号的引用。我们目前认为，sunfish 可能是仅支持 4G 的 Pixel 4a，而 bramble 或 redfin 可能是支持 5G 的 Pixel 4a XL。我认为今年不会有 3 款中端 2020 Pixel 手机，因此 redfin 或 bramble 中的一款可能是商用设备，而另一款则是开发板。拥有一个略高端的带 5G 连接的 4a XL 型号可以解释*9 到 5Google* 听到的关于它的定价的消息——据推测，它将比 3a XL 更贵。