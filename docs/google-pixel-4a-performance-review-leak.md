# 谷歌 Pixel 4a 性能评测测试手机的骁龙 730

> 原文：<https://www.xda-developers.com/google-pixel-4a-performance-review-leak/>

如果没有全球性的疫情需要担心，那么谷歌[将于本周在加州山景城举行](https://www.xda-developers.com/google-io-2020-canceled/)年度开发者大会 Google I/O。在去年的 I/O 大会上，谷歌发布了其首款中端像素设备 Pixel 3a 和 3a XL。今年，我们预计谷歌将推出一款名为 Pixel 4a 的中端智能手机。我们不知道这个 2020 年中端像素将于何时公布，但由于泄漏，我们知道了关于它的所有信息。在谷歌 Pixel 4a 发布之前，我们可以详细介绍这款手机的性能，这要归功于在预发布硬件上进行的基准测试。

迄今为止，Pixel 4a 最实质性的泄露来自古巴 YouTube[Julio Lusson](https://twitter.com/julio_lusson)，他运营着 [*TecnoLike Plus*](https://www.youtube.com/channel/UCSExLh16bM4dOYec9D6zx8g) 频道。上周，他分享了他从预发布的 Pixel 4a 中拍摄的多张照片，让我们提前了解了谷歌 2020 年中端 Pixel 的相机性能。今天，他在 YouTube 频道上发布了一段视频，展示了这款即将推出的智能手机在各种基准测试应用中的性能。在发布视频之前，他与我们分享了原始结果，允许我们将数据汇编和分析成下面的表格和图表。请注意，由于他在运行预发布软件的预发布硬件上执行了这些基准测试，如果 Google 进一步优化了性能，零售部门在基准测试中的表现可能会稍好一些。

**[谷歌 Pixel 4a 论坛](https://forum.xda-developers.com/pixel-4a)**

Julio 在下面的视频中展示了他在多个基准测试中运行 Pixel 4a，它甚至提供了一些在该设备上运行的游戏，如任天堂 GameCube 的*塞尔达传说:风觉醒*(通过 Dolphin Emulator)和 *PUBG Mobile* 。不过，视频是西班牙语的，所以如果你对我们收集的基准测试结果感兴趣，请继续阅读下面的内容。

## 测试设备-像素 4a、4、3 XL、3a XL 和最新的 QRD

谷歌 Pixel 4a 由高通骁龙 730 移动平台驱动，该平台由三星使用 8 纳米 LPP 工艺制造。骁龙 730 有一个八核 CPU，由两个集群组成:2 个基于 ARM Cortex-A76 的 CPU 内核，主频高达 2.2GHz，6 个基于 ARM Cortex-A55 的 CPU 内核，主频高达 1.8 GHz。GPU 是高通的 Adreno 618。

骁龙 730 不再是高通最好的中端处理器，因为皇冠被骁龙 765 摘走了，但 730 仍然比 Pixel 3a 和 3a XL 中的[骁龙 670](https://www.xda-developers.com/qualcomm-snapdragon-670-chipset/) 有了显著的提升。由于“性能”CPU 内核之间的架构差异，我们可以预期 CPU 性能会有明显的提升。我们还可以预计，Pixel 4a 中的骁龙 730 比 Pixel 3a 中的骁龙 670 更节能，因为它采用了更现代的制造工艺，尽管我们的基准测试不会反映这种改进。在现实世界的性能方面，谷歌 Pixel 4a 应该明显优于 Pixel 3a，因为它有更好的处理器、更好的 GPU、更高的内存容量和[更快的存储技术](https://www.xda-developers.com/google-pixel-4a-64gb-ufs-2-1-storage/)。

为了更好地衡量，我们还添加了谷歌 Pixel 4(由高通骁龙 855 驱动)、谷歌 Pixel 3 XL(由高通骁龙 845 驱动)和最新的高通参考设备(由高通骁龙 865 驱动)的基准测试结果。我们在去年 12 月[对骁龙 865](https://www.xda-developers.com/qualcomm-snapdragon-865-benchmarks-cpu-gpu-performance-vs-kirin-990-snapdragon-855-snapdragon-845/) 进行基准测试时收集了大部分基准测试结果。我们相当确定即将到来的[谷歌 Pixel 5 不会采用骁龙 865](https://www.xda-developers.com/google-pixel-2020-code-names-snapdragon-765-snapdragon-730/) ，但我们认为，看看谷歌 2020 年的中端 Pixel 和你能在任何安卓设备上找到的最好的硬件之间有多大的性能差距仍然是有趣的。Pixel 5 预计将采用骁龙 765，但我们还没有配备这种处理器的设备，因为在中国以外很少有配备这种平台的设备。

|  | 

高通参考装置(QRD)

 | 

谷歌像素 4

 | 

谷歌 Pixel 3 XL

 | 

谷歌像素 4a

 | 

谷歌 Pixel 3a XL

 |
| --- | --- | --- | --- | --- | --- |
| **设备名称** | 高通骁龙 865 | 高通骁龙 855 | 高通骁龙 845 | 高通骁龙 730 | 高通骁龙 670 |
| **软件** | 安卓 10 | 安卓 10 | 安卓 10 | 安卓 10 | 安卓 10 |
| **显示** | 2880x1440 @ 60Hz | 2280x1080 @ 60Hz | 2960x1440 @ 60Hz | 2340x1080 @ 60Hz | 2160x1080 @ 60Hz |
| **内存** | 12GB LPDDR5 | 6GB LPDDR4X | 4GB LPDDR4X | 6GB LPDDR4X | 4GB LPDDR4X |
| **存储** | 128GB UFS 3.0 | 64GB UFS 2.1 | 64GB UFS 2.1 | 64GB UFS 2.1 | 64GB eMMC 5.1 |

以下是高通骁龙 865、高通骁龙 855、高通骁龙 845、高通骁龙 730 和高通骁龙 670 的规格概述。

### 高通骁龙 730、865、855、845 和 670 规格

|  | 

高通骁龙 865

 | 

高通骁龙 855

 | 

高通骁龙 845

 | 

高通骁龙 730

 | 

高通骁龙 670

 |
| --- | --- | --- | --- | --- | --- |
| **CPU** | 1 个 Kryo 585“Prime”(基于 ARM Cortex-A77)，最高 2.84GHz

*   3 Kryo 585“性能”(基于 ARM Cortex-A77)，最高 2.4GHz
*   4 Kryo 385“效率”(基于 ARM Cortex-A55)，最高 1.8GHz
*   4 Kryo 385“效率”(基于 ARM Cortex-A55)，最高 1.8GHz

 | 1 个 Kryo 485“Prime”(基于 ARM Cortex-A76)，最高 2.84GHz

*   3 Kryo 485“性能”(基于 ARM Cortex-A76)，最高 2.42GHz
*   4 Kryo 385“效率”(基于 ARM Cortex-A55)，最高 1.8GHz
*   4 Kryo 385“效率”(基于 ARM Cortex-A55)，最高 1.8GHz

 | 4 Kryo 385“性能”(基于 ARM Cortex-A75)，最高 2.8GHz

*   4 Kryo 385“效率”(基于 ARM Cortex-A55)，最高 1.8GHz
*   4 Kryo 385“效率”(基于 ARM Cortex-A55)，最高 1.8GHz

 | 2 Kryo 470“高性能”(基于 ARM Cortex-A76)，最高 2.2GHz

*   6 Kryo 470“高效”(基于 ARM Cortex-A55)，最高 1.8GHz
*   6 Kryo 470“高效”(基于 ARM Cortex-A55)，最高 1.8GHz

 | 2 Kryo 360“高性能”(基于 ARM Cortex-A75)，最高 2.0GHz

*   6 Kryo 360“高效”(基于 ARM Cortex-A55)，最高 1.7GHz
*   **GPU**

 |
| 肾上腺素 650 | 肾上腺素 640 | 肾上腺素 630 | 肾上腺素 618 | 肾上腺素 615 | **记忆** |
| 4x 16 位、2133MHz LPDDR4X4x 16bit 位、2750MHz LPDDR5 | 4x 16 位 2133MHz LPDDR4X | 4x 16 位 1866MHz LPDDR4X | 2 个 16 位 1866MHz LPDDR4X | 2 个 16 位 1866MHz LPDDR4X | **制造工艺** |
| 7 纳米(TSMC N7P) | 7 纳米(TSMC) | 10 纳米 LPP(三星) | 8 纳米 LPP(三星) | 10 纳米 LPP(三星) | 10 纳米 LPP(三星) |

每个基准的快速概述

## *输入来自[马里奥·塞拉费罗](http://www.xda-developers.com/author/mario-serrafero/)*

*输入来自[马里奥·塞拉费罗](http://www.xda-developers.com/author/mario-serrafero/)*

*   **AndroBench:** AndroBench 是一个相当老的基准测试，其设计也同样过时，但它仍然是存储测试的首选。它测试顺序读/写、随机读/写以及 SQLite 插入、更新和删除操作的速度。顺序读/写是涉及读/写连续的存储块的操作，而随机读/写涉及读/写随机分散的存储块。SQLite 描述了一种数据库管理系统；处理大型数据库的开发人员经常需要进行 SQLite 调用来检索或修改数据库。我们可以通过 AndroBench 很好地了解 Android 设备的存储性能。默认情况下，基准测试写入一个 64MP 文件，对于顺序和随机读/写分别使用 32MB 或 4KB 的缓冲区大小，SQLite 事务大小为 1。前者的速度以 MB/s 为单位，而后者以每秒查询数(QPS)为单位。
    *   **安图图**:这是一个整体基准。AnTuTu 测试 CPU、GPU 和内存性能，同时包括抽象测试和最近的相关用户体验模拟(例如，涉及滚动 ListView 的子测试)。最终得分根据设计者的考虑进行加权。
    *   **GeekBench** :一项以 CPU 为中心的测试，使用了多种计算工作负载，包括加密、压缩(文本和图像)、渲染、物理模拟、计算机视觉、光线跟踪、语音识别和对图像的卷积神经网络推理。分数细分给出了具体的指标。最终分数根据设计者的考虑进行加权，重点是整数性能(65%)，然后是浮点性能(30%)，最后是加密(5%)。
    *   **GFXBench** :旨在使用最新的 API 模拟视频游戏图形渲染。大量的屏幕效果和高质量的纹理。较新的测试使用 Vulkan，而遗留测试使用 OpenGL ES 3.1。输出是测试期间的帧数和每秒帧数(本质上是另一个数除以测试长度)，而不是加权分数。**阿兹特克废墟**:这些测试是 GFXBench 提供的计算量最大的测试。目前，顶级移动芯片组无法支持每秒 30 帧。具体来说，该测试提供了非常高的多边形计数几何图形、硬件镶嵌、高分辨率纹理、全局照明和大量阴影贴图、丰富的粒子效果，以及 bloom 和景深效果。这些技术中的大多数将强调处理器的着色器计算能力。
    *   **PCMark 2.0** :将设备作为一个完整的单元进行测试。它模拟可以实现抽象算法和大量算术的日常用例；不同之处在于，它们是在一个应用程序环境中被分派的，具有特定的实际用途，并由多个应用程序通用的 API 调用和 Android 库来处理。该测试将输出对应于各种子测试的各种分数，这将在下面详细描述；Work 2.0 的综合分数是所有这些分数的几何平均值，这意味着所有测试的权重相等。

        ### PCMark 2.0 Subscore 解说。单击以展开。

        *   *网页浏览 2.0* 模拟浏览社交媒体:渲染网页，搜索内容，随着新图片的添加重新渲染页面，等等。该子测试使用原生 Android WebView 来呈现(WebKit)内容并与之交互，内容存储在本地-这意味着您可以离线运行它，但它不能完全模拟网页浏览，因为它排除了互联网连接因素(延迟、网络速度)。它专门跟踪七个任务的**帧速率和完成时间**，它们的分数是几何平均值的倍数。
        *   *视频编辑*模拟视频编辑性能:使用 OpenGL ES 2.0 片段着色器将效果应用于视频，解码视频帧(发送到 Android GLSurfaceView)，并以高达 4K 的几种帧速率和分辨率在 H.264/MPEG-4AVC 中渲染/编码视频。它专门跟踪 UI 上的**帧速率**，除了跟踪视频编辑流水线的**完成时间**的最终测试。
        *   *编写*模拟一般的文档和文本编辑工作:在文档内添加或编辑文本和图像，复制和粘贴文本，等等。它使用原生 Android EditText 视图以及 PdfRenderer 和 PdfDocument APIs。它将打开压缩文档，移动文本正文，在文档中插入图像，然后将它们保存为 PDF，然后对它们进行加密和解密(AES)。它专门跟踪打开和保存文件、添加图像和移动文本正文、加密/解密文件以及在 ImageViews 上呈现 PDF 页面等过程的任务完成时间。
        *   *照片编辑*模拟照片编辑性能:打开图像，通过滤镜应用不同的效果(颗粒、模糊、浮雕、锐化等)并保存图像。它使用 4MP JPEG 源图像，并使用 android.media.effect API、android.renderscript API 的 renderscript 内部函数、android-jhlabs 和原生 android.graphics API 以位图格式操纵它们，以便在屏幕上绘制过程。这是一个非常全面的测试，因为它会受到存储访问、CPU 性能、GPU 性能的影响，并且依赖于许多不同的 Android APIs。该测试专门测量**内存和存储访问时间、编码和解码时间、任务完成时间**。各种滤镜和效果来自不同的 API。
        *   *数据操作*模拟数据库管理操作:解析和验证来自文件的数据，与图表交互，等等。它将打开 CSV、XML、JSON 文件中的(日期、值)元组，然后用 MPAndroidChart 库呈现动画图表。它专门跟踪每个图表动画的**数据解析时间**以及**每秒绘制**(类似于帧速率，但具体到更新图表)。

    *   PCMark 2.0 子分数解释。单击以展开。

基准测试结果

## AnTuTu 并不是我的首选基准，尤其是在 Play Store 下架之后[，但不可否认的是，它是 Android 设备最受欢迎的基准之一。在该测试中，像素 4a 的总得分约为高通参考器件的 48%,约为像素 4 的 70%,但它与像素 3 XL 一样好，并且明显优于像素 3a XL。当我们查看 AnTuTu 的子分数时，我们可以看到 Pixel 4a 在 CPU、内存和 UX 测试中得分相当高，但在 GPU 测试中明显落后于我们测试的所有骁龙 8 系列处理器。事实上，在 AnTuTu 的大多数测试中，Pixel 4a 的表现都优于 Pixel 3 XL，除了 GPU 测试，Pixel 4a 的表现比 Pixel 3 XL 好 50%到 60%。在 AnTuTu 的内存测试中，Pixel 4a 的性能与 Pixel 4 和 Pixel 3 XL 相当，不过这并不奇怪，因为所有这些设备都有类似的内存配置。Pixel 4a 在 AnTuTu 的总体 UX 分数也与 Pixel 4 相当，但比 Pixel 3 XL 和 Pixel 3a XL 的分数高出约 35-36%。然而，在所有这些设备中，Pixel 4 仍将提供最佳的真实用户界面性能，因为我们不能忽视它是唯一一款具有 90Hz 刷新率面板的 Pixel 设备。总的来说，Pixel 4a 在 AnTuTu 的几乎所有测试中都优于 Pixel 3a XL，而不出所料，它在所有测试中都不如 QRD。](https://www.xda-developers.com/antutu-benchmark-removed-google-play-store/)

PCMark 是我最喜欢的基准之一，因为它强调真实世界的性能。虽然像素 4a 和像素 3a-x1 之间的得分差距很大，但前者与像素 4 或像素 3-x1 之间的得分差距要小得多。可以预见的是，QRD 因为其全面的硬件优势而将竞争对手打得落花流水，所以它甚至不值得分析它的子分数。Pixel 4a 在 PCMark 的 Writing 2.0 和 Photo Editing 2.0 测试中的得分远高于 Pixel 3a XL(分别为 44%和 56%)，这对于希望在设备上执行基本文档和图像编辑任务的用户来说是个好消息。

Julio 只能与我们分享 GFXBench 的一个结果，但它清楚地证明了我之前谈到的 GPU 性能:骁龙 730 中的 Adreno 618 远远优于高通骁龙 8 系列中的 Adreno GPUs。GFXBench 的 Aztec 废墟测试是 Kishonti 迄今为止计算最密集的图形测试，但它并不代表大多数 Android 游戏，所以不要让这些结果阻止你尝试在 Google Pixel 4a 上玩游戏。我敢打赌，只要你愿意调低一些图形设置，大多数游戏在这款设备上都能正常运行，即使是众所周知的性能密集型游戏，比如堡垒之夜移动。不管怎样，Julio 告诉我，他在游戏的“高”图形预设下玩了一轮 *PUBG Mobile* 就很好。

如果你喜欢通过模拟器玩复古游戏，那么你会对谷歌 Pixel 4a 的 CPU 性能非常满意。虽然 Pixel 4a 的多核 Geekbench 5.0 分数明显低于 Pixel 4 和 Pixel 3 XL(再次强调，QRD 遥遥领先，甚至不值得讨论)，但 Pixel 4a 的单核分数更接近 Pixel 4 和 Pixel 3a XL 的分数。在单核得分比较中，Pixel 4a 实际上优于 Pixel 3 XL，这可能归因于骁龙 730 的性能集群由 2 个基于 ARM Cortex-A76 的 CPU 内核组成，而骁龙 845 的旧款基于 ARM Cortex-A75 的 CPU 内核。当查看 Geekbench 5.0 的多核分数时，我们可以看到，在加密计算方面，Pixel 4a 的骁龙 730 大多不如 Pixel 4 的骁龙 855 和 Pixel 3 XL 的骁龙 845。

下表总结了这些条形图中的总体基准分数。为了防止这个表格变得太大，我们没有包括每个测试的子分数——如果你有兴趣看到这些结果，请随时联系我。

基准

| 

版本

 | 

QRD -骁龙 865

 | 

谷歌像素 4 -骁龙 855

 | 

谷歌像素 3 XL -骁龙 845

 | 

谷歌像素 4a -骁龙 730

 | 

谷歌像素 3a XL -骁龙 670

 | 

安图图

 |
| --- | --- | --- | --- | --- | --- | --- |
| 8.0.4 & 8.3.2 | 565,384 | 386,499 | 278,647 | 268,973 | 192,779 | Geekbench 单核 |
| 5.0.2 | 929 | 600 | 521 | 548 | 338 | Geekbench 多核 |
| 5.0.2 | 3,450 | 2,499 | 2,125 | 1,628 | 1,226 | GFXBench 1440p 阿兹特克废墟 OpenGL(高层)离屏 IFH |
| 5.00 | 20 | 16 | 14 | 6 | 4.5 | PCMark - Work 2.0 |
| 2.0.3716 | 12,626 | 9,311 | 8,988 | 8,687 | 6,881 | Androbench 顺序读取(MB/s) |
| 5.0.1 | 1,459 | 873 | 659 | 509 | 301 | Androbench 顺序写入(MB/s) |
| 5.0.1 | 225 | 189 | 231 | 188 | 237 | 随机读取(IOPS) |
| 5.0.1 | 50,378 | 37,600 | 32,376 | 33,422 | 16,226 | Androbench 随机写入(IOPS) |
| 5.0.1 | 48,410 | 41,340 | 37,417 | 39,053 | 25,522 | Androbench 随机读取(MB/s) |
| 5.0.1 | 195 | 147 | 126 | 131 | 63 | Androbench 随机写入(MB/s) |
| 5.0.1 | 189 | 161 | 146 | 153 | 100 | Androbench SQLite 插件 |
| 5.0.1 | 3,705 | 3,207 | 2,627 | 1,914 | 1,712 | Androbench SQLite 更新 |
| 5.0.1 | 4,014 | 3,996 | 3,333 | 2,458 | 2,080 | Androbench SQLite 删除 |
| 5.0.1 | 5,037 | 4,558 | 4,081 | 2,826 | 2,471 | 结论——谷歌 Pixel 4a 是一款性能稳定的中端智能手机 |

谷歌 Pixel 4a 正在成为一款出色的中端智能手机。如果传言的 399 美元起价是正确的，这将使 Pixel 4a 成为苹果 iPhone SE (2020 年)和三星 Galaxy A51 的直接竞争对手。虽然谷歌可能没有在这款设备中安装最好的硬件，但我们可以肯定的是，这款手机[将能够拍摄出色的照片](https://www.xda-developers.com/google-pixel-4a-camera-review-leak/)。谷歌的软件也将是其他中端产品的巨大优势。虽然一些公司基本上是在[的驱使下承诺只提供 2 年的 Android 更新](https://www.xda-developers.com/motorola-edge-plus-android-12-android-11/)，但谷歌为所有 Pixel 设备提供 3 年的更新。更重要的是，Pixel 4a 将采用已经宣布的大多数 Pixel 软件功能，包括现在播放、直播字幕和新的谷歌助手(Julio 向我们确认支持)。剩下的就是谷歌已经宣布了这款手机，但是我们[可能要等到 6 月 3 日](https://www.xda-developers.com/google-pixel-4a-delayed-june-android-11-beta/)才能实现。

## 结论——谷歌 Pixel 4a 是一款性能稳定的中端智能手机

**[谷歌 Pixel 4a 论坛](https://forum.xda-developers.com/pixel-4a)**

**传闻中的谷歌 Pixel 4a 规格**

处理器:高通骁龙 730

## GPU: Adreno 618

*   内存:6GB LPDDR4X
*   内部存储:64GB UFS 2.1
*   显示屏:单孔 5.81 英寸显示屏，2，340 x 1，080 分辨率，443 dpi，60Hz 刷新率
*   后置摄像头:12.2 MP 索尼 IMX363，f/1.73 光圈，1.4 m 像素，OIS，EIS，LED 闪光灯，4K 视频录制，自动对焦
*   前置摄像头:800 万像素索尼 IMX355，f/2.0 光圈，1.14 m 像素，EIS，定焦
*   连接:4G、双卡、GPS、WiFi 5、蓝牙、GLONASS、NFC
*   端口:USB Type-C、3.5 毫米耳机插孔
*   安全性:后置指纹传感器
*   电池:3080 毫安时
*   软件:安卓 10
*   电池:3080 毫安时
*   软件:安卓 10