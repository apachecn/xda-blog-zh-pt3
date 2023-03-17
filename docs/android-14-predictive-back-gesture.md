# Android 14 的预测性后退手势可以让你在向后滑动时预览你要去的地方

> 原文：<https://www.xda-developers.com/android-14-predictive-back-gesture/>

[Android 14](https://www.xda-developers.com/android-14/) 正在大幅度升级背部手势。以下是新的预测性背部手势的工作原理和外观。

当你在任何安卓应用中滑动返回时，下一个屏幕会出现在哪里并不总是很明显。如果您接下来看到的屏幕是您期望看到的，那么就没有问题。如果你无意中通过向后滑动退出应用程序，你可能会在做某事时失去你的位置或进度，尽管由于 Android 12 中的[变化，这种情况现在不太可能发生。无论如何，意外退出应用程序会扰乱开发者收集的指标，以更好地了解他们的用户，这就是为什么谷歌一直在研究一种新的](https://developer.android.com/about/versions/12/behavior-changes-all#back-press)[预测背部手势](https://www.xda-developers.com/android-13-beta-2-released/)模型，为用户提供关于背部手势将带他们去哪里的视觉提示。

当你浏览应用程序时，Android 会记录你所经过的目的地，称为 back stack。这是为了在您刷卡返回时，系统会将您带到正确的目的地。然而，在 Android 13 之前，系统无法确切知道后退手势会把用户带到哪里。这是因为应用程序可以[实现它们自己的后台行为](https://developer.android.com/guide/navigation/navigation-custom-back)并创建它们自己的后台堆栈，而系统不会意识到。由于系统本身不确定当你滑动返回时会发生什么，它也不能通知你会发生什么。

然而，从 Android 13 开始，应用程序可以提前告诉系统它们是否处理 back 事件。这种新的提前模型让系统知道后退手势应该导航到应用程序后退堆栈中的上一个任务还是返回到主屏幕。知道去哪里使得系统可以播放过渡动画，该动画充当用户的视觉提示，告诉他们当他们滑动返回时会发生什么。

然而，预测性背部手势模型在 Android 13 中仅部分实现。谷歌增加了一个新的“回到主页”过渡动画，当系统知道后退手势会让用户回到主屏幕时，就会播放出来，但他们无法为用户导航到应用程序的后退堆栈时添加动画。换句话说，Android 13 中的预测性后退手势只能告诉用户后退手势是否会退出应用程序回到主屏幕，而不是其他任何地方。

然而，从 Android 14 开始，预测性后退手势可以显示上一个任务的预览，当用户滑动返回时，它会从后退堆栈中弹出。这意味着你将能够判断后退手势是否会带你回到主屏幕，回到应用程序中的上一页，或者完全回到另一个应用程序，因此当你执行后退手势时，不会有任何模糊不清的事情发生。下面是这种新行为的演示:

如果你在你的 Pixel 设备上安装了 Android 14 DP1，你还不会看到这个新行为。这是因为新的过渡动画在 DP1 中默认是禁用的，所以我必须翻转一个开发者标志来启用它。我还不得不[在开发者选项中启用预测性背部动画设置](https://developer.android.com/guide/navigation/predictive-back-gesture#dev-option)，我还不得不使用一个应用程序，该应用程序[选择](https://developer.android.com/guide/navigation/predictive-back-gesture#opt-predictive)新的预测性背部手势行为。

针对 API 级别 34 的应用程序将默认启用新的预测性后退行为，因此我希望“预测性后退动画”设置将默认启用，并最终在未来的版本中从开发者选项中删除。我认为你不用等太久就会在应用程序中看到这种新行为，特别是因为谷歌警告开发者，如果他们不支持这一功能，他们的应用程序中的后退导航将被破坏。尚未添加对预测性后退手势支持的开发者应该仔细阅读谷歌文档中的[部分。](https://developer.android.com/guide/navigation/predictive-back-gesture)