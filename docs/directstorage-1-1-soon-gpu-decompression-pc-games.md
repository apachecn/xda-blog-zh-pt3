# DirectStorage 1.1 即将为 PC 游戏带来 GPU 解压

> 原文：<https://www.xda-developers.com/directstorage-1-1-soon-gpu-decompression-pc-games/>

微软宣布，DirectStorage 将在今年晚些时候通过 DirectStorage 1.1 进行首次重大更新，并将以 GPU 解压缩的形式带来一个重要的新功能。目标是通过将资产解压缩卸载到 GPU 而不是使用 CPU 来完成，从而进一步减少加载时间。

DirectStorage 首次出现在 Xbox 系列 X|S 游戏机上，但该 API [于今年早些时候向 PC 游戏开发商](https://www.xda-developers.com/directstorage-available-windows-games/)推出。然而，最初的版本并没有承诺所有的变化。微软首先关注存储堆栈的改进，减少从 NVMe 固态硬盘读取数据时的开销，并支持并行 I/O 请求，以便更多数据可以一次传输到 CPU 或 GPU。通过允许处理各种请求，快速 NVMe 驱动器可以利用其最大带宽，而不是让用户等待每个请求完成后再开始下一个请求。这些改变本身已经可以减少 40%的加载时间。

但是 GPU 解压缩也是一件大事。当你安装一个游戏时，诸如纹理等资源通常会被压缩以节省硬盘空间。然而，在加载和运行游戏时，这些资产自然需要即时解压缩才能使用，这通常由 CPU 处理，然后 CPU 将未压缩的资产发送到 GPU，以便可以在需要时访问它们。在过去，压缩格式大多是为 CPU 优化的，所以这是有意义的。但是，正如微软解释的那样，GPU 非常适合处理这样的解压缩任务，因此将这项工作卸载到 GPU 意味着资产解压缩速度更快。如果资产针对 GPU 解压缩进行了优化，您可以获得更高的速度。

在下面的例子中，微软展示了在适当优化的情况下，使用 GPU 解压缩，5.65GB 的资产加载速度提高了近三倍。您还可以看到，在这个过程中，CPU 的使用率要低得多，因此它为其他任务节省了资源。

为了帮助实现这一点，微软与 Nvidia 合作创建了 GDeflate，这是一种针对 GPU 解压缩优化的新压缩格式，可以利用 DirectStorage 1.1。除了更快的速度之外，新格式应该可以帮助您节省磁盘空间，并且还可以节省互连带宽。虽然 Nvidia 贡献了这种格式，但任何 GPU 制造商都可以利用它，微软正在与英特尔和 AMD 合作，使他们的驱动程序也可以利用它。

当然，有一些硬件和软件要求完全使用 DirectStorage。Windows 10 和 11 都受支持，但后者对存储堆栈进行了某些优化，使其更加高效。你还需要一台配有 NVMe 固态硬盘的电脑，你的 GPU 需要支持 DirectX 12 和 Shader Model 6.0，尽管微软也建议支持 DirectX 12 Ultimate。此外，请记住，DirectStorage 1.11 是开发人员的工具，所以一旦它发布，你需要等待游戏实际使用它，所以它不会只是对每个现有游戏的神奇升级。微软表示，将在 2022 年底发布升级后的 API。

* * *

**来源:** [微软](https://devblogs.microsoft.com/directx/directstorage-1-1-coming-soon/)