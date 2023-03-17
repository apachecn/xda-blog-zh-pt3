# 2022 年你应该考虑启用的 10 个 Chrome 标志

> 原文：<https://www.xda-developers.com/chrome-flags-settings/>

谷歌 Chrome 是最受欢迎的浏览器之一，尤其是当你使用 Chromebook 的时候。Chrome 的稳定版本身非常出色，但对于高级用户来说，你可以添加许多调整来满足特定需求。

如果你喜欢测试新功能，不介意 bug，你可能已经通过你的 [Chromebook 的设置菜单](https://www.xda-developers.com/chrome-os-settings-guide/)加入了 ChromeOS Beta 或 ChromeOS Dev 频道。(你也可以在其他操作系统上使用 [Chrome Beta](https://www.google.com/chrome/beta/) 或 [Chrome Dev](https://www.google.com/chrome/dev/) 浏览器版本。)这些不同的版本给你一个完全不同的 Chrome 版本。但是如果你想测试一些实验性的功能，你会想看看 Chrome 的标志。如果你想了解 Chrome Flags，你来对地方了。

## 什么是 Chrome 标志？

Chrome 标志是谷歌目前正在 ChromeOS 或 Chrome 浏览器上测试的实验性功能，尽管有些标志是 ChromeOS 独有的，而其他标志则可以在不同操作系统的 Chrome 浏览器上使用。标志最终都会被移除，因为它们要么成为 Chrome 稳定版本的一部分，要么被 Chrome 开发者工具所吸收。启用标志后，您需要重新启动浏览器或计算机，以使更改生效。

如果你运行不同版本的 ChromeOS 或 Chrome 浏览器，你可以找到不同的标志。例如，Chrome Beta、Dev 和 Canary 频道将有不同的标志可供选择。如果你想访问最大数量的标志，Chrome Canary 可能是你最好的选择，尽管它是最不稳定的版本。

但是，使用标志有一些风险。并非所有标志都是稳定的，可能会导致浏览器或设备出现一些意外行为。基于浏览器的标志也没有经过在线安全协议测试，这意味着使用未经测试的 Chrome 标志进行在线金融交易可能存在风险。

## 如何启用 Chrome 标志？

好消息(但可能经常是危险的)是 Chrome 标志很容易定位和启用。事实上，启用标志的方法完全独立于您的操作系统。下面看一下如何启用标志。

1.  要找到可用的标志，打开你的 Chrome 浏览器，输入: **chrome://flags/**
2.  点击**进入**。这将把你带到 Chrome 的标志主页，在这里你可以滚动浏览(看起来无穷无尽的)标志列表进行选择。您可以使用下拉菜单轻松地浏览并选择启用或禁用标志，但这是非常令人难以接受的。
3.  如果你在寻找特定类型的旗帜，你也可以在 Mac 上使用 **Control+F** 或 **Command+F** 来搜索页面。
4.  如果你想启用一个特定的标志，只需输入: **chrome://flags/#tag。**这将直接带您到指定的标志。
    *   在此语法中，**#标签**应该替换为附加到您希望启用的标志的适当标签。每个 Chrome 标志都有一个标签。在上面的截图中，它就列在主页上旗帜描述的下面。

通常，要启用一个标志，必须关闭下拉菜单中的**默认**和**启用**。

## 识别启用标志和重置标志

关于 Chrome 标志的一个更烦人的事情是很难确定哪些标志是启用的。您应该可以在主标志页面的顶部看到大多数已启用的标志，但是没有简单的方法来确定一些标志的状态。如果您没有更改状态，它很可能被禁用，但是一些带有菜单的标志不会告诉您默认状态。

如果您启用的标志导致浏览器或设备出现问题，您可以将该标志重置为默认值或明确禁用它。如果您想禁用个别标志，请通过主页上的下拉菜单来实现。如果你想撤销对 Chrome 标志所做的所有更改，顶部还有一个按钮**重置所有**。

## 现在要启用的十大 Chrome 标志

现在你知道什么是 Chrome 标志了，你可能想尝试几个。这些是我们最喜欢的 Chrome 标志，让你开始你的改装之旅。我们在下面指出了 ChromeOS 的标志。

1.  chrome://flags/# side-search 这在谷歌 Chrome 的右侧增加了一个侧边栏，看起来很像微软 Edge 的侧边栏。有了它，你可以在你已经登录的网站上搜索谷歌上的东西，而不必打开一个新标签。
2.  **chrome://flags/# enable-reader-mode**这个给 Chrome 增加了一个阅读模式。它将消除网页上的许多混乱，使阅读新闻和其他内容更加容易。
3.  如果你想让网页加载得更快，请选择这个标志。这将导致 Chrome 在你的设备上使用更多的存储空间，但如果启用，Chrome 将缓存更多的网页，因此单击后退按钮可以减少加载时间。
4.  **chrome://flags/#平滑滚动**在网页中移动很多？这个标志使得滚动内容更加平滑。
5.  chrome://flags # enable-parallel-downloading 这个标志可以让你的系统更快的下载。它会将你正在下载的多个文件分成更小的部分，以便更快地完成。
6.  **chrome://flags # top-Chrome-touch-ui**有了这个标志，你就可以强制 Chrome 一直使用平板模式。
7.  **chrome://flags/# coming-sharing-features**这个标志让网页截图变得更加容易。它在地址栏的 Chrome share 菜单下添加了一个工具。
8.  **chrome://flags/# enable-force-dark**我们喜欢 XDA 的黑暗模式。这个标志可以在你所在的任何页面上启用它。
9.  **(仅限 ChromeOS)chrome://flags/# files-trash**启用时，此标志会在 Files 应用程序中添加一个垃圾桶文件夹。这有助于避免意外删除 Chromebook 上的重要文件。
10.  **(仅限 ChromeOS)**chrome://flags/# enable-cro-ime-system-e moji-picker****这将在 ChromeOS 中启用表情选择器。你可以通过右击任何你想插入表情符号的地方，或者使用**搜索+ Shift +空格**来召唤它。

如果您意外启用了导致问题的内容，请将每个标志还原为原始默认设置。Chrome 标志可以带来很多乐趣，并为 ChromeOS 和跨设备的 Chrome 浏览器增加一个额外的维度。也有许多其他方式来修改你的 Chrome 体验，包括 Android 应用、Linux 应用和 [Chrome 主题](https://www.xda-developers.com/best-google-chrome-themes/)。如果你使用了任何不在我们列表上的不能错过的 Chrome 标志或插件，请在评论中告诉我们。