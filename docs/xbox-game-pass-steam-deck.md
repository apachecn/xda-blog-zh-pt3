# 如何在 Steam Deck 上获得 Xbox 游戏通行证

> 原文：<https://www.xda-developers.com/xbox-game-pass-steam-deck/>

# 如何在 Steam Deck 上获得 Xbox 游戏通行证

按照以下步骤，在您闪亮的新掌上电脑上享受 Xbox Game Pass 游戏

所以，你终于拿到了[蒸汽甲板](https://www.xda-developers.com/steam-deck-review/)并准备好享受一些游戏。但你的 Steam 库非常简单，你不会想花数百美元购买你已经通过 Xbox Game Pass 订阅获得的游戏。虽然你可以在 Steam Deck 上安装 Windows 来访问你的 Xbox Game Pass 库，但这并不是在掌上游戏机上获得 Xbox Game Pass 的唯一方式。

使用一个简单的解决方法，包括在桌面模式下向 Steam 库添加一个 Microsoft Edge 快捷方式，您可以在 Steam 平台上获得 Xbox Game Pass。这个变通办法最棒的地方在于，它直接来自微软的编程团队，所以你不必担心不小心弄坏了你全新的主机。如果这听起来很吸引人，请按照以下步骤在 Steam 平台上访问 Xbox Game Pass 游戏。

## 在 Steam 库中创建一个 Microsoft Edge 快捷方式，以便在 Steam 平台上获得 Xbox Game Pass 游戏

在我们开始之前，使用 USB-C 集线器将外部键盘和鼠标连接到 Steam Deck。这不是必须的，但它会使这个过程变得简单一点。完成后，按照这些说明在 Steam 平台上获得 Xbox Game Pass。

1.  通过导航到电源设置菜单，启动 Steam Deck 并进入桌面模式。或者，您可以通过按住 Steam Deck 的电源按钮来进入桌面模式。
2.  选择显示屏底部的购物袋图标，打开发现软件中心。
3.  打开选项菜单，导航至*应用>互联网>网络浏览器。*
4.  在下一页选择 Microsoft Edge Beta，并选择下载选项下载并安装浏览器。
5.  安装微软 Edge Beta 后，导航到 Steam，在*添加游戏*窗口选择微软 Edge，选择*添加选定程序*按钮。
6.  现在回到桌面，从应用程序启动器打开 *Konsole* ，打开一个终端窗口。
7.  在 Konsole 中输入以下命令并按 enter:**flat pak-user override-file system =/run/udev:to com . Microsoft . edge**
8.  键入“Exit”并按回车键退出 Konsole。
9.  在桌面模式下回到 Steam，在 Steam 库中右击 Microsoft Edge，选择*属性*选项。
10.  从*属性*菜单中打开*启动选项*，用以下命令替换“e @@u @”之后的所有内容:**-window-size = 1024640-force-device-scale-factor = 1.25-device-scale-factor = 1.25-kiosk " https://www . Xbox . com/play "**
11.  (可选)通过右键单击 Steam 库中的 Microsoft Edge 并导航到*管理>控制器布局>浏览器配置*来更改控制器布局
12.  选择首选控制器布局，您就可以开始了。

这种解决方法实质上是在 Steam 库中添加了一个经过修改的 Microsoft Edge 快捷方式，让您可以在 Steam 平台上访问 Xbox Game Pass 游戏。切换回游戏模式，在 Steam 库中选择 Microsoft Edge，使用您的 Microsoft 帐户登录，享受您最喜爱的游戏。

我们建议您使用键盘和鼠标在 Steam 平台上玩 Xbox Game Pass 游戏，同时连接外部显示器。如果您没有兼容的坞站来创建这样的设置，请查看我们推荐的[蒸汽甲板坞站](https://www.xda-developers.com/best-steam-deck-docks/)来立即订购一个。