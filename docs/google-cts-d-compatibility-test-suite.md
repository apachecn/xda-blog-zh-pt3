# CTS-D 是一个新的兼容性测试套件模块，由应用程序开发人员进行测试

> 原文：<https://www.xda-developers.com/google-cts-d-compatibility-test-suite/>

# CTS-D 是一个新的兼容性测试套件模块，由 Android 应用程序开发者提交测试

为了让应用开发者有机会分享他们对设备兼容性问题的独特观点，谷歌推出了新的 CTS-D 模块。

作为 Android 兼容性计划的一部分，谷歌允许智能手机原始设备制造商访问兼容性测试套件(CTS)。该套件包括超过 200 万个测试案例，原始设备制造商使用这些案例在智能手机开发过程的早期清除错误，以便用户在各种设备上获得一致的应用体验。然而，CTS 主要包括 Android 工程师编写的测试，应用程序开发人员很少参与。为了让应用开发者有机会分享他们的*“对实际设备兼容性问题的独特观点”，*谷歌现在推出了 CTS-D。

CTS-D 是一个新的 CTS 模块，包括由应用程序开发人员编写的兼容性测试。它[已经由社区](https://android-review.googlesource.com/c/platform/cts/+/1890987)贡献的一些测试组成，谷歌现在邀请更多的开发者来构建和贡献测试案例，以捕捉他们面临的应用兼容性问题。该公司进一步指出:*“我们知道你们中的许多人已经创建了自己的测试来验证各种设备上的兼容性。我们希望与你们合作，将这些测试引入 AOSP。”*

要提交一个新的测试，你可以在将你的测试代码提交给 AOSP 之前，使用这个模板提交一个提议[。Android 团队随后将审核您的提交，以验证其资格。目前，谷歌正在邀请应用开发者提交](https://issuetracker.google.com/issues/new?component=1124973&template=1633344)[电源管理](https://developer.android.com/about/versions/pie/power)测试案例。

除了应用开发者，谷歌还*“强烈建议”智能手机原始设备制造商使用 CTS-D 来识别和缓解问题。然而，该公司并不严格要求 OEM 厂商运行 CTS-D 测试以通过设备认证。因此，一些原始设备制造商可能不会在其设备上运行 CTS-D 测试。如果事实证明是这样，应用程序开发人员将可以选择使用[问题跟踪模板](https://issuetracker.google.com/issues/new?component=1124973&template=1633344)提交一份设备未通过 CTS-D 测试的报告。谷歌表示，它将与 OEM 合作伙伴一起解决这个问题。*

 ** * *

**来源:** [安卓开发者博客](https://android-developers.googleblog.com/2022/06/developer-powered-cts-cts-d.html)*