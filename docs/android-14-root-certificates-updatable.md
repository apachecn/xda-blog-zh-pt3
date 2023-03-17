# Android 14 使根证书可通过 Google Play 更新，以保护用户免受恶意 ca 的攻击

> 原文：<https://www.xda-developers.com/android-14-root-certificates-updatable/>

Android 有一个轻微的问题，它只会在每个蓝色的月亮上出现一次，但当它出现时，它会引起一些恐慌。幸运的是，谷歌在 Android 14 中有一个解决方案，将这个问题扼杀在萌芽状态。问题是 Android 系统的根证书库(root store)在 Android 存在的大部分时间里只能通过空中下载(OTA)更新。虽然原始设备制造商和运营商在更快、更频繁地推出更新方面做得更好，但事情仍有可能变得更好。这就是为什么谷歌设计了一个解决方案，让 Android 的根商店可以通过 Google Play 更新，从 [Android 14](https://www.xda-developers.com/android-14/) 开始。

当您每天上网时，您相信您设备的软件配置正确，可以将您指向托管您想要访问的网站的正确服务器。建立正确的连接很重要，这样你就不会被某个心怀不轨的人使用，但是安全地建立连接也很重要，这样你发送到该服务器的任何数据都会在传输过程中被加密(TLS ),希望不会被轻易窥探。但是，如果您的操作系统、web 浏览器和应用程序信任服务器的(TLS)安全证书，它们将只与互联网(HTTPS)上的服务器建立安全连接。

然而，由于互联网上有如此多的网站，操作系统、网络浏览器和应用程序不会维护它们信任的每个网站的安全证书列表。相反，他们会查看是谁签署了发给站点的安全证书:它是自签名的还是由他们信任的另一个实体(证书颁发机构[CA])签署的？这个验证链可以有几层，直到您到达一个根 CA，该根 CA 颁发了用于签署证书的安全证书，该证书最终签署了颁发给您正在访问的站点的证书。

根 CA 的数量比拥有由它们直接或通过一个或多个中间 CA 颁发的安全证书的网站的数量少得多，因此使得操作系统和 web 浏览器维护它们信任的根 CA 证书的列表是可行的。例如，Android 在/system/etc/security/cacerts 的只读系统分区中提供了一个可信根证书列表。如果应用程序没有[限制信任哪些证书](https://developer.android.com/training/articles/security-config#LimitingCas)，这种做法被称为证书锁定，那么在决定是否信任安全证书时，它们默认使用操作系统的根存储。由于“系统”分区是只读的，Android 的根存储在操作系统更新之外是不可变的，当 Google 想要删除或添加新的根证书时，这可能会造成问题。

有时，根证书[即将到期](https://blog.esper.io/android-14-updatable-certificates/#:~:text=Case%201%3A%20How%20Let%E2%80%99s%20Encrypt%20narrowly%20avoided%20disaster)，这可能导致网站和服务中断，web 浏览器抛出不安全连接的警告。在某些情况下，发布根证书的 CA 是被怀疑是恶意的[或受到损害的](https://blog.esper.io/android-14-updatable-certificates/#:~:text=Case%202%3A%20How%20TrustCor%20lost%20trust)。或者一个[新的根证书](https://letsencrypt.org/2020/09/17/new-root-and-intermediates.html)出现，它需要在 CA 可以真正开始签署证书之前将自己添加到每个主要操作系统的根存储中。Android 的根商店不需要经常更新，但它经常发生，以至于 Android 相对较慢的更新速度成为一个问题。

然而，从 Android 14 开始，Android 的根商店[可以通过 Google Play](https://blog.esper.io/android-14-updatable-certificates/) 更新。Android 14 现在有两个目录包含操作系统的根存储:前面提到的不可变的 OTA/system/etc/security/cacerts 位置和新的可更新的/apex/com。[Google]. Android . con crypt/security/cacerts 目录。后者包含在 Conscrypt 模块中，这是 Android 10 中引入的一个项目主线模块，提供 Android 的 TLS 实现。由于 Conscrypt 模块可以通过 Google Play 系统更新来更新，这意味着 Android 的根存储也将是如此。

除了使 Android 的根存储可更新之外，Android 14 还添加和删除了一些根证书，作为谷歌对系统根存储年度更新的一部分。

Android 14 新增的根证书包括:

1.  AC RAIZ FNMT-RCM 服务公司
2.  ANF 安全服务器根 CA
3.  CIF A62634068 专业认证公司授权
4.  当然支持 E1
5.  当然支持 R1
6.  Certum EC-384 CA
7.  Certum 受信任的根 CA
8.  D-TRUST BR 根 CA 1 2020
9.  D-TRUST EV 根 CA 1 2020
10.  DigiCert TLS ECC P384 Root G5
11.  DigiCert TLS RSA4096 Root G5
12.  全球信任 2020
13.  GlobalSign 根 E46
14.  GlobalSign Root R46
15.  HARICA TLS ECC 根 CA 2021
16.  HARICA TLS RSA 根 CA 2021
17.  HiPKI 根 CA - G1
18.  ISRG 根 X2
19.  安全通信 ECC RootCA1
20.  安全通信根 CA3
21.  Telia Root CA v2
22.  Tugra 全局根 CA ECC v3
23.  Tugra 全局根 CA RSA v3
24.  不信任根 CA
25.  vTrus ECC 根 CA
26.  vTrus 根 CA

Android 14 中移除的根证书包括:

1.  商会根- 2008
2.  网络信任全球根
3.  夏令时根 CA X3
4.  欧共体-ACC
5.  GeoTrust 主要认证机构- G2
6.  全球张伯伦根 2008
7.  全球标志
8.  希腊学术和研究机构 RootCA 2011
9.  网络解决方案证书颁发机构
10.  QuoVadis 根证书颁发机构
11.  Sonera Class2 CA
12.  荷兰国家公园
13.  荷兰根的状态 CA - G3
14.  TrustCor ECA-1
15.  TrustCor RootCert CA-1
16.  TrustCor RootCert CA-2
17.  Trustis FPS 根 CA
18.  VeriSign 通用根证书颁发机构

对于 TLS 证书更深入的解释，你应该在这里阅读我的同事 [Adam Conway 的文章](https://www.xda-developers.com/android-14-updatable-root-certificates/)。为了更彻底地分析 Android 14 的可更新根存储如何工作以及它为什么会出现，请查看[我之前写的关于这个主题的文章](https://blog.esper.io/android-14-updatable-certificates/)。