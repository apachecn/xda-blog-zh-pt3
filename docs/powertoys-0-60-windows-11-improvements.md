# PowerToys 0.60 为 Windows 11 用户增加了改进

> 原文：<https://www.xda-developers.com/powertoys-0-60-windows-11-improvements/>

微软发布了最新版本的 PowerToys，这是其为 Windows 10 和 11 上的高级用户提供的工具套件，使其版本达到了 0.60。这个版本主要集中在小的改进和修复上，但也有一些值得注意的变化，特别是如果你使用的是 Windows 11。

首先，图像缩放工具和 PowerRename 已经被添加到 Windows 11 的上下文菜单中。到目前为止，如果你想在你的文件上使用这些工具中的任何一个，你需要右键单击以显示 Windows 11 上下文菜单，然后选择**显示更多选项**按钮以查看旧菜单，这些功能将在那里显示。此更改减少了重命名文件或调整图像大小所需的步骤。该团队指出，如果你是开发频道的 Windows 内部人员，这可能不太好。

与 Windows 11 相关的另一项改进是“永远在顶部”工具。此工具将任何窗口固定在所有其他窗口的顶部，并用彩色边框突出显示固定的窗口。现在，在窗口 11 上，该边界将具有圆角，以跟随窗口本身的圆角。

此外，还有一些更全面改进，比如针对 OneNote 的新 PowerToys 运行插件。此外，FancyZones 工具现在使用新的区域识别技术，提高了稳定性，并防止您的区域在使用多个监视器时重置。此次更新也使得通过微软商店和 Windows 包管理器安装 [ARM64 版本的 PowerToys](https://www.xda-developers.com/powertoys-0-59-native-arm-support/) 变得更加容易。

PowerToys 0.60 中有很多较小的改进和修复，你可以在下面找到它们。

### PowerToys 0.60 的改进

**通用**

*   已将 Windows App SDK 运行时升级至 1.1.1。(这是 0.59 的修补程序)

**永远在顶端**

*   增加了对更多样的键盘快捷键的支持，并支持低级键盘挂钩。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   在 Windows 11 上为圆角窗口添加了圆角高光。

**FancyZones**

*   修正了所有桌面上显示的窗口不能与 FancyZones 一起工作的错误。(这是 0.59 的修补程序)
*   更改区域布局时，如果该选项打开，窗口将匹配新的大小/位置。(这是 0.59 的修补程序)
*   FancyZones 编辑器中的小 UI 修复。感谢 [@ZetaSp](https://github.com/ZetaSp) ！
*   修复了在 FancyZones 编辑器中正确的画布布局渲染，现在显示了未缩放的监视器分辨率。
*   修正了某些窗口透明度导致窗口空白的问题。

**图像缩放器**

*   图像大小调整条目现在显示在新的 Windows 11 上下文菜单中。

**文件浏览器附加组件**

*   为 svg 文件缩略图添加一个 viewBox 属性，以便它尝试显示整个图像，类似于在预览处理程序中所做的。
*   在降价测试预览中删除了对远程映像的访问。
*   修复了 markdown 预览测试套件中的剥落问题，组件初始化超时正确。
*   修复了 svg 缩略图导致的 WebView2 资源泄漏。

**键盘管理器**

*   编辑器标题栏现在显示在沉浸式黑暗模式主题中。感谢[@威廉布拉德利](https://github.com/WilliamABradley)！

**鼠标效用**

*   鼠标指针十字光标默认激活快捷方式已更改，不会与某些国际键盘上的特殊字符组合发生冲突。

**电源重命名**

*   修复了文件枚举逻辑，仅更改文件名末尾的枚举。
*   单击 regex/date and time cheat sheet 将该项目附加到所选的搜索或替换文本字段。
*   PowerRename 条目现在显示在新的 Windows 11 上下文菜单中。
*   标题栏现在显示在沉浸式黑暗模式主题中。感谢[@ William bradley](https://github.com/WilliamABradley)！

**电动玩具运行**

*   添加了一个设置来禁用和配置搜索查询的输入延迟。(这是 0.59 的修补程序)
*   修复并添加了默认 Web 浏览器检测的日志。(这是 0.59 的修补程序)
*   程序插件现在可以搜索了。按可执行名称链接快捷方式。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   添加了一个新的 OneNote 插件。感谢 [@palenshus](https://github.com/palenshus) ！
*   OneNote 插件中添加了查询缓存和延迟执行功能。感谢 [@palenshus](https://github.com/palenshus) ！
*   时区插件的生活质量修正，包括对空字幕、缺失时区和没有找到预期结果的修正。感谢 [@TobiasSekan](https://github.com/TobiasSekan) ！
*   对过时的 WebRequest API 的调用已被删除。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   在设置插件中增加了共享设置的常用名称。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   计算器法师引擎更新到 2.0.1，为更高的精度。感谢测试和推动改变 [@htcfreek](https://github.com/htcfreek) ！
*   计算器和时间日期插件的翻译修正。感谢 [@htcfreek](https://github.com/htcfreek) ！
*   “搜索设置”条目被添加到设置插件中。感谢 [@jefflord](https://github.com/jefflord) ！
*   删除了不推荐使用的 BinaryFormatter，它包含漏洞。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   添加了设置以更好地控制查询结果顺序。感谢 [@jefflord](https://github.com/jefflord) ！
*   终端插件现在使用更好的 API 来检测已安装的终端包。感谢 [@htcfreek](https://github.com/htcfreek) ！

**设置**

*   修正了一个错误，即使 PowerToys 完全更新了，更新还是失败。(这是 0.59 的修补程序)
*   OOBE 窗口是可调整大小的。(这是 0.59 的修补程序)
*   OOBE 现在可以通过认证代理显示发行说明。
*   OOBE 现在隐藏了 x64 和 ARM64 安装程序的哈希值。
*   键盘管理器页面中的小 UI 修复。感谢 [@ZetaSp](https://github.com/ZetaSp) ！
*   修正复选框控件的内部数据类型。感谢 [@ghost1372](https://github.com/ghost1372) ！
*   标题栏现在显示在沉浸式黑暗模式主题中。感谢[@威廉布拉德利](https://github.com/WilliamABradley)！
*   修正了一个加载系统时的崩溃问题。ARM64 版本 Windows 上的管理 API。

**安装人员**

*   修复了新管道中安装自定义操作 dll 的签名。
*   Visual C++可再发行版已更新到 14.32.31332，并修复了安装较新版本时出现的安装程序错误。感谢 [@snickler](https://github.com/snickler) ！
*   更新了。净依赖于 6.0.6。

**发展**

*   CA1031 警告抑制的清理。感谢 [@davidegiacometti](https://github.com/davidegiacometti) ！
*   Microsoft Store 提交任务中添加了对 ARM64 二进制文件的支持。感谢 [@azchohfi](https://github.com/azchohfi) ！
*   为帮助识别监视器 id 的工具添加了代码。
*   winget 包创建任务增加了对 ARM64 二进制文件的支持。
*   更新了拉式请求模板，以更好地反映项目变更。
*   组件治理检查在新的主分支上被重新激活。
*   CI 无法运行调用较新的 WebView 2 版本的测试，因此在找到解决方案之前，这些测试将被禁用。
*   将测试 SDK 更新到 17.2.0。
*   解决方案中使用的 Nuget 包版本已整合。
*   CodeQL CI 任务在 repo 中被禁用，但在 forks 上引起了问题，因此被删除。
*   特定的牛顿软件。测试中指定了 Json 版本，以避免以前版本中存在的漏洞。
*   FabricBot 配置已添加到存储库中。
*   添加了一个 dependabot 配置，用于更新 GitHub 操作的依赖关系。感谢 [@naveensrinivasan](https://github.com/naveensrinivasan) ！
*   更新了拼写检查操作，并在工作流中添加了生活质量修复。感谢 [@jsoref](https://github.com/jsoref) ！

你可以从 GitHub 下载 PowerToys 0.60，或者，如果你已经安装了应用程序，检查应用程序的更新以获得最新版本。