# Windows 11 版本 22H2 中的新错误中断了远程桌面连接

> 原文：<https://www.xda-developers.com/windows-11-version-22h2-remote-desktop-bug/>

Windows 11 版本 22H2 已经给一些用户带来了问题，现在，微软已经承认了另一个影响最新 [Windows 11](https://www.xda-developers.com/windows-11/) 更新的问题。一些用户，特别是在商业环境中，在尝试使用 Windows 远程桌面应用程序连接到另一台电脑时，可能会遇到死机或崩溃的情况。

根据微软的说法，问题发生在使用远程桌面网关或远程桌面连接代理建立连接时，大多数家庭用户应该不会受到它的影响，因为默认情况下连接过程是不同的。例如，当尝试访问远程桌面服务集合或使用 RemoteApp 和桌面连接时，可能会出现此问题。

用户在尝试连接到虚拟机时，可能会在“加载虚拟机”或“配置远程连接”阶段注意到该问题。在某些情况下，Remote Desktop 应用程序可能只是停止响应，但也有可能您会看到一条错误信息，提示连接已结束。微软表示，无论你试图连接的是什么版本的 Windows，问题都会发生，所以问题的根源在于客户端机器。

如果你碰巧遇到这个问题，远程桌面应用停止响应，你需要使用 Windows 中的任务管理器终止它。您需要浏览到任务管理器的进程选项卡，查找 mstsc.exe，然后终止该进程。

虽然这个问题还没有一个确定的解决方案，但是如果您遇到这个问题，Microsoft 已经提供了一个潜在的解决方法。然而，该公司警告说，使用远程桌面时，应用这种解决方法会导致性能下降，所以一旦有了解决方案，您就会想要恢复它。从本质上来说，修复包括在客户端设备上禁用 UDP，这可以通过策略编辑器来完成。方法如下:

*   打开组策略管理控制台(对于受管理的企业设备)或组策略编辑器(对于不受管理的家庭设备)
*   在右侧窗格中，导航到**计算机配置** > **管理模板** > **Windows 组件** > **远程桌面服务** > **远程桌面连接客户端**
*   找到一个名为**的策略，关闭客户端**上的 UDP，并将其设置为**启用**
*   点击**确定**并重启设备以应用更改

完成后，您应该能够再次使用远程桌面连接，但是如上所述，这可能会影响 WAN 上远程桌面连接的性能。在 Microsoft 发布针对此问题的修复程序之前，您可能不得不忍受这种情况，但问题解决后，您会希望将此策略更改为其原始设置。

这只是困扰 Windows 11 版本 22H2 的众多问题中的最新一个，但至少微软正在积极解决这些问题。就在本周早些时候，该公司[解除了因印刷问题](https://www.xda-developers.com/windows-11-22h2-printing-safeguard-removed/)而实施的兼容性搁置。这些问题现在已经得到修复，所以如果你的 Windows 11 机器以前无法更新到版本 22H2，你现在可能可以这样做。

* * *

**来源:** [微软](https://learn.microsoft.com/en-us/windows/release-health/status-windows-11-22h2#2954msgdesc)