# 这些功能在 Windows 10 21H1 中被删除或弃用

> 原文：<https://www.xda-developers.com/features-removed-deprecated-windows-10-may-2021-update/>

# 在 Windows 10 2021 年 5 月更新中，这些功能已被删除或弃用

微软今天发布了 Windows 10 2021 年 5 月更新，和往常一样，有一些功能被删除或弃用。

今天，微软[向非业内人士](https://www.xda-developers.com/windows-10-may-2021-update-now-available-for-everyone/)发布了 Windows 10 2021 年 5 月更新。从今天开始，您应该可以通过 Windows Update 获得它，也可以通过媒体创建工具获得它。如果你想安装它，你可以[在这里查看我们的指南](https://www.xda-developers.com/how-to-install-windows-10-may-2021-update/)。

与往常一样，新功能更新会带来新功能，但这也意味着一些功能将会消失。微软将这些分为[弃用和移除列表](https://docs.microsoft.com/en-us/windows/deployment/planning/windows-10-deprecated-features)，前者仅表示该功能不再开发，并将在未来的更新中移除。

这是一个小更新，所以没有任何疯狂的变化也就不足为奇了。名单很小。以下是被否决的内容:

| 

特征

 | 

细节和缓解措施

 |
| --- | --- |
| 个性化漫游 | 个性化设置(包括壁纸、幻灯片、强调颜色和锁屏图像)的漫游不再开发，可能会在未来的版本中删除。 |
| Windows Management 规范命令行(WMIC)工具。 | WMIC 工具在 Windows 10 版本 21H1 和 Windows Server 的 21H1 半年期渠道发行版中已被弃用。这个工具被 WMI 的 Windows PowerShell 所取代。注意:这种反对仅适用于[命令行管理工具](https://docs.microsoft.com/en-us/windows/win32/wmisdk/wmic)。WMI 本身没有受到影响。 |

显然，这些不是你会想念的东西。当人们不使用时，功能通常会被弃用。以下是删除的内容:

| 

特征

 | 

细节和缓解措施

 |
| --- | --- |
| 基于 XDDM 的远程显示驱动程序 | 此版本中删除了对基于 Windows 2000 显示驱动程序模型(XDDM)的远程显示驱动程序的支持。使用基于 XDDM 的远程显示驱动程序的独立软件供应商应该计划迁移到 WDDM 驱动程序模型。有关实现远程显示间接显示驱动程序的更多信息，请参见 IddCx 版本 1.4 及更高版本的[更新。](https://docs.microsoft.com/en-us/windows-hardware/drivers/display/iddcx1.4-updates) |
| 微软 Edge |  |

值得注意的是，虽然微软 Edge Legacy 在删除的列表中，但它实际上并不是此次更新的一部分。它在之前的累积更新中被移除，所以即使你不安装 Windows 10 版本 21H1，你仍然会获得 Chromium Edge 其实你应该已经有了。