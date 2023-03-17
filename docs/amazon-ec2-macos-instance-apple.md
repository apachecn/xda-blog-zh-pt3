# 亚马逊为苹果开发者在其云上推出 macOS 实例

> 原文：<https://www.xda-developers.com/amazon-ec2-macos-instance-apple/>

如果你是 Amazon Web Services (AWS) EC2 用户，这里有一个潜在的方便更新。该公司已宣布面向 macOS 的弹性计算云 Mac 实例的全面上市，允许苹果生态系统中的应用程序开发人员在云中运行按需 macOS 工作负载。此前，亚马逊只为 Windows 和 Linux 提供这项服务。

与典型的虚拟化实例不同，新的 EC2 macOS 实例构建在实际的 Mac Mini 机器之上，这无疑是一大优势。请注意，在 2021 年之前，你不会得到最新的苹果 M1 动力版本。目前，亚马逊正在使用上一代 Mac Mini，采用英特尔第八代 Coffee Lake Core i7-8700B 处理器，具有 6 个物理/12 个逻辑内核和 32 GB 内存。处理器的时钟频率通常为 3.2 GHz，但在睿频模式下会升至 4.6 GHz。开发者将可以在 macOS 10.14 Mojave 和 macOS 10.15 Catalina 之间进行选择，而 macOS 11.0 Big Sur 支持即将推出。

AWS 首席传道者杰夫·巴尔[将 Mac 实例描述为给苹果开发者的东西...能够快速&经济高效地为多个目标构建代码，而无需拥有&操作自己的硬件”。这里的前提很简单:考虑一个成熟的 macOS 开发平台，但是是在 AWS 上。您将受益于 EC2 提供的弹性、可伸缩性、安全性和可靠性。](https://aws.amazon.com/blogs/aws/new-use-mac-instances-to-build-test-macos-ios-ipados-tvos-and-watchos-apps/)

AWS 利用 Mac Mini 的高速雷电 3 端口将其与 Nitro 系统相连，以获得 10Gb/s VPC 网络带宽和 8Gb/s 存储带宽。这些实例可以通过带有图形界面的 VNC 访问，这意味着你可以在它们上面运行 Xcode 和 Swift 开发工具，并为 iPhone、iPad、Mac、Apple Watch、Apple TV 和 Safari 创建应用程序。命令行爱好者也可以使用 SSH 访问。

值得一提的是，EC2 Mac 实例的最小租用期为 24 小时，这意味着它们不能属于自动扩展组。macOS 实例现已在美国东部(N. Virginia)、美国东部(Ohio)、美国西部(Oregon)、欧洲(爱尔兰)和亚太地区(新加坡)推出，其他地区也将推出。

* * *

**来源:[亚马逊 AWS](https://aws.amazon.com/about-aws/whats-new/2020/11/announcing-amazon-ec2-mac-instances-for-macos/)**