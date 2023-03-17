# 英特尔详细介绍了旨在挑战 ARM 的全新 Lakefield 处理器

> 原文：<https://www.xda-developers.com/intel-lakefield-processors-launch-sunny-cove-tremont/>

英特尔一直是移动领域的后起之秀。该公司的移动 Atom SoC 业务在 2015 年随着华硕 ZenFone 2 的推出而展现出希望，但随后在 2016 年被取消。调制解调器行业被嘲笑为技术不如高通的调制解调器。当苹果成为调制解调器的最大客户，仅在 iPhone 中使用调制解调器时，英特尔获得了第一次重大突破，但在 2019 年，高通和苹果[就他们的法律纠纷](https://www.xda-developers.com/qualcomm-accuses-apple-stealing-secrets-giving-intel/)达成了和解。因此，英特尔别无选择，只能停止移动调制解调器业务，讽刺的是，这项业务后来被卖给了苹果。目前，英特尔没有涉足智能手机领域，无论是智能手机 SOC 还是调制解调器芯片。然而，该公司继续追求为 2 合 1 设备、笔记本电脑、可折叠设备等供电的低压芯片。英特尔的 Core M 被重新命名为 Core Y 系列，目前仍用于苹果 MacBook Air 等笔记本电脑。现在，英特尔透露了更多关于其即将推出的“Lakefield”芯片的细节，这些芯片不是 Atom 芯片，也不是纯粹的 Core 芯片(尽管它们将被标记为“Intel Core”阵容的一部分)。它们可以被视为 Core M/Core Y 系列理念的继承者，旨在巩固英特尔在超移动设备领域相对于 ARM 的领导地位。

自去年以来，英特尔一直在戏弄莱克菲尔德芯片，但这些芯片直到周三才正式推出。Lakefield 是英特尔的第一个混合 CPU 计划(想想英特尔相当于 ARM 的 big。多集群计算的 LITTLE 和 DynamIQ 概念)。Lakefield 计划利用英特尔的 Foveros 3D 封装技术，并采用混合 CPU 架构来实现功率和性能的可扩展性。英特尔表示，Lakefield 处理器是最小的处理器，可提供英特尔酷睿性能和全面的 Windows 兼容性，支持超轻和创新外形的工作效率和内容创作体验。(“完全 Windows 兼容性提及”是对高通的一次抨击，他的[骁龙 8c](https://www.xda-developers.com/qualcomm-snapdragon-8c-snapdragon-7c-announced/) 和[8cx](https://www.xda-developers.com/qualcomm-snapdragon-8cx-battery-life-performance-benchmarks-windows-10/)SOC 使用仿真来使用 Windows 上的 Win32 软件。)

根据英特尔的说法，采用英特尔混合技术的英特尔酷睿处理器提供了完整的 Windows 10 应用兼容性，封装面积减少了 56%，主板尺寸减少了 47%，电池续航时间延长。这为 OEM 厂商在单、双和可折叠显示设备的外形设计方面提供了更大的灵活性。Lakefield 处理器是首款附带层叠封装内存(PoP)的英特尔酷睿处理器，进一步减小了主板尺寸。它们也是首款待机 SoC 功耗低至 2.5mW 的核心芯片，与 Y 系列芯片相比，待机 SoC 功耗降低高达 91%。最后，它们是第一款具有原生双内部显示管道的英特尔处理器，英特尔表示，这使它们“非常适合”可折叠和双屏电脑。

第一批宣布的由 Lakefield 处理器支持的设计包括[联想 ThinkPad X1 Fold](https://www.xda-developers.com/lenovos-foldable-thinkpad-x1-fold/) ，这是在 CES 2020 上宣布的世界上第一款在个人电脑中使用的折叠有机发光二极管显示器(售价 2499 美元)。预计将于今年晚些时候上市。[三星 Galaxy Book S](https://www.xda-developers.com/samsung-galaxy-book-s-intel-lakefield-lte/) 预计将于本月开始在特定市场发售。[微软 Surface Neo](https://www.xda-developers.com/microsoft-surface-duo-suface-neo-surface-pro-7-surface-laptop-3/) ，一款定于 2020 年第四季度发货的双屏设备，也采用了 Lakefield 平台。

Lakefield 处理器将作为采用英特尔混合技术的英特尔酷睿 i5 和 i3 系列的一部分。它们拥有一个 10 纳米 Sunny Cove 内核(这与支持 Ice Lake 和即将推出的 Tiger Lake 的微架构相同)，将用于更密集的工作负载和前台应用，而四个高能效的 Tremont 内核(通常支持 Atom 芯片)用于不太密集的任务。这两种处理器都完全兼容 32 位和 64 位 Windows 应用程序，但正如 AnandTech 指出的那样，它们使用不同的指令集。两组内核都可以访问 4MB 末级高速缓存。

Foveros 3D 堆叠技术使 Lakefield 处理器能够显著减少封装面积。它现在只有 12x12x1 毫米，英特尔指出这大约是一个硬币的大小。这种减小是通过堆叠两个逻辑管芯和两层 DRAM 以及三维来实现的。这也消除了对外部存储器的需求。

对于不同架构的多核 CPU，调度成为一个重要的课题。英特尔表示，Lakefield 平台使用硬件引导的操作系统调度。这支持 CPU 和操作系统调度程序之间的实时通信，以便在正确的内核上运行正确的应用。英特尔表示，混合 CPU 架构的每 SoC 功耗性能提高了 24%，单线程整数计算密集型应用性能提高了 12%。所有这些比较都是针对英特尔酷睿 i7-8500Y，这是一款 14 纳米琥珀湖 Y 系列酷睿 i5 芯片。

对于人工智能增强的工作负载，英特尔 UHD 显卡的吞吐量提高了 2 倍以上。英特尔表示，其灵活的 GPU 引擎计算支持持续的高吞吐量推理应用，包括分析、图像分辨率升级等。与酷睿 i7-8500Y 相比，Lakefield 平台的图形性能提升了 1.7 倍。第 11 代显卡为 7W 英特尔芯片带来了最大的图形飞跃。视频转换速度可提高 54%，并支持多达四个外部 4K 显示器。最后，Lakefield 芯片支持英特尔的 Wi-Fi 6(千兆字节+)和 LTE 解决方案。

最初将有两款 Lakefield 处理器，分别是酷睿 i5-L16G7 和酷睿 i3-L13G4。两者的区别可以从下表中看出。i5 有更多的图形执行单元(eu):64 对 48。grahics 的最高频率上限为 0.5GHz(远低于 Amber Lake 的 1.05GHz)，这表明英特尔正在广泛而缓慢地提高性能，同时控制功耗要求。两者在 7W 时具有相同的 TDP。i5 的基频为 1.4GHz，而 i3 的基频只有区区 0.8GHz。i5 和 i3 的最高单核睿频(仅适用于 Sunny Cove core)分别为 3.0GHz 和 2.8GHz，而最高全核睿频分别为 1.8GHz 和 1.3GHz。据推测，英特尔正在依靠 Sunny Cove 比 Skylake 增加的 IPC 来抵消这些低时钟速度。请记住，只有一个“大”内核(相对而言)，所以不要指望这些超移动芯片能与 Ice Lake、Comet Lake 和 Tiger Lake 平台中的常规 U 系列芯片竞争。内存支持是 LPDDR4X-4267，顺带高于冰湖。

| **处理器号** | **图形** | **内核/线程** | **图形(EUs)** | **缓存** | **TDP** | **基本频率(GHz)** | **最大单核睿频(GHz)** | **最大全核睿频(GHz)** | **显卡最大频率(GHz)** | **记忆** |
| i5-L16G7 | 英特尔 UHD 显卡 | 5/5 | 64 | 4MB | 7W | 1.4 | 3.0 | 1.8 | 高达 0.5 | LPDDR4X-4267 |
| i3-L13G4 | 英特尔 UHD 显卡 | 5/5 | 48 | 4MB | 7W | 0.8 | 2.8 | 1.3 | 高达 0.5 | LPDDR4X-4267 |

AnandTech 能够提供更多关于莱克菲尔德芯片的细节。据称，英特尔告诉该出版物，Lakefield 芯片将使用 Tremont 内核进行几乎所有事情，并且只调用 Sunny Cove 内核进行用户体验类型的交互，如打字或与屏幕交互。这与英特尔在新闻稿中的说法不同。Foveros 技术意味着芯片的逻辑区域，如内核和图形，被放置在 10+纳米的芯片上(Ice Lake 制造的同一工艺节点)，而芯片的 IO 部分则在 22 纳米的硅芯片上(Ivy Bridge 和 Haswell 制造的同一工艺节点，在五年多前)，它们被堆叠在一起。内核之间的连接如何工作？英特尔在两个不同的硅片之间实现了 50 微米的连接焊盘，并通过注重功耗的 tsv(硅通孔)为顶层的内核供电。

总的来说，莱克菲尔德平台似乎很有前途。英特尔低功耗芯片的最大缺陷是，到目前为止，它们的价格都太贵了。这似乎不会随着 Lakefield 而改变，但至少消费者会期待新型的个人电脑，如前面提到的由 Lakefield 驱动的前三种设备。至少目前，由于应用支持的压倒性优势，英特尔仍然在 PC 领域占据主导地位，Lakefield 等宣布意味着 ARM 和高通将需要不断迭代，以克服英特尔固有的指令集优势。

* * *

**来源:[英特尔](https://newsroom.intel.com/news/intel-hybrid-processors-uncompromised-pc-experiences-innovative-form-factors-foldables-dual-screens/#gs.7tmpin)，[安达信](https://www.anandtech.com/show/15841/intel-discloses-lakefield-cpus-specifications-64-execution-units-up-to-30-ghz-7-w)，**