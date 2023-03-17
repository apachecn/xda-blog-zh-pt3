# 华为为 Mate 30 推出集成 5G 的麒麟 990

> 原文：<https://www.xda-developers.com/huawei-hisilicon-kirin-990-5g-integrated-modem/>

2019 年迄今为止，大多数重大公告都围绕 5G 展开，5G 是网络技术的下一个进步。大多数半导体公司都加入了 5G 潮流，推动智能手机原始设备制造商生产可以利用网络基础设施改善的设备。然而，迄今为止发布的大多数支持 5G 的 SOC 基本上都是 4G 芯片，带有一个额外的 5G 调制解调器来支持 5G 功能。三星刚刚宣布了集成 5G 调制解调器的 [Exynos 980 SoC，现在，华为紧随其后，推出了自己的 5G 集成旗舰 SoC。华为推出的海思麒麟 990 5G 与麒麟 990 一起在 2019 年 IFA 发布。](https://www.xda-developers.com/samsung-exynos-980-5g-modem/)

* * *

## 规格-麒麟 990 和麒麟 990 5G

| 

规范

 | 

麒麟 980

 | 

麒麟 990

 | 

麒麟 990 5G

 |
| --- | --- | --- | --- |
| **流程** | 7 纳米 | 7 纳米 | 7 纳米+ EUV |
| **CPU** | 

*   2 个 Cortex-A76 @ 2.6GHz
*   2 个 Cortex-A76 @ 1.92GHz
*   4x Cortex-A55 @1.8GHz

 | 

*   2 个 Cortex-A76 @2.86GHz
*   2x Cortex-A76 @2.09GHz
*   4x Cortex-A55 @1.86GHz

 | 

*   2 个 Cortex-A76 @2.86GHz
*   2x Cortex-A76 @2.36GHz
*   4x Cortex-A55 @1.95GHz

 |
| **GPU** | 马里-76 国集团 MP10 | 马里-G76 MP16 | 马里-G76 MP16 |
| NPU | 两个内核，剑桥架构 | 1 个大核+ 1 个小核，达芬奇建筑 | 2 个大核+ 1 个小核，达芬奇架构 |
| **调制解调器** | 第四代移动通信技术 | 第四代移动通信技术 | 巴龙 5000，5G |

麒麟 990 5G 成为全球首款旗舰 5G SoC 之一。但是，不管围绕 5G 的宣传如何，实际的现实是，网络技术仍处于发展阶段，5G 要像 4G 一样普及还需要相当长的时间。对于大量消费者来说，这意味着 5G 在智能手机上的存在将只是一个他们无法使用的功能，这些用户不在不必要的硬件上花费额外的费用是有意义的。华为认识到了这一点，因此该公司发布了一款非 5G/4G 版本的旗舰 SoC。在大多数情况下，标准的麒麟 990 与麒麟 990 5G 相同，但也有一些差异。为了避免混淆，我们将在标准的麒麟 990 上添加 4G。

麒麟 990 5G 基于 7 纳米极端紫外(EUV)光刻工艺，而 4G 版本在 EUV 光刻工艺中失败，而是与麒麟 980 基于相同的 TSMC 7 纳米。华为声称，配备集成 Balong 5G 调制解调器的麒麟 990 5G 比配备 [X50 5G 调制解调器](https://www.xda-developers.com/qualcomm-announces-x16-and-x50-modems-for-next-generation-snapdragon-8xx-devices-and-5g-connectivity/)的高通[骁龙 855](https://www.xda-developers.com/qualcomm-snapdragon-855-sdx50-5g-modem/) 更小。该芯片还支持全频率 5G 非独立(NSA)和独立(SA)架构，以及全频率 TDD/FDD 频段。Balong 5000 集成调制解调器允许这款旗舰 SoC 实现 2.3Gbps 的峰值下行链路速率和 1.25Gbps 的峰值上行链路速率。

在性能方面，两款新的麒麟 990 都配备了由两个 Cortex-A76 主内核、两个 Cortex-A76 大内核和四个 Cortex-A55 小内核组成的 CPU 设置。两种芯片组之间的频率设置会发生变化，这实质上让 5G 变体以微小的优势脱颖而出。GPU 任务由具有 16 核设置的 Mali-G76 处理。这两款 SOC 都配备了新的系统级智能缓存，支持“智能流量分配”，旨在节省带宽和功耗。还有一个升级的麒麟游戏+ 2.0 板载，但目前还不清楚这将转化为营销之外的话。

5G 变体和 4G 变体之间的另一个关键区别点是 NPU，因为 5G 变体基于达芬奇架构，配备了一个双大核和一个小核 NPU，而 4G 变体“只”配备了一个大核和一个小核。大内核在繁重的计算场景中实现高性能和高能效，而小内核结构则支持超低功耗 NPU 应用。

图像信号处理器也有所升级，因为华为声称麒麟 990 系列配备了“全新”的 ISP 5.0，利用块匹配和 3D 过滤(BM3D)进行基于硬件的降噪，让手机理论上在弱光下捕捉更亮更清晰的图像。考虑到华为 P30 Pro 是[现有的最佳弱光拍摄者之一](https://www.xda-developers.com/huawei-p30-pro-camera-review-50x-zoom/)，我们倾向于相信华为在这方面的说法。麒麟 990 系列还首次使用双域视频降噪技术，对视频进行更精确的噪声处理。还有基于 AI 分割的实时视频后期处理和渲染，可以逐帧调整图像颜色。

新的麒麟 990 和麒麟 990 5G 将出现在即将到来的[华为 Mate 30 系列智能手机](https://www.xda-developers.com/huawei-mate-30-pro-7-cameras/)中，预计[将于 2019 年 9 月 19 日在欧洲](https://www.xda-developers.com/huawei-mate-30-september-19th/)推出。我们也应该看到旗舰 SoC 系列在 2019 年和 2020 年的其他未来华为和 Honor 旗舰上使用。

* * *

*带有来自[Anand tech](https://www.anandtech.com/show/14851/huawei-announces-kirin-990-and-kirin-990-5g-dual-soc-approach-integrated-5g-modem)的附加输入*