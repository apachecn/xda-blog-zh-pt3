# Windows 11 更新跟踪器:下载并安装最新的 Windows 11 更新

> 原文：<https://www.xda-developers.com/windows-11-update-tracker/>

Windows 11 的首次展示正在全速进行。事实上，微软最新版本操作系统的最新重大更新——Windows 11 2022(版本 22 H2)Moment 2——已经作为可选更新在[推出。然而，这些版本并不是没有问题，这个雷德蒙的科技巨头](https://www.xda-developers.com/windows-11-moment-2-update-launch/)[很清楚这个事实。该公司定期推出 Windows 11 的更新，以修复漏洞并引入新功能。本文将作为知识库(KB)文章的中央存储库，并提供与 Windows 11 相关的所有更新的下载链接。](https://docs.microsoft.com/en-us/windows/release-health/status-windows-11-22h2)

## 词汇表

Windows 更新以一种称为 Microsoft CAB(CAB)的特殊存档文件格式进行压缩，这种格式支持用于维护存档完整性的嵌入式数字证书。当通过[微软更新目录](https://www.catalog.update.microsoft.com/Home.aspx)发布时，微软经常将它们包装成 MSU(微软更新)格式。

该索引的主要焦点集中在累积更新(也称为每月汇总)上，其中包括打包在一起的安全性和可靠性更新。因为它们本质上是累积的，所以最新的汇总软件包可以将目标 Windows 版本更新到最新的内部版本，而不管以前的内部版本号是多少。

在某些情况下，您可能需要在安装最新的累积更新(CU)之前应用服务堆栈更新(SSU)。服务栈是安装其他操作系统更新的代码，因此微软通常在发布独立的 MSU 包之前将它们与 Cu 捆绑在一起。高级用户或系统管理员可能仍然喜欢使用 CAB 版本，以便于部署。在这种情况下，务必在与 CU 接合之前安装/集成 SSU。

微软也为。Windows 操作系统的. NET 框架部分。与 SSU 不同的是，它们与常规的 Cu 分开分发。

Windows 功能体验包是另一种类型的更新，它为客户提供了主要 Windows 功能更新之外的新功能改进。

然后是针对 Windows 安装引擎的动态更新(DU)。它们会被自动下载并即时应用，以修复 Windows 恢复环境(WinRE)、设置二进制文件或 Windows 安装程序用于功能更新的任何文件。然而，为了避免混乱，我们决定不将它们包含在这个索引中。

要清楚地了解 Windows update 术语，请参阅关于 Windows update 的[类型的文章。请记住，操作系统间(例如从 Windows 10 到 Windows 11)或内部版本(例如从 Windows 10 2019 年 11 月更新/版本 18363 到 2020 年 5 月更新/版本 19041)更新是一种更复杂的情况。微软使用](https://docs.microsoft.com/en-us/troubleshoot/windows-client/deployment/standard-terminology-software-updates)[统一更新平台(UUP)](https://docs.microsoft.com/en-us/windows/deployment/update/windows-update-overview) 处理这样的升级路径，其细节不是本教程的一部分。

## Windows 11 构建索引

以下指数按时间顺序排列。由于更新是从不同的开发管道中推出的，较高的 KB/build 号并不总是最新版本的理想指标。请在安装前浏览更新描述。

在某些情况下，您可能会发现两个或更多的构建指向同一个知识库文章。这对于最新发布的版本来说是非常正常的，因为微软很可能会将 KB 编号分配给具有聚合修复功能的最新版本。

### 内部版本号 22621 (22H2) - Windows 11 2022 更新

支持包

自. 290 发布以来，微软已经决定将 Windows 11 22H2 的测试版分成两组。22622.x 系列是为前沿用户设计的，因为这些构建将默认启用有趣的特性。从. 730 发行版开始，实验基础已经提升到 22623.x，从. 1391 发行版开始提升到 22624.x。另一组内部人员将留在 build 22621.x 中，这些新功能将被关闭。

您可以通过安装下面链接的相应启用包，手动从 22621.x 切换到 22622.x(或 22623/4.x)。注意，它要求事先至少安装 build 22621.285(针对 22622) / 22621.726(针对 22623) / 22621.1390(针对 22624)，但微软从未公开发布过那些版本。因此，只要您安装了更高版本号的更新，您就可以开始了。

Windows 累积更新

我们在下面保留了以前累积更新的链接。

的累积更新。NET Framework 3.5 和 4.8.x

以前的链接。NET Framework 3.5 和 4.8.x 累积更新也会保留:

* * *

### 内部版本号 22000 (21H2) - Windows 11(原始版本)

Windows 累积更新

先前累积更新的链接也会保留:

的累积更新。NET 框架 3.5 和 4.8

以前的链接。也保留了. NET Framework 3.5 和 4.8 累积更新:

(可选)。NET 框架 4.8.1

自 2022 年 8 月起，一款单机。NET Framework 4.8.1 更新适用于 Windows 11 和 Windows 10。因为微软提供累积更新。NET Framework 4.8.1 独立于 4.8 分支，我们在下面单独的索引中列出了它们。基本 CAB 包和离线安装程序是独立于版本的，因此您可以在 Windows 11 和 Windows 10 上安装它们。

(可选)的累积更新。NET 框架 3.5 和 4.8.1

* * *

## 如何安装 Windows 11 累积更新

### 驾驶室套件

要安装 CAB 更新包，您需要使用一个名为部署映像服务和管理(DISM)的内置系统实用程序。[命令行语法](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/dism-operating-system-package-servicing-command-line-options)应该如下所示:

```
 dism /online /add-package /packagepath:<path_to_cabfile> 
```

### CAB 和 PSF 封装

自 [Windows 10 Insider 预览版 Build 21382](https://blogs.windows.com/windows-insider/2021/05/14/announcing-windows-10-insider-preview-build-21382/) 以来，微软在最新的累积更新(LCU)格式上进行了重大改变。因此，最终用户不能直接使用 CAB 文件。要使用内置更新模块执行安装，必须存在相应的[补丁存储文件](https://docs.microsoft.com/en-us/windows/deployment/update/psfxwhitepaper) (PSF)包。这就是为什么人们可以在 Windows 11 UUP 转储中找到对应于每个 LCU 的 PSF 文件。在联机安装的情况下，Windows Update 仅下载并生成缺失的 PSFX (PSF Express)有效负载，而 CAB 包仅包含清单。

然而，DISM 一个人无法处理 PSF 包，这意味着我们需要以某种方式手动合并 PSF 和 CAB 文件，然后再尝试离线安装它们。幸运的是，有一个名为 [PSFX Repack](https://github.com/abbodi1406/WHD/raw/master/scripts/PSFX_Repack_6.zip) 的开源工具可以完成这项工作。

*   将 PSFX 重新打包工具的归档文件解压到一个路径较短的文件夹中(如“D:\PSFX_Repack”)。
*   下载与 SSU 和 LCU 对应的 CAB 和 PSF 文件，并将其移动到上述文件夹中。请参考上述索引，在下载前记下适当的 KB 编号。
    *   您可以从文件名中删除散列(如果存在的话)，这样文件集看起来就像`Windows10.0-KBxxxxxxx-x64.cab`和`Windows10.0-KBxxxxxxx-x64.psf`。这一步是可选的，因为最新版本的 PSFX 重新打包工具可以处理新的命名方案。

*   运行`psfx2cab_CLI.cmd`生成合并的 CAB 文件。

*   首先使用 DISM 安装最新的 SSU CAB 文件，然后安装生成的 LCU CAB 文件。

### MSU 套餐

另一方面，MSU 变种在本质上有点独立，因为人们可以简单地双击它来安装包。请注意，DISM 也可以安装 MSU 文件。

安装完成后，系统会提示您重启电脑以使更改生效。

* * *

## 确认

Windows 11 中的设置应用程序有一个选项，可以查看你的 PC 上安装的更新列表。下面是访问它的方法。

*   打开设置，点击 *Windows 更新*。
*   点击/轻触*更新历史*。

经典控制面板中的传统*程序和功能*小程序也可以显示已安装更新的列表。

*   右键开始，点击*运行*。
*   键入`appwiz.cpl`并点击确定。这将打开经典控制面板中的程序和功能。
*   单击左侧的*查看已安装的更新*链接。这将向您显示更新列表以及安装日期列。

如果您喜欢命令行，那么您也可以选择 DISM 或 Windows Management Instrumentation(WMIC)。您需要从 Windows 终端的提升实例执行该命令。

```
 dism /online /get-packages /format:table | findstr "Package_for" 
```

```
 wmic qfe 
```

* * *

我们希望这篇文章不仅可以作为 Windows 11 的通用更新索引，还可以提供对其他 Windows 版本有用的通用安装说明。我们将更新此指南，提供更新 Windows 版本的链接，请稍后再来查看！