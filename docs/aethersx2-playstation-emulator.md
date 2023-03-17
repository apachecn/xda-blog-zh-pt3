# AetherSX2 是在 Android 智能手机上玩 PlayStation 2 游戏的最佳方式

> 原文：<https://www.xda-developers.com/aethersx2-playstation-emulator/>

PlayStation 2 emulation 在 Android 上处于一个奇怪的位置已经很久很久了。虽然可以使用 Play Store 上的某种模拟器在智能手机上模拟该系统，但被盗代码和不道德商业行为的指控意味着，包括我们在内的许多人拒绝推广该应用，即使这是播放它们的最佳方式。现在，AetherSX2 是在 Android 智能手机上玩 PlayStation 2 游戏的最佳方式。它是免费的，速度很快，你现在可以从谷歌 Play 商店下载。你只需要一部顶级规格的智能手机。

我做了一些测试，看看哪些游戏有效，哪些无效，结果出奇的好。我在 [Android 12](https://www.xda-developers.com/android-12) 上的[一加 9](https://www.xda-developers.com/oneplus-9/) Pro 上进行了测试，这是在这篇评论发表时市场上[最强大的仿真设备](https://www.xda-developers.com/best-android-phones/)之一，根据游戏在哪里表现最好而在 Vulkan 和 OpenGL 之间切换。我测试了原版的*棘轮&叮当*、*极品飞车:地下 2* 、*辛普森一家:撞上&跑路*。我还想测试*音速英雄*，虽然它在之前的版本中运行得很完美，但在最近的版本中却出现了问题。

请注意，所有这些测试都是在模拟器的私有 alpha 版本上运行的，但是您可以看到性能有多好。从那时起，随着市场上功能更强大的智能手机的出现，情况才有所改善。如果你有一台带[骁龙 8 代 1](https://www.xda-developers.com/qualcomm-snapdragon-8-gen-1/) 甚至[骁龙 8 代 2](https://www.xda-developers.com/qualcomm-snapdragon-8-gen-2/) 的设备，你会得到比我们这里更好的结果。

## AetherSX2 是在手机上玩 PlayStation 2 游戏的最佳方式

PlayStation 2 模拟真的只有两种可供选择的模拟器。一个是玩！，一个是不需要 BIOS 运行的高级仿真器，另一个是违反 PCSX2 的许可协议。虽然 AetherSX2 使用 PCSX2 代码，但 PCSX2 的开发人员对 AetherSX2 大加赞赏，解释说，从本质上讲，其核心代码是 LGPLv3 授权的。

要运行 AetherSX2，你需要一个 64 位设备，芯片组必须有“大”性能核心(开发者建议至少是骁龙 845)。你可以使用 Vulkan 或 OpenGL 玩游戏，这取决于哪一个在你的设备上表现最好，并且你可以在游戏中在两者之间热插拔。AetherSX2 有很多很棒的特性，包括内部分辨率缩放、保存状态、多种控制方案等等。正如已经提到的，我们测试它时，它仍然是在阿尔法，所以你的里程可能会有所不同的性能。例如，*棘轮:角斗士*(在美国被称为*棘轮:僵局*)在发布时无法播放，在完成第一个过场动画后会崩溃，随后才会更新。

对于那些寻找源代码的人来说， [Tahlreth 在 Reddit](https://www.reddit.com/r/EmulationOnAndroid/comments/qzrgb5/someone_posted_an_alleged_aethersx2_apk_i_have/hlqnovs/) 上分享说，LGPL 的部分将根据要求提供。您还可以“根据许可证的要求，用提供的对象文件重新链接组合的共享库。”根据 Tahlreth 的说法，不会公开任何 Java 源代码，给出的原因是为了防止克隆产品被塞满广告和应用内购买。鉴于已经有一些应用程序声称自己是 AetherSX2，这种说法确实有道理。AetherSX2 没有广告，甚至连上网都没有。LGPL 和 GPL 的区别在于，在 LGPL 的情况下，开发者可以借用、修改和重新发布代码，作为他们自己项目的一部分，只要这部分代码在 LGPL 下被重新许可。项目的其余部分被允许在另一个许可证下。在 GPL 的情况下，*整个*项目将需要 GPL 的许可。

如果你也看过 AetherSX2 的任何片段，你会注意到它没有 D-Pad，只有一个控制杆。在游戏进行到一半时，可以通过访问模拟器菜单来显示这些额外的控件。问题是，由于屏幕空间的减少，没有理由一直显示这些，尤其是许多游戏没有它们也能工作。我在这方面唯一有问题的游戏是*棘轮:角斗士*，因为需要第二个控制杆来转动相机。

## 设置 Aether SX2 以获得最佳性能

你可以采取一些措施来提高 AetherSX2 的性能，事实上，开发人员已经在他们的 POCO F3 和骁龙 870 上进行了大量测试。有很多设置你可以调整和使用，但是我实际上只修改了三个。

您可以调整的第一个设置可以说是最重要的是 GPU 渲染器。你可以选择 Vulkan 或 OpenGL，你得到的性能将取决于你使用的设备和你玩的游戏。例如，在联发科天玑 9000 上使用 Vulkan 可能比使用 OpenGL 更好。

如果你没有听说过 Khronos Group 的 [Vulkan](http://xda-developers.com/t/vulkan) Graphics API，那就把它当成 OpenGL 或 OpenGL ES 等图形 API 的替代品吧。它得到了英伟达和英特尔等公司的支持，旨在给开发者在编写跨平台游戏时提供更多选择。它还具有较低的 CPU 开销，这反过来可以带来更好的性能。正如 [Tahlreth 所说，](https://www.reddit.com/r/EmulationOnAndroid/comments/r8yzgc/is_vulkan_really_better_than_opengl_es/hn9r7jf/) OpenGL 只是在某些游戏中更快，因为它有帧缓冲提取。您的里程会因此而有所不同。

下一个选项是欠锁，我发现欠锁到 75%时效果很好。第三个也是最后一个是在撰写本文时最新的 AetherSX2 更新中添加的新选项，那就是“跳过重复帧”。它试图检测游戏的内部帧速率，并防止它出现重复的帧。结合这一点和欠锁的游戏，如*的速度需求:地下 2* 从边界不可玩到以 100%的速度运行。

## 游戏测试

### 棘轮和叮当公司

棘轮叮当是我在 PlayStation 2 中最喜欢的怀旧游戏，也是我最兴奋在智能手机上玩的游戏。虽然性能还不完美，但您可以采取一些措施来改善它。上面的视频是在一加 9 Pro 上录制的，具有开箱即用的 AetherSX2 体验，也就是说，没有进行任何调整或其他更改。

### 极品飞车:地下 2

《极品飞车:地下 2》是需要额外调整才能运行的游戏之一。然而，当应用 75%的欠锁并删除重复的帧渲染时，速度从大约 50-60%变为 100%。上面的镜头也是在一加 9 Pro 上拍摄的，尽管游戏确实挂在视频的最后。这款游戏在 PCSX2 上模拟多年都有问题，在这里运行如此之好是一个不可思议的成就。

### 辛普森一家:打了就跑

《辛普森一家:Hit & Run 是我在测试智能手机时经常回来玩的一款游戏，因为这是一款我非常熟悉的游戏。通过 AetherSX2，这无疑是玩游戏的最佳方式，比通过 Dolphin Emulator 之类的方式运行要好得多。我甚至在[谷歌 Pixel 6 Pro](https://www.xda-developers.com/google-pixel-6/) 上测试了它，虽然有很多图形故障，但游戏运行得很好——比海豚模拟器好。你可以在下面看到一个简短的游戏片段。Vulkan 渲染器在非 Adreno GPUs 上不起作用。

## 如何下载 AetherSX2

AetherSX2 在谷歌 Play 商店上公开发布，你也可以直接从开发者那里下载 APK。你也可以[在登录谷歌账户](https://play.google.com/apps/testing/xyz.aethersx2.android)时注册 alpha。

鉴于过去 PlayStation 2 模拟的替代方案，AetherSX2 是一个了不起的进步。PCSX2 开发人员对它的支持也很有帮助，我们期待着看到仿真器在未来如何发展和成熟。我个人很高兴看到新的高通骁龙 8 代 2 将如何发展。一定要试一试。