# Android 14 可能会为带有触摸板手势和修改键重新映射的键盘带来更好的支持

> 原文：<https://www.xda-developers.com/android-14-improved-keyboard-support/>

谷歌一直试图让 Android 在大屏幕设备上更好地工作，由于这些努力，我们现在有了任务栏、活动嵌入、更优化的应用程序、改进的信箱和更好的分屏支持，这只是其中的几个变化。Android 还为大屏幕设备添加了大量其他有用的功能，其中许多功能要么仍在开发中，要么正在进一步完善，例如中枢模式、桌面模式、手写笔手写和手掌拒绝支持。现在，Android 14 DP1 已经发布，我们可以为谷歌正在为大屏幕设备进行的改进添加更好的键盘支持。

虽然平板电脑作为媒体消费设备的效果最好，但也可以用来工作。然而，如果你没有无线连接或连接到平板电脑的键盘，做任何涉及大量打字的工作都会令人沮丧。幸运的是，Android 很早就支持使用外置物理键盘，很多平板电脑[甚至自带专门为其设计的键盘](https://www.xda-developers.com/oneplus-pad-release/)。

Android 支持 Linux 的输入设备接口，因此大多数键盘在连接时都能被识别，但该平台使用在[键布局文件](https://source.android.com/docs/core/interaction/input/key-layout-files)中定义的映射将 Linux 键码翻译成 Android 键码。但是，除非键盘使用唯一的产品 ID 来标识自己，并且操作系统具有对应于该 ID 的特定键布局文件，否则 Android 将使用[通用键布局](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/data/keyboards/Generic.kl?q=generic.kl&start=1)和[通用键字符映射图](https://cs.android.com/android/platform/superproject/+/master:frameworks/base/data/keyboards/Generic.kcm)来确定当用户按下键盘上的键时要发送什么 Android 键码。

这些通用键文件是通用的，所以它们可以支持广泛的(全字母美国英语 PC 风格外部)键盘。这适用于您遇到的大多数通用 QWERTY 键盘，但有时，您可能会发现自己的键盘布局与通用 QWERTY 略有不同，其中修饰键(如 Caps lock、Ctrl、Meta 和 Alt)的位置略有不同，但仍然执行相同的功能。如果是这样的话，那么如果你能重新映射这些键，那将会很有用。幸运的是，Android 14 正准备加入改变修饰键行为的支持！

在 Android 14 DP1 中，我在设置>语言和输入>物理键盘下发现了一个新的“修饰键”界面。通过此页面，您可以交换 Caps lock、Ctrl、Meta 和 Alt 键的行为。虽然这里没有给你重新映射每个键的选项，但是你可以重新映射修饰键。然而，在 Android 14 DP1 中，默认情况下“修饰键”页面是不可见的。我不得不翻转一个开发者标志，让它出现，表明该功能仍在开发中。尽管如此，一旦它登陆，用户将可以选择重新映射他们不喜欢的带有修饰键位置的键盘！

当我谈到按键的话题时，我还想指出，Android 14 中更新了通用键布局文件，以将更多的 Linux 键码映射到 Android 键码中。这些变化是:

*   键 120 从(未定义)到最近的应用程序
*   按键 228:键盘背光开关
*   按键 229:键盘 _ 背光 _ 向下
*   按键 230:键盘 _ 背光 _ 开启
*   按键 248:静音
*   按键 418:放大
*   按键 419:缩小
*   关键 528:聚焦

键盘背光输入在我看来特别值得注意，因为 android 还通过新的内部 API 增加了对控制连接键盘背光的支持:Android . hardware . input . keyboard backlightstate 和 com . Android . server . input . keyboard backlightcontroller。为了更好地处理非 QWERTY 键盘布局，Android 还增加了新的内部 API 来改变键盘布局，提供了 azerty、colemak、dvorak、extended、qwertz、turkish_f、turkish_q 和 workman 选项。我不知道在未来的 Android 14 版本中，我们是否会获得改变键盘布局的能力，但我相信这对一些人来说将是一个不错的生活质量改善。

没有鼠标或者触摸板的键盘有多大用处？当然，你可以使用触摸屏，但如果你在一个很小的距离或连接到外部显示器时工作呢？许多键盘配件都集成了触摸板，Android 已经支持触摸板很多年了，但是除了指向和点击，你不能在 Android 上做太多事情。然而，在 Android 14 中，你不仅可以获得触摸板的一些有用的生活质量功能，还可以获得新的触摸板手势。

启用开发者标志后，Android 14 DP1 会在设置>系统下显示新的“触摸板”选项。在这里，您可以切换是否必须点击才能点击，更改滚动方向(反向滚动)，或者切换是否点击触摸板的右下角可以显示更多选项。您还可以调整指针速度，以防默认值太低或太快。我也希望看到指针加速调整，但这可能会在未来的版本中出现，因为 InputManager 中有一些与指针加速相关的新的内部方法。

在页面底部，有一个按钮，上面写着“学习触摸板手势”点击它没有任何作用，因为可能包含学习如何使用触摸板手势的教程的活动还没有实现。然而，翻转第二个开发者标志并返回到这个相同的页面，将导致一个名为“触摸板手势”的新条目出现在顶部。在这里，您可以“自定义单独的触摸板导航手势”您可以选择:

*   用三个手指向左或向右滑动即可返回
*   用三个手指向上滑动即可回家
*   用三个手指向上滑动，然后按住来打开最近使用的应用程序
*   用三个手指向下滑动来打开通知
*   用四个手指向左或向右滑动来切换应用程序

任何想要使用带有键盘和触摸板的 Android 平板电脑工作的人都会发现这些操作很有用，尤其是在他们进行多任务处理的时候。虽然我肯定一些原始设备制造商已经在他们的 AOSP 中实现了这样的功能，但看到操作系统制造商自己将更好的键盘和触摸板支持融入 Android 仍然很好。

最后，我想强调另外两个变化。第一个你可能已经在之前的截图中注意到了，但是“语言和输入”页面被分成了“语言”和“键盘”。鉴于我们在 Android 14 中看到的对键盘支持的重新关注，这是有意义的。然而，这个重新设计，就像我提到的其他变化一样，在 Android 14 DP1 中默认是不启用的。第二个变化是一个新的启动器标志，名为 ENABLE _ SPLIT _ FROM _ full screen _ SHORTCUT，默认情况下是启用的，它允许你在应用程序全屏时使用键盘快捷键进入分屏模式。