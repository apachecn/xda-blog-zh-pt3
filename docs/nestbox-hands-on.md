# Nestbox 实践:在你的谷歌 Pixel 手机上运行真正的 Linux 虚拟机

> 原文：<https://www.xda-developers.com/nestbox-hands-on/>

如果你曾经想成为智能手机的超级用户，那么你可能会遇到 Termux 这样的产品。这是一个 Android 终端模拟器和 Linux 环境应用程序，一些人已经用它开发 Python 脚本，甚至从智能手机上运行《我的世界》服务器。现在，你可以更进一步，通过根像素 6 或常规像素 7，这要感谢 XDA 资深会员[的 Nestbox KD rag 0n](https://forum.xda-developers.com/m/kdrag0n.7291478/)，可在他的 [Patreon](https://www.patreon.com/kdrag0n) 上获得。

## 什么是 Nestbox？

Nestbox 是一款允许你在智能手机上创建容器和运行真实虚拟机的应用程序，它需要是最新的谷歌 Pixel 智能手机才能工作。这是因为 Nestbox 使用 pKVM(**p**protected**K**ernel-based**V**I virtual**M**achine)，这在 Android Common Kernel 的更新版本中可用，包括在 Google Pixel 6 系列和 Google Pixel 7 系列上。根据斯珀的 Mishaal Rahman 的说法，Pixel 6 系列需要 root 的原因是 pKVM 不是开箱即用的。

这里的大问题是它本质上是一个更强大的 Termux。对于大多数高级用户用例，Termux 已经可以让您实现大部分目标，但是通过虚拟化，您将能够在智能手机上运行 Docker 容器之类的东西。平心而论，这有点夸张，但有些人可能会用得上。您可以在 Nestbox 创建的容器中获得内核访问和 root 权限，这比使用 Termux 获得的权限要多。

## 安装和设置 Nestbox

如果你想在谷歌 Pixel 上使用 Nestbox，你需要[订阅 kdrag0n 的 Patreon](https://www.patreon.com/posts/74333551) 。我们使用了一台[谷歌 Pixel 7 Pro](https://www.xda-developers.com/google-pixel-7-pro-review/) 进行安装和测试，尽管步骤在 Pixel 6 系列上会略有不同。目前，Pixel 6 设备需要授予应用程序 root 访问权限，尽管 kdrag0n 表示这可能会在未来发生变化。

在 Pixel 7 上，你需要做的大部分配置与滴相似。您通过无线 adb 连接到自己的电话，配置最大容器大小，然后选择您的 Linux 发行版。它将下载、配置并执行虚拟机。

## 你能用 Nestbox 做什么？

至于你能做的事情，基本上是你能想到的都可以。这是一个 Linux 容器，尽管我发现我需要安装很多工具才能做任何事情。例如，我需要使用高级打包工具(Ubuntu 中的 apt)来安装 wget 和 curl，因为它是开箱即用的准系统。然后你可以添加任何你喜欢的东西。目前，还没有虚拟 GPU 支持，kdrag0n 说他也不打算支持它。

作为一个想法，你可以从你的手机托管一个网页或《我的世界》服务器。虽然两者目前都可以工作，但你实际上不能从容器外部访问它们。我和 kdrag0n 谈过，他确认目前没有合适的端口转发，也不可能在容器外部与这些实例进行交互。他告诉我，当他实现端口转发时，这种情况将会改变，他预计很快就会完成。

如果想试用 Nestbox，可以从 kdrag0n 的 Patreon 获得。由于网络限制，它目前非常有限，但是一旦这些限制解除，你将能够从它的外部连接到你的容器，并托管网页、游戏服务器等等。你会用 Nestbox 做什么？

*感谢 kdrag0n 与我们分享 Nestbox！*