# 谷歌宣布正式支持 Android RISC-V

> 原文：<https://www.xda-developers.com/google-officially-supports-risc-v/>

谷歌开发的操作系统 Android 目前支持几种不同的指令集架构(ISAs)，如 Arm 和 x86。大多数使用 Android 的设备，包括智能手机、平板电脑、电视和智能手表，都使用基于 Arm 的芯片组。英特尔停止为手机生产 CPU，并且在 NDK 修订版 17 中取消了对 MIPS 的支持。不过有一个比较喋喋不休的 is a 就是 **R** 导出 **I** 构造**S**et**C**computer V，RISC-V，这是一个免费开放的 ISA。任何人都可以自由地设计基于它的芯片，而无需支付任何许可费或版税，谷歌在 RISC-V 峰会期间举行的公司主题演讲中宣布了对它的官方支持。

RISC-V 很特别，因为它是一个免费开放的 ISA，希望制造廉价物联网产品的供应商将有兴趣使用 RISC-V 开发低成本芯片。与此同时，寻求减少对竞争对手或外国实体依赖的公司也将认真寻找。有趣的是，[谷歌已经在谷歌 Pixel 系列的 Titan M2 安全芯片中使用了](https://security.googleblog.com/2021/10/pixel-6-setting-new-standard-for-mobile.html)RISC-V 架构，而[英特尔现在提供](https://www.xda-developers.com/intel-arizona-factories-make-chips-other-companies/)为商业客户制造 RISC-V 芯片组。

在该公司的主题演讲中，Android 的工程总监拉斯·博格斯特伦说，他希望 RISC-V 被视为 Android 中的“一级平台”。这相当于 Arm 目前对 Android 的地位，面对谷歌此前似乎完全不感兴趣的事情，这是一个相当大胆的举措。ArsTechnica 的 Ron Amadeo 在 Google I/O 2022 大会上询问 Android 团队是否支持 RISC-V 时，Android 团队似乎暗示 RISC-V 不会很快出现。Amadeo 关于未来 RISC-V 支持的问题得到的回答是“我们正在观察，但对我们来说这将是一个很大的变化。”

博格斯特伦说，你现在可以下载并试用非常有限的 RISC-V 版本的 Android，但它缺乏对 Java 工作负载的 Android 运行时(ART)的支持。他说，他预计官方模拟器支持很快就会到来，ART 将于 2023 年在 Q1 推出。他分享了上面的幻灯片，该幻灯片显示，虽然要让 AOSP 在 RISC-V 上起步还有很多工作要做，但该公司致力于该架构。

最棒的是，开发人员不必做太多工作就能让他们的应用在 RISC-V 设备上运行。ART 基本上将字节码“翻译”成运行它的设备的本机指令，所以它将被翻译成 RISC-V 而不是 Arm。本机代码是一个不同的故事，但 Java 代码构成了大多数 Android 应用程序的全部。

至于为什么公司可能会从 Arm 跳槽，有几个原因。首先，该公司一直非常不稳定。其所有者软银曾试图将该公司出售给英伟达，但未果。此外，Arm 已经成为华为等公司遭受贸易制裁的一枚棋子，被迫中断联系数月。更糟糕的是， [Arm 已经起诉高通收购 Nuvia】，起诉你们最大的客户之一看起来不太好。](https://www.xda-developers.com/arm-suing-qualcomm-over-nuvia/)

RISC-V 被视为摆脱西方依赖的一种方式，这很大一部分是因为 RISC-V 国际公司在瑞士注册成立。它可以作为美国和中国的中立方，使其成为寻求设计芯片组的公司的一个有吸引力的选择。阿里巴巴是 RISC-V 的最大支持者之一，该公司的[工程师两年前将 Android 10 移植到 RISC-V 主板上](https://www.xda-developers.com/android-risc-v-port/)。

在接下来的几个月里，我们将拭目以待 RISC-V 的发展。虽然我们可能需要一段时间才能在市场上看到可行的 RISC-V 芯片组旗舰设备，但谷歌为公司打开了尝试的大门。

* * *

**来源:[谷歌](https://www.youtube.com/watch?v=70O_RmTWP58)**

Via: [ArsTechnica](https://arstechnica.com/gadgets/2023/01/google-announces-official-android-support-for-risc-v/)