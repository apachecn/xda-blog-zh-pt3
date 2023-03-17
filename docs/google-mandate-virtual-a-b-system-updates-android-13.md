# 谷歌要求搭载 Android 13 的设备进行虚拟 A/B 系统更新

> 原文：<https://www.xda-developers.com/google-mandate-virtual-a-b-system-updates-android-13/>

据报道，谷歌正在授权虚拟 A/B 支持使用 Android 13 的设备上的 GMS 许可。由于这一点，三星和 Oppo 等制造商的 Android 13 发布设备在落后竞争对手几年后，终于可以支持无缝更新。

对于不知情的人，谷歌在 Android 7.0 牛轧糖中引入了 A/B 分区方案，以加快软件更新。该公司增加了对将某些分区复制成“A”分区和“B”分区的支持。您的活动分区是您当前正在使用的分区，非活动分区可以在后台更新，然后通过快速重启切换到该分区。

这种实现使得 Android 设备上的软件更新明显更快。然而，一些原始设备制造商尚未采用这种方法。例如，三星设备没有 A/B 分区，应用软件更新需要更长时间，这使得设备在几分钟内无法使用。谷歌现在的目标是改变这种情况，让搭载 Android 13 的设备必须支持虚拟 A/B，才能获得 GMS 许可。

谷歌此前试图在所有搭载 Android 11 的设备上强制推行虚拟 A/B 支持。然而，该公司[收回了要求](https://www.xda-developers.com/google-virtual-ab-seamless-updates-android-11/)，并更新了 Android 11 兼容性定义文件(CDD ),建议但不是强制支持 A/B 系统更新。由于这个原因，一些 Android OEMs 还没有实现虚拟 A/B 支持，以及对其设备上无缝更新的支持。

虽然 Android 13 CDD [仍然不要求原始设备制造商提供虚拟 A/B 支持](https://source.android.com/docs/compatibility/13/android-13-cdd#11_updatable_software)，但来自*斯珀*的一份新报告显示，谷歌现在授权它在 Android 13 发布设备上进行 GMS 授权。为此，该公司在供应商测试套件(VTS)中增加了新的测试，使得虚拟 A/B 支持成为 Android 13 发布设备的强制要求。

该报告指出，尽管这些测试在 Android 13 发布前被合并，但它们甚至在发布后仍然存在，这与 Android 11 开发期间的情况形成了对比。"这意味着所有搭载 Android 13 的设备都必须通过这些测试才能获得 GMS 认证。

实际上，如果希望提供谷歌移动服务，谷歌将要求推出 Android 13 设备的原始设备制造商提供虚拟 A/B 支持。正如*斯珀*指出的那样，唯一的例外是*“安卓 13 发布设备搭载的是较旧的供应商软件，这要感谢作为谷歌需求冻结(GRF)项目结果的 VTS 测试中的例外。*

随着虚拟 A/B 支持成为带 GMS 的 Android 13 发布设备的一项要求，无缝更新最终将在所有 OEM 的设备上可用。关于虚拟 A/B 以及它如何加速软件更新的更多信息，请查看下面链接的*斯珀*博客。

* * *

**Via:** [斯珀](https://blog.esper.io/android-13-virtual-ab-requirement/)