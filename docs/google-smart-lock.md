# 什么是谷歌智能锁？它在 Android 和 Chromebooks 上如何工作？

> 原文：<https://www.xda-developers.com/google-smart-lock/>

智能锁是让你的安卓智能手机更容易使用的方法之一，它已经存在很久很久了。它允许你根据你定义的标准解锁你的手机或 [Chromebook](http://www.xda-developers.com/best-chromebooks/) ，无需 pin 码、模式或密码。谷歌有三种不同的智能锁产品:Android 智能锁、密码智能锁和 Chromebook 智能锁。因此，基本上，谷歌智能锁包含的功能可以让你快速解锁并开始使用设备或登录帐户，只需点击几下，避免了记住密码的需要。

## 安卓智能锁

Android 智能锁由三个列出的选项组成，您可以使用它们来保持设备解锁。

*   **体内检测:**这种方法需要你解锁一次你的设备，之后它会保持解锁状态，直到它认为它被放在桌子上或远离你的地方，或者直到四个小时过去了。
*   **可信设备:**如果您戴着健身腕带，或者可能有其他设备使用蓝牙连接到您的手机，此选项允许您选择这些设备作为可信实体。现在，当您的手机与这些设备配对时，不需要密码即可解锁。它将保持解锁状态，直到您从设备上断开连接，或者直到您的手机解锁四个小时，然后它将要求您再次登录。
*   **可信位置:**如名称所示，通过它，您可以将任何位置(最好是您的家)设置为您的设备可以保持解锁的位置。它将保持解锁状态，直到你离开该位置，或者直到你在该位置停留了四个小时，然后它将要求你再次登录。这需要精确的位置访问。

 <picture>![Google Smart Lock for Android on OnePlus 5](img/be5971ac1368f3dff08197f8bb5f9eae.png)</picture> 

Smart Lock for Android on OnePlus 5 running Android 10

您可以调出电源菜单，并在任何阶段点击“锁定”，以便随时强制锁定您的设备。

**请注意:**随着谷歌助手语音匹配和面部解锁功能在大多数安卓手机上可用，这些功能已经从智能锁中移除，只是旧款手机的一部分。

## Chromebooks 智能锁

与 Android 的智能锁类似，Chromebooks 的这一变体将允许你快速登录到你的系统，前提是你的手机使用相同的谷歌账户。要使用此功能，链接的智能手机必须解锁，打开蓝牙，并且需要配置一种屏幕锁定类型(PIN、模式或密码)。

一旦你的 Android 智能手机连接上，Chromebooks 的智能锁默认是打开的，但如果你对此感到不舒服，你可以通过以下方式关闭它:

1.  在 Chromebook 的右下角，选择时间。
2.  选择设置。
3.  在“连接的设备”下，选择您的 Android 手机。
4.  打开或关闭智能锁。

## 智能密码锁

此功能允许您通过在设备之间共享保存到您帐户的密码来快速登录各种应用程序。它的功能类似于苹果基于 iCloud 的钥匙链服务或任何其他的[密码管理器](https://www.xda-developers.com/best-free-password-manager/)。

**注:** [智能密码锁](https://developers.google.com/identity/smartlock-passwords/android/overview)现已弃用，鼓励开发者改用[一键登录](https://developers.google.com/identity/one-tap/android/get-started)。