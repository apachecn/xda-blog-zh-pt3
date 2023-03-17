# 如何在 Android 设备上使用 Rboard 应用程序创建和编辑 Gboard 的自定义主题

> 原文：<https://www.xda-developers.com/how-to-create-edit-gboard-custom-themes-rboard-apps/>

在永无止境的可定制的 Android 世界中，爱好者和修改者都在不断地努力使我们的设备更好地匹配我们的个性。我们喜欢调整我们能得到的任何东西，无论是新的壁纸，最热门的新图标包，还是完全定制的主题。这就是为什么许多用户喜欢 Gboard 作为他们的[键盘应用](https://www.xda-developers.com/best-android-keyboard/)的原因，因为你可以通过像 [Rboard 主题管理器](https://www.xda-developers.com/rboard-theme-manager-gboard-custom-themes-hidden-settings/)这样的项目使用自定义主题来修改股票 UI。

尽管谷歌为 Gboard 提供了太多现成的主题，但有一个完整的社区为键盘应用程序提供自制主题和其他 mod。然而，定制一个现有的主题包或者从头开始创建一个定制主题并不是一件简单的工作。为了填补这一空白，两位经验丰富的 Gboard 主题人——XDA 资深会员 [RKBD](https://forum.xda-developers.com/m/rkbd.7544065/) 和 XDA 会员[der typ 7214](https://forum.xda-developers.com/m/dertyp7214.7113548/)——开发了一对应用程序:Rboard 主题创建器和 Rboard 修补器。

*   Rboard 主题创建器允许你创建基本的 Gboard 主题。
*   使用 Rboard Patcher，您可以进一步编辑主题的不同方面。
*   定制的主题可以通过 Rboard 主题管理器来应用。
*   您需要 root 权限来安装主题。

**浏览本文:**

* * *

## Gboard 主题的内部结构

在 Gboard 主题场景中，themepack 可以通过它的。包”扩展。本质上，该文件是图像资产、样式表和元数据的集合——所有这些都以特殊的容器格式压缩。

由于大部分的主题组件都是未加密的，你也可以编写额外的补丁来动态修改主题的特定部分。补丁通常以 ZIP 文件的形式分发。

* * *

## 如何使用 Rboard 主题创建器创建一个 Gboard 主题

Rboard 主题创建器是一个轻量级的 Android 应用程序，允许任何人在他们的手机上创建一个基本的 Gboard 主题。你甚至不需要访问 PC 来编译 themepack，因为应用程序会为你处理一切。

为了设计自己的 Gboard 主题，请执行以下操作:

1.  从前面提到的谷歌 Play 商店链接安装应用程序。
2.  打开应用程序，找到用于颜色选择的旋转转盘。[](https://www.xda-developers.com/how-to-create-edit-gboard-custom-themes-rboard-apps/rboard-theme-creator/)
3.  接下来，选择配色方案(如**深色**或**莫奈**)和对应的 UI 组件(如 **AMOLED** 或**三原色**)。这款应用可以让你尝试各种可能的组合。
4.  现在调整颜色盘，直到你在预览部分得到你想要的主题用户界面。
5.  要保存您自定义创建的主题，点击左下角的共享图标，选择文件选择器，并在给它一个合适的名称和作者信息后保存它。

或者，您可以将新创建的主题直接传输到 Rboard Patcher(如果安装了的话)进行进一步的编辑。为此，点击**添加主题**按钮并按照向导进行操作。

对于阅读本文的任何应用程序开发人员来说，Rboard 主题创建器是完全开源的。你可以自由探索代码，提交新的补丁，或者自己编译应用程序。

**[Rboard 主题创建者 GitHub 资源库](https://github.com/DerTyp7214/RboardThemeCreator)**

值得注意的是，开发者还拥有一个网页版的应用程序，这对于在你的 PC/Mac 上设计 Gboard 主题来说非常方便。

* * *

## 如何使用 Rboard Patcher 修补 Gboard 主题

Rboard Patcher 是一款多功能的 Gboard 主题工具。首先，该应用程序允许您自定义基础主题包(*。pack)由 Rboard 主题创建器应用程序制作。此外，您还可以编辑现有的社区制作的主题，并使用公开托管的主题补丁修改它们的不同方面。该补丁程序还不支持第三方补丁回购，但该功能预计将很快登陆。

以下是如何通过 Rboard Patcher 定制任何 Rboard 兼容的主题:

1.  从前面提到的谷歌 Play 商店链接安装应用程序。
2.  打开 app，打开一个有效的 Gboard 主题*。使用文件选择器打包文件。
    *   例如，你可以将应用指向 Rboard Theme Creator 制作的 themepack。
3.  Rboard Patcher 将获取[公开托管的主题补丁](https://github.com/GboardThemes/Patches)并将它们分类列出。[](https://www.xda-developers.com/how-to-create-edit-gboard-custom-themes-rboard-apps/rboard-patcher/)
4.  点击您想要应用的选项(如字体或圆形图标)。
5.  要保存定制的主题，点击左下角的共享图标，选择文件选择器，并在给它一个合适的名称和作者信息后保存它。

如果你想通过 Rboard 主题管理器立即准备好定制的闪烁主题，你可以点击**添加到管理器**按钮并按照向导进行操作。当然，你需要事先在你的设备上安装 [Rboard 主题管理器应用](https://forum.xda-developers.com/t/4331445/)，否则这个选项将不起作用。此外，您需要 root 权限来安装主题。

Rboard Patcher 也是开源的，这意味着欢迎您修改代码库。如果你想在不自己编译应用程序的情况下尝试前沿版本，选择[持续集成版本](https://github.com/DerTyp7214/RboardPatcher/actions/workflows/ci.yml)。

**Rboard Patcher GitHub 资源库 **

* * *

## 结论

这就是全部了。如您所见，为 Gboard 创建定制主题并不难，尤其是当您可以利用 Rboard 社区提供的强大工具时。你用 Gboard 主题化得到多少粒度完全取决于你，但是如果你对 Google 的产品不满意，那么从头开始构建你想要的主题是最好的办法。

你是否经常用不同的 mod 定制你的键盘应用程序，或者你对这样的主题化不感兴趣？请在下面的评论区告诉我们。