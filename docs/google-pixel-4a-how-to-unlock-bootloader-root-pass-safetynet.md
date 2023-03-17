# 如何解锁 bootloader 并 root 谷歌 Pixel 4a

> 原文：<https://www.xda-developers.com/google-pixel-4a-how-to-unlock-bootloader-root-pass-safetynet/>

谷歌推出期待已久的谷歌 Pixel 4a 已经有几个星期了，该公司已经发布了这款智能手机的 Android 11 测试版。Pixel 4a 的工厂图像和内核源代码也已经在[发布](https://www.xda-developers.com/google-pixel-4a-android-11-beta-factory-image-kernel-source/)，这正是改装爱好者开始使用该设备所需的正确成分。如果你专门为了修补而购买这款手机，那么你会很高兴地知道 XDA 认可的开发商 [Zackptg5](https://forum.xda-developers.com/member.php?u=6037748) 已经成功地在谷歌 Pixel 4a 上实现了 root。开发人员还整理了一份精美的指南，利用 XDA 资深公认开发人员 [topjohnwu 的](https://forum.xda-developers.com/member.php?u=4470081) s [Magisk](https://forum.xda-developers.com/apps/magisk) 在解锁引导程序后对设备进行根操作。

**[谷歌 Pixel 4a XDA 论坛](https://forum.xda-developers.com/pixel-4a)**

**[从美国亚马逊购买谷歌 Pixel 4a](https://www.amazon.com/dp/B08DY51H2Y/?tag=xda-1qs1r9o-20&ascsubtag=UUxdaUeUpU29584&asc_refurl=https%3A%2F%2Fwww.xda-developers.com%2Fgoogle-pixel-4a-how-to-unlock-bootloader-root-pass-safetynet%2F&asc_campaign=Short-Term)| |[Pixel 4a 的最佳案例](https://www.xda-developers.com/best-google-pixel-4a-cases/)**

在我们进入如何找到像素 4a 的根之前，记得进行设备外备份。那是因为寻根过程**需要擦除手机上的所有数据，包括内部存储**上的文件。由于[安全网认证失败](https://www.xda-developers.com/safetynet-hardware-attestation-hide-root-magisk/)，你的银行应用程序以及 Pokémon Go 等热门游戏也可能在寻根后停止工作，但我们确实有一个临时的解决办法来解决这个问题。

* * *

## 如何 root 谷歌 Pixel 4a

### 步骤 1 -解锁引导加载程序

重要的是要注意，下面描述的步骤旨在用于像素 4a 的载体解锁变体。大多数美国运营商都不允许解锁引导程序，这样就无法锁定你的手机。

1.  进入“系统设置”->“关于手机”->“内部版本号”几次，直到启用“开发者选项”
2.  返回设置，进入系统->高级->开发选项->启用“OEM 解锁”
3.  如果你的手机插在任何东西上，拔掉插头并关机
4.  按住 Power + Vol Down 进入快速启动界面
5.  将手机插入 PC，打开终端/Shell/命令提示符/PowerShell(取决于操作系统)
6.  在终端上键入`fastboot flashing unlock`并按照设备上的提示解锁引导程序(注意**这一步将设备**复位)
7.  引导程序现在解锁了！

### 步骤 2–使用 Magisk Manager 修补股票启动映像

虽然您可以在我们的论坛上找到 Pixel 4a 的预补丁启动映像，但请确保验证其来源。您下载的任何预打补丁的启动映像都应该与安装的软件构建版本相匹配，否则您可能会面临严重的异常。我们总是建议您自己修补启动映像。

1.  [下载与安装版本的库存 ROM 相对应的出厂固件](https://developers.google.com/android/images?hl=en#sunfish),并从档案中提取引导镜像
2.  将 boot.img 复制到您的设备
3.  安装 Magisk 管理器(从项目的 GitHub repo 的[发布部分获取)](https://github.com/topjohnwu/Magisk/releases/download/manager-v7.5.1/MagiskManager-v7.5.1.apk)
4.  打开 Magisk 管理器->选择“安装”->“选择并修补文件”->选择 boot.img 文件
5.  修补后的启动映像应该可以在您的下载文件夹中找到

### 步骤 3–刷新补丁启动映像

1.  将 magisk_patched.img 复制到您的 pc
2.  将您的设备重新启动到快速启动模式(参见上面的解锁部分)
3.  在补丁引导 img 文件所在的目录下打开一个终端，输入`fastboot flash boot magisk_patched.img`
4.  你现在扎根了！

### (可选)步骤 4 -在您的 Google Pixel 4a 上传递安全网

绕过 SafetyNet 的硬件证明方法可能不是一件容易的事情，但是下面的解决方法应该可以暂时完成这项工作。

1.  从 Magisk 模块库中下载并安装 [MagiskHide Props Config](https://forum.xda-developers.com/apps/magisk/module-magiskhide-props-config-t3789228) 模块
2.  重新启动
3.  打开手机上的终端应用，输入“su -c props”
4.  选择“强制基本密钥证明”
5.  这将使您的设备在某些情况下看起来不同，默认情况下，这是 Nexus 5。 [Zackptg5](https://forum.xda-developers.com/member.php?u=6037748) 更喜欢它看起来像一个没有硬件认证的新设备(像谷歌 Pixel 3a)。所以选择:'从指纹列表中选择'- >'谷歌'- >'谷歌像素 3a '
6.  重启并验证你应该有希望通过安全网！

* * *

如果你想了解更多关于这个过程的细节，请查看我们论坛中的以下帖子:

**[指南:解锁/根/像素 4a 的安全网](https://forum.xda-developers.com/pixel-4a/how-to/guide-unlock-root-pixel-4a-t4153773)**

 <picture>![For the easiest and most convinent Pixel 4a purchase, go with Amazon! Pixel 4a orders come with Prime shipping, and if you have an Amazon Prime Rewards card, you can sign up for a monthly payment plan to boot.](img/7c058dee0fd7d0b006a64a3126925f29.png)</picture> 

Google Pixel 4a

##### 谷歌像素 4a

亚马逊很早就开始了预购，所以这款手机已经被延期订购了几周。你仍然可以试试你的运气，看看你是否能在遥远的未来买到一台并送货上门。亚马逊也有三种捆绑包可供选择。