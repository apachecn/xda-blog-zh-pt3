# 使用这些 unbrick 软件包将您的一加 9、9 Pro 和 9R 恢复到出厂固件

> 原文：<https://www.xda-developers.com/oneplus-9-9-pro-9r-unbrick-msmdownloadtool/>

在现实生活中，给你的 Android 设备砌砖经常感觉像是一场灾难。对于许多设备来说，在这种情况下，没有明确的方法或公开可用的工具可以帮助你。根、配件市场内核和定制 rom 通常会受到媒体的广泛关注，但是帮助用户修复硬件设备的工具也同样重要。令人欣慰的是，一加 9 系列的用户现在足够幸运，可以在我们的论坛上下载普通一加 9、一加 9 Pro 和一加 9R 的单独 unbrick 软件包。

通常被称为“MsmDownloadTool”，一加的低级闪存程序利用了底层高通 SoC 的**E**emergency**D**own**l**oad 模式(EDL)。你需要一台运行微软 Windows 7 或更新版本的电脑，因为 unbrick 软件包与 Linux 和 macOS 不兼容。Windows 虚拟机可能有效，但不推荐使用。

 <picture>![The vanilla OnePlus 9 is for those who want flagship performance but don't want to pay top dollar. It offers a 6.5 inch 120Hz AMOLED display, a triple-camera setup tuned by Hasselblad, and the Snapdragon 888 SoC.](img/d66608aa9e3d6d32dbda78614c3ddc62.png)</picture> 

OnePlus 9

##### 一加 9

香草一加 9 是为那些谁想要旗舰性能，但不想支付最高美元。它提供 6.5 英寸 120Hz AMOLED 显示屏，由哈苏调整的三摄像头设置，以及旗舰骁龙 888 SoC。

 <picture>![The OnePlus 9 Pro is a really fast 2021 flagship that still keeps up well today. ](img/e87b0190e6eaa03a7cf726cd74516288.png)</picture> 

OnePlus 9 Pro

##### 一加 9 专业版

凭借 6.7 英寸的大尺寸四高清有机发光二极管显示屏和智能 120Hz 刷新率，一加 9 Pro 可能拥有市场上最好的显示屏。与 Hasselblad 合作调整的相机可拍摄出出色的静态照片，并捕捉精彩的 4K 视频。

 <picture>![The OnePlus 9R marks the company's return to the affordable flagship space. It's a rehashed OnePlus 8T from last year, featuring Qualcomm's new Snapdragon 870 chip and an affordable price tag.](img/5cd19bbf4c274d1e2dcf9e65c9d90842.png)</picture> 

OnePlus 9R

##### 一加 9R

一加 9R 标志着一加重新进入平价旗舰领域。这款手机是去年一加 8T 的翻版，设计略有更新，采用了新的骁龙 870 芯片。遗憾的是，它目前仅限于印度市场。

unbrick 包的工作流程非常简单。只需确保您的一加 9/9 Pro/9R 已关闭，然后在将手机插回电脑时按住音量增大和音量减小按钮。此时，手机应该会启动到 EDL 模式，这可以通过在设备管理器下搜索新的“QDLOADER 9008”条目(或者“QHUSB_BULK”，如果驱动程序没有正确安装)来轻松验证。一旦连接，只需打开适合您的模型的工具，选择“用户类型”为“其他”，点击“目标”按钮验证设备变量，按“开始”，你就可以开始了。

比起把你的砖头设备运回一加或者送到维修店，使用 unbrick 工具是一个更好、更省时的选择。请记住，在复活过程中，您的手机将被完全清除，引导程序将被重新锁定。在这种情况下，这没什么大不了的，因为你可以轻松地再次解锁，但这值得注意。