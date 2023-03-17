# Android 13 Beta 3 获得了又一个漏洞修复更新

> 原文：<https://www.xda-developers.com/android-13-beta-3-3-released/>

# 谷歌推出 Android 13 Beta 3.3，修复了一系列错误

谷歌正在推出 Android 13 Beta 3.3，以解决之前测试版中存在的一些错误。查看变更日志！

Android 13 的测试分支[刚刚获得了一个新的 bug 消除更新。继 Android 13 Beta 3 的早期](https://www.xda-developers.com/android-13/)[更新](https://www.xda-developers.com/a-minor-issue-fix-arrives-in-android-13-beta-3-1-update/)增量[更新](https://www.xda-developers.com/android-13-beta-3-2-released/)之后，这个新版本修复了一系列问题，包括 UI 渲染缓慢、无法连接到 Wi-Fi 网络、系统 UI 崩溃以及其他一些问题。

Android 13 Beta 3.3 的 build 号是 **TPB3.220617.002** 。不过，安全补丁级别没有变化，因此这个版本仍然是 2022 年 6 月。您可以在下面的更新中找到已发布修补程序的完整列表:

*   修复了 Pixel launcher 的一个问题，如果为应用程序抽屉启用了**总是显示键盘**选项，那么当用户关闭应用程序抽屉并在主屏幕上打开应用程序文件夹时，键盘也会错误地显示。([问题编号 236584457](https://issuetracker.google.com/issues/236584457) )
*   修正了在某些情况下，如手势返回，系统界面崩溃的问题。([问题编号 236558007](https://issuetracker.google.com/issues/236558007)
*   修复了在某些情况下，即使网络可用且信号强度良好，设备也无法连接到 WiFi 网络的问题。([问题编号 236617510](https://issuetracker.google.com/issues/236617510)
*   修复了一个问题，即`BluetoothManagerService`继续尝试并绑定到`TbsService`，即使`bluetooth.profile.ccp.server.enabled`是`false`，导致应用程序的缓慢性能和冷启动。
*   修复了一个问题，在某些情况下，设备插入充电后(例如，过夜)，设备会变得没有反应，直到它重新启动。
*   修正了一个关于`lib/list_debug.c`的内核问题，该问题在某些设备上的某些情况下会导致内核崩溃。
*   修复了连接热能管理器在某些情况下导致 UI 渲染缓慢、应用程序无响应以及电池性能不佳的问题。

除了前述的漏洞修复，更新还将 Google Play 服务版本从 *22.18.19* 提升至 *22.21.16* 。

如果你的谷歌 Pixel 设备已经注册了 Android 13 beta 计划，你将自动收到 Beta 3.3 的无线更新。如果你想手动将升级到最新的测试版，你也可以从下面的链接下载完整的 OTA 或者工厂镜像。

**[下载安卓 13 Beta 3.3](https://www.xda-developers.com/how-to-download-android-13/#beta3point3)**

* * *

**来源:**[Reddit 上的 Android Beta 程序](https://www.reddit.com/r/android_beta/comments/vm0veo/)