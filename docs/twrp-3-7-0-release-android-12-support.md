# TWRP 3.7.0 发布，终于带来 Android 12 支持

> 原文：<https://www.xda-developers.com/twrp-3-7-0-release-android-12-support/>

TeamWin Recovery Project，简称 TWRP，是目前为止 Android 售后开发领域最流行的定制恢复解决方案。有了它，您可以刷新新的自定义 rom，进行完整的数据备份，修改受保护的文件，以及用您的设备做更多的事情。该项目已经存在多年，支持多种设备。

上一个主要的 TWRP 版本是在去年 11 月宣布的。将近一年后，TeamWin 带着另一个重大更新回来了:TWRP 3.7.0。除了新增功能，这个版本还增加了对 Android 12 的官方支持。

## TWRP 3.7.0 的新功能

这个版本最重要的变化是 TWRP 现在跨三个不同的分支开发。新推出的 *android-12.1* 分支现在支持运行 Android 12/12L 的设备上的数据解密，因此它是新设备的默认目标。出于兼容性原因，现有的 *android-11* 分支也从其继任者那里获得了一系列功能。另一方面，大多数传统设备仍然可以从 *android-9.0* 分支中构建出来。

您可以通过查看构建版本来检查设备正在使用哪个分支——来自最新分支的正式构建在文件名中会有“12-0”。

值得注意的是，TWRP 还没有对 Android 13 的任何官方支持，但它正在开发中。

TWRP 3.7.0 的完整变更日志可以在下面找到:

### TWRP 3.7.0 变更日志

**安卓 12.1 和安卓 11 分支**

*   FFS 设备的 MTP 错误处理- nijel8
*   模块正在加载 opt-in - CaptainThrowback
*   SELINUX 缺少上下文- CaptainThrowback
*   使用加密备份删除更多不推荐使用的代码
*   主题版本移植到 golang - AndroiableDroid
*   TWRP 的 Python 支持- CaptainThrowback
*   中文更新- bluehomewu
*   排除/data/extm - sekaicg
*   MTP 修复复制文件> 4G - sekaicg
*   在供应商 bigbiff 中配置硬件二进制文件
*   不要强制使用超大容量的滚烫咖啡
*   解锁 setup - me-cafebabe 中的所有块分区
*   二进制 xml - me-cafebabe 上的 RapidXML bail
*   仅当逻辑分区存在时才创建其符号链接- me-cafebabe
*   状态栏图标的主题变量
*   委员会定义的备份目录排除- DarthJabba9
*   波兰语更新- kacskrz
*   包括 fastbootd 和板变量- me-cafebae
*   在 zip 安装期间解锁块设备
*   更新 size - me-cafebabe 时将分区挂载为 RO
*   允许取消超级设备在“只有我的设备”咖啡桌上的映射
*   在刷新 TWRP 之前解锁块分区

**安卓 12.1 分支**

*   构建期间的 BASH 和 nano 修复
*   zip 安装增强功能- DarthJabba9
*   Android 12 加密支持- bigbiff
*   12 - me-cafebabe 的依赖关系修复
*   cryptfs-hw fixes - me-cafebabe
*   FDE 兼容性-我的咖啡
*   boot-hal 1.2 支持- tnakamur
*   boot-hal 库修复- CaptainThrowback
*   不要将 fastbootd 包括在所有设备中
*   内核模块加载-等待电池系统初始化- sekaicg
*   修复安装自定义主题- sekaicg
*   android 12 - me-cafebabe 中 XML 二进制文件的更新处理
*   跳过解密修复- sekaicg
*   ABX xml 文件的集成代码- _that 和 DarthJabba9

**Android 11 分支**

*   修复在没有供应商分区的设备上复制策略- webgeek1234
*   为 system _ ext partition-me-cafe babe 设置默认值

**安卓 9 分支**

*   中文更新- bluehomewu
*   波兰语更新- kacskrz
*   TWRP 对 Oreo 及以上版本的 Python 支持
*   V1 修复- bigbiff

* * *

## 新支持的设备

除了主要版本的提升，官方支持的设备列表也有所增长。该团队现在增加了对以下智能手机的支持:

此外，一些设备(如下所列)已经获得了新的维护者。

* * *

## [计] 下载

TWRP 3.7.0 版本适用于大多数当前支持的设备。要为您的设备下载最新版本，请通过下面的链接访问 TWRP 官方网站。一定要看看你的设备的 XDA 分论坛，因为 TWRP 的维护者可能会在新版本上线时发布额外的设备特定说明。

**[为您的设备下载 TWRP](https://twrp.me/Devices/)**

如果你想在不使用 PC/Mac 的情况下下载 TWRP 的官方版本，你应该看看 TWRP 的官方应用程序。当新版本的自定义恢复可用时，该应用程序会提醒您。

* * *

**来源:** [TWRP](https://twrp.me/site/update/2022/10/10/3.7.0-released.html)