# 以下是 FIDO 安全密钥如何保护您的 Apple ID 的安全

> 原文：<https://www.xda-developers.com/how-fido-security-keys-keep-apple-id-secure/>

iOS、[和 macOS](https://www.xda-developers.com/ios-16-3-macos-13-2/) 的最新更新带来了许多改进和其他变化，但最突出的是引入了对 Apple IDs 的 FIDO 认证安全密钥的支持。Apple 已经详细说明了这些密钥如何与您的 Apple ID 配合使用，以及您如何使用它们来保护您的帐户。

## 什么是安全密钥？FIDO 是什么？

安全密钥是用来代替密码的，它们为您的帐户增加了一层保护。如果您使用双因素身份验证，则需要使用两种不同类型的信息登录您的帐户。第一个是您的密码，第二个通常是类似验证码的东西。通过配对安全密钥，您将不再需要依赖发送到您授权的 Apple 设备或通过短信发送的传统双因素验证码。安全密钥不会被拦截或窃取，不像验证码会通过短信发给你。

FIDO (Fast ID Online)是一套旨在消除密码的认证协议，由 FIDO 联盟开发。苹果，微软和谷歌，在去年年中的承诺支持通过这些认证协议实现的无密码登录。 [iOS 16.3 beta 1](https://www.xda-developers.com/ios-16-3-beta-1/) 随后带来了对这些按键的第一级支持，以便用户可以试用。

## 安全密钥对我的 Apple ID 有什么作用？

安全密钥为您的帐户增加了一层额外的保护，在使用您的帐户设置安全密钥后，您将需要它来执行以下操作:

*   在新设备或网络上使用您的 Apple ID 登录
*   重置 Apple ID 密码或解锁 Apple ID
*   添加其他安全密钥或删除一个安全密钥

因为一旦你设置了安全密钥，它们对你的 Apple ID 是多么重要，所以你至少需要两个。这意味着如果你丢失了一个，你仍然可以访问你的帐户，也意味着你可以在一个安全的地方存储一个备用的以防万一。例如，如果你在旅行，你可以选择留一个在家里。

## 为您的 Apple ID 设置安全密钥

虽然苹果没有说，但用户报告表明，使用的 FIDO 协议是认证者协议 2 的客户端，或 CTAP2。您需要以下内容来设置 Apple ID 的安全密钥。

*   至少两个支持 CTAP2 的物理 FIDO 认证密钥。
*   **上的 iOS 16.3、iPadOS 16.3、macOS Ventura 13.2 所有登录到你的 Apple ID 的设备。**
*   为您的 Apple ID 设置的双因素鉴定。
*   现代网络浏览器。请注意，Firefox 的最新夜间版本 Firefox 109[不支持苹果使用的安全密钥标准](https://bugzilla.mozilla.org/show_bug.cgi?id=1530370)。
*   若要在配置安全密钥后登录 Apple Watch、Apple TV 或 HomePod，您需要支持安全密钥的 iPad 或 iPhone。

不过，如果你在 Apple ID 上设置了安全密钥，你需要注意一些限制。

*   你将无法登录 iCloud for Windows
*   您不能登录到不能更新到支持安全密钥的软件版本的旧设备
*   不支持子帐户和管理的 Apple IDs
*   不支持与家庭成员的 iPhone 配对的 Apple Watches。若要使用安全密钥，请先用您自己的 iPhone 设置您的手表。

## 为您的设备选择正确的安全密钥

根据您的主要设备，它会更改您可以用来登录 Apple ID 的设备。例如，iPhone 支持 NFC，因此支持 NFC 的按键也可以工作，但只能在 iPhone 上使用。您可以通过 Lightning to USB-C 适配器将 USB-C 安全密钥用于 iPad、Mac 或 iPhone。最后，USB-A 安全密钥将与旧 MAC 或 USB-C 到 USB-A 适配器一起工作。

Apple 建议使用以下安全密钥，作为与您的 Apple ID 配合使用的良好范例。

*   YubiKey 5C NFC(适用于大多数 Mac 和 iPhone 机型)
*   YubiKey 5Ci(适用于大多数 Mac 和 iPhone 机型)
*   谭飞 ePass K9 NFC USB-A(适用于较旧的 Mac 机型和大多数 iPhone 机型)

## 如何为您的 Apple ID 添加安全密钥

如果您设定为 Apple ID 添加安全密钥，您可以根据您拥有的设备执行以下操作。

### 在 iPhone 或 iPad 上

1.  打开**设置** app。
2.  轻点你的**名字**，然后轻点**密码&安全**。
3.  点击**添加安全密钥**，然后按照屏幕指示添加您的密钥。
4.  查看与您的 Apple ID 相关联的设备，然后选择:
    *   保持登录到所有活动设备。
    *   选择您不想继续访问您的帐户的设备，并注销它们。

### 在 Mac 上

1.  从苹果菜单中，选择**系统设置**，然后点击你的**名字**。
2.  点击**密码&安全**。
3.  在**安全密钥**旁边，点击**添加**，然后按照屏幕指示添加您的密钥。
4.  查看与您的 Apple ID 相关联的设备，然后选择:
    *   保持登录到所有设备。
    *   选择您不想继续访问您的帐户的设备，并注销它们。

如果您遇到任何问题，请务必查看苹果自己网站上链接的指南，以及设置安全密钥的指南！

* * *

**来源:[苹果](https://support.apple.com/en-us/HT213154)**