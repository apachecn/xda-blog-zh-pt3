# Jetpack 合成来到 Android TV，合成材料 3 达到稳定

> 原文：<https://www.xda-developers.com/jetpack-compose-material-3-android-tv/>

Jetpack Compose 是一个用 Kotlin 编写的声明式 UI 引擎，旨在取代或成为经典命令式 UI 引擎的可行替代方案，如 Android 的 XML 布局。本质上，Jetpack Compose 是一个强大的纯代码布局引擎，可以使 UI 实现更加容易。它于去年八月在 alpha 版本中首次发布，接着是今年二月在 beta 版本中的 T2 版本，并增加了更多内容。现在，在谷歌的 Android 开发者峰会上，该公司宣布 Compose 将进入 Android TV。更好的是，Material 3 现在处于稳定状态，这意味着您可以放心地使用它来构建您的应用程序。

合成材料 3 提供了[材料设计 3](http://m3.material.io/) 风格的组件和[主题](https://developer.android.com/jetpack/compose/themes/material#material3)，使材料你个性化的功能，如动态颜色。Compose Material 3 的库包含许多 UI 组件的新版本，如按钮、卡片、复选框、开关、导航栏、抽屉等，并正在支持其他组件。谷歌还发布了文档，向你展示如何将你的 Material Design 2 应用迁移到 Material Design 3。还有对不同 Android Studio 版本的改进，您可以使用它们在 Jetpack Compose 中构建，如下所述。

[Android Studio Dolphin](https://developer.android.com/studio/releases#new_in_compose) 是最新的稳定版本，具有:

*   动画协调
*   多重预览注释
*   布局检查器中的重组计数

[Android Studio Electric Eel](https://developer.android.com/studio/preview/features#2022.1.1)包含测试版功能，例如:

*   实时编辑(实验性)
*   合成渲染高亮显示
*   配置预览设备
*   预览中的实时更新

[Android Studio Flamingo](https://developer.android.com/studio/preview/features#2022.2.1) 包含金丝雀功能，例如:

*   默认情况下，实时编辑处于打开状态
*   改进的合成跟踪有助于您更好地检查性能问题。

不仅如此，谷歌还宣布，Compose 现已在 Android TV 的 Alpha 版本中推出。像 [Carousel](https://developer.android.com/reference/kotlin/androidx/tv/material/carousel/package-summary#Carousel(kotlin.Int,androidx.compose.ui.Modifier,androidx.tv.material.carousel.CarouselState,kotlin.Long,androidx.compose.animation.EnterTransition,androidx.compose.animation.ExitTransition,kotlin.Function1,kotlin.Function1)) 和 [ImmersiveList](https://developer.android.com/reference/kotlin/androidx/tv/material/immersivelist/package-summary#ImmersiveList(kotlin.Function3,androidx.compose.ui.Modifier,androidx.compose.ui.Alignment,kotlin.Function1)) 这样的组件已经实现，未来还会有更多。这是在今年夏天早些时候 Compose 达到 WearOS 的稳定状态之后。