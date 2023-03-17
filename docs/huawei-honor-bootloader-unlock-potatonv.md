# 采用麒麟片上系统的华为和 Honor 设备的 Bootloader 解锁方法

> 原文：<https://www.xda-developers.com/huawei-honor-bootloader-unlock-potatonv/>

早在 2018 年，当中国 OEM 厂商透露[不会为其设备](https://www.xda-developers.com/huawei-stop-providing-bootloader-unlock-codes/)提供任何官方 bootloader 解锁方法时，华为在发烧友社区引起了巨大的轩然大波。该政策对售后开发和改装场景是一个相当大的打击，因为缺乏对引导加载器解锁的官方支持将极大地限制华为设备的定制潜力。虽然[华为的前子品牌](https://www.xda-developers.com/honor-unveil-first-phone-independent-brand-later-this-week/)Honor 开始在[通过授权服务中心](https://www.xda-developers.com/honor-india-support-service-centers-unlock-bootloader/)在有限的试验中提供引导程序解锁代码，但只有一种可行的方法来解锁你的华为或 Honor 设备的引导程序:第三方付费服务。这些服务当然关心让他们的客户满意，但是有一件事阻碍了我们推荐他们，那就是无法审计他们的方法。进入 potato NV——一个用于选择华为/Honor 智能手机的开源 bootloader 解锁器。

击败华为严苛的安全措施并不是一件容易的事情，但一位名为 Andrey Smirnoff 的开发人员实际上成功破译了基于海思麒麟 960/659/655 芯片组的设备的引导加载器解锁代码生成算法。除此之外，让 PotatoNV 成为可能的是[XDA 资深会员](https://github.com/penn5/hisi-idt) [hackintosh5](https://forum.xda-developers.com/m/hackintosh5.8556932/) 发现的一种低级 bootloader flashing 方法。该工具利用 VCOM 下载模式，要求用户打开目标设备并访问主板上的测试点。

开发者[发布了](https://github.com/mashed-potatoes/PotatoNV/wiki/How-to-use-PotatoNV)非常详细的说明，关于移除设备的后盖，解锁引导程序，如果需要的话，安装正确的驱动程序。据他所说，PotatoNV 使用以下设备。即使您的手机或平板电脑不在列表中，也可以在该工具上尝试不同的引导程序选项，看看它是否能提供有效的解锁代码。

我们 XDA 开发人员总是欣赏开发人员所做的出色工作，他们中的大多数人从他们的生活中抽出宝贵的时间来为我们免费提供他们的劳动成果。随着 PotatoNV 的发布，上述华为和 Honor 设备的所有者终于能够闪存他们想要的所有定制 rom 和内核。

**[PotatoNV GitHub 库](https://github.com/mashed-potatoes/PotatoNV)**