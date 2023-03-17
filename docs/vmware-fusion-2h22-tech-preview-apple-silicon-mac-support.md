# VMware 的 Fusion Tech Preview 为 Apple silicon Macs 提供 Windows 11 支持

> 原文：<https://www.xda-developers.com/vmware-fusion-2h22-tech-preview-apple-silicon-mac-support/>

# VMware 的 Fusion Tech Preview 为 Apple silicon Macs 提供 Windows 11 支持

VMware 发布了 Fusion 的新公共技术预览版。Fusion 2H22 允许 Windows 11 在装有苹果芯片的 Mac 上运行。

VMware 希望您能以其最新版本 Fusion 的新技术预览的形式提供帮助。新版本为运行英特尔和苹果芯片的 MAC 电脑带来了 Windows 11 支持。Fusion 2H22 将允许用户通过虚拟化在 Mac 上运行 [Windows 11](https://www.xda-developers.com/windows-11/) 、Linux 等。

为了在 Windows 11 上实现虚拟化，WMware 必须创建一个虚拟可信平台模块(TPM)。由于该模块是 Windows 11 的一个要求，VMware 创建了一个带有快速加密的虚拟 TPM，这是一个自动生成的密钥，通过 Keychain 处理存储。速度对虚拟化很重要，因此新的 Fusion 提供了一种“快速加密”模式，只加密虚拟机最关键的部分。这种加密方法并不仅限于 Windows 11，而是可以用于 Fusion 支持的所有虚拟化。

Fusion 2H22 还支持带有 WDDM 驱动程序的 2D 图形，支持高达 4K 的分辨率。尽管当前版本中有图形和网络驱动程序，但 VMware 声明其 vmxnet3 网络驱动程序在当前版本中不可用。vmxnet3 网络驱动程序是一个自定义驱动程序，可提供高效的数据传输速率和更高的速度以及低延迟。如前所述，该软件不仅支持 Windows，还支持其他操作系统。目前，Linux 将使用 22.11 或更高版本的 Mesa 支持 OpenGL 4.3 + GLES 3.1 的 3D 图形。

为了简单起见，VMware 将只提供一个。dmg 文件，将与英特尔和苹果硅 MAC 兼容。如前所述，这仍然是一个技术预览，这意味着软件可能会有问题。还有一些已知的限制，比如只能支持 M1 设备上的 M1 虚拟机，如 [MacBook Pro 14 和 16](https://www.xda-developers.com/macbook-pro-2021/) 。这同样适用于仅运行在英特尔 Mac 系统上的英特尔虚拟机。如果这引起了你的兴趣，你可以从[这里](https://customerconnect.vmware.com/downloads/get-download?downloadGroup=FUS-PUBTP-22H2)下载这个文件。

* * *

**来源** : [VMware](https://blogs.vmware.com/teamfusion/2022/07/just-released-vmware-fusion-22h2-tech-preview.html)