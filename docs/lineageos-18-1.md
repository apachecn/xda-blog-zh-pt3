# 基于 Android 11 的 LineageOS 18.1 现已面向近 60 款设备推出

> 原文：<https://www.xda-developers.com/lineageos-18-1/>

在售后市场开发领域，并不缺乏定制 ROM 的选择，但如果有一个我们可以认为是“最大的”，那就是 LineageOS。LineageOS 项目受到社区的喜爱有很多原因，不仅仅是因为定制 ROM 在香草 AOSP 基础上提供的所有功能。得益于[设备支持要求宪章](https://www.xda-developers.com/lineageos-device-support-requirements-charter/)，如果您选择在受支持的设备上闪存 LineageOS 的官方版本，您可以放心，您的设备将运行稳定的软件，并且针对严重的安全漏洞保持最新——通常远远超过官方制造商支持的结束时间。现在，该团队已经准备好迈向下一个重大里程碑:正如诺伦·约翰逊[在官方博客](https://lineageos.org/Changelog-25/)中宣布的那样，LineageOS 18.1 终于在这里以 Android 11 为基础。

**[XDA 论坛](https://forum.xda-developers.com/c/lineageos.6080/)**

## 为什么是血统 18.1 而不是 18.0？

通常情况下，随着主要版本号的变化，会有一个大的平台更新。虽然在 Android 11 的源代码[之上](https://www.xda-developers.com/android-11-source-code-aosp/)重新构建 LineageOS 代码库确实证明了“18”部分的合理性，但 subversion 的变化还涉及到其他东西。谷歌没有提高次要版本号，而是延续传统，通过“像素功能下降”为新的 Android 版本[推出重大功能更新。因此，LineageOS 团队](https://www.xda-developers.com/pixel-feature-drop-adaptive-sound-google-photos-suggestions/)[决定](https://lineageos.org/Changelog-25/)从 18.0 升级到 18.1。

* * *

## LineageOS 18.1 中的新功能

LineageOS 18.1 具有多项新功能和增强功能:

*   从[2020 年 4 月](https://www.xda-developers.com/google-april-2020-android-security-bulletin-patches-pixel-4-3-3a-2-xl/)到[2021 年 3 月](https://www.xda-developers.com/android-march-2021-security-update/)的安全补丁已经合并到 LineageOS 15.1 到 18.1。
    *   18.1 构建目前基于 android-11.0.0_r32 标签，即 Pixel 系列 unifiedtag。
*   Wi-Fi 显示可用于较新的高通设备，具体视设备而定。
*   WebView 已更新至 Chromium 89.0.4389.105。
*   Recorder 应用程序在很多方面都得到了极大的改进，快去给自己留个语音备忘录吧，这样你就不会忘记那个好主意了！
    *   屏幕录制已被移动到 QS 瓷砖，以配合 AOSP 的行为。
    *   用户界面已经过改进，现在还有一个用户界面，可以方便地查看、管理和分享您的语音笔记。
    *   现在可以选择音频录音的质量来节省空间。
    *   现在可以暂停和恢复录制。
*   FOSS [Etar](https://github.com/Etar-Group/Etar-Calendar) 应用程序已经被派生、改进并发布，取代了停滞不前且基本无人维护的 AOSP 日历。
*   Calyx institute 的 FOSS [Seedvault](https://calyxinstitute.org/projects/seedvault-encrypted-backup-for-android) 应用程序已经[作为内置备份解决方案](https://www.xda-developers.com/lineageos-seedvault-open-source-backup-solution/)包含在内。
    *   要使用它，导航到设置->系统->备份，然后“更改备份提供商”到 Seedvault。然后，您可以单击“Seedvault Backup”来配置、计划和加密备份！
    *   使用 Seedvault 创建的备份可以上传到您的 Nextcloud 实例、外部 USB 驱动器或保存在您的本地存储上。
*   现在，在非 A/B 设备上有一个选项可以与操作系统一起更新恢复映像，就像普通操作系统一样！
    *   要使用此功能，请在初始设备设置期间启用该选项，或者导航至设置->系统->更新程序(显示更多)右上角的三点菜单->并选中“更新操作系统旁边的恢复”。
*   音乐应用 Eleven 现在有了一个更新的用户界面，并与音乐播放器的所有新的 Android 功能很好地集成在一起，例如从通知中查找。
*   所有 LineageOS 应用程序现在都支持黑暗模式。

除了上述改进之外，LineageOS 18.1 和 17.1 代码库还包含以下更改:

*   LineageOS recovery 现在有了一个新的、丰富多彩的、有趣的用户界面，更加易于使用。
*   防火墙现在可以通过让应用程序认为设备处于飞行模式来阻止所有连接。
*   该团队引入了新的可扩展卷对话框 UI。
*   部分截图增加了多项功能，并与 AOSP 的新“即时截图”功能相结合。
*   投石机现在支持图标包。
*   ADB 根经过重新设计，以确保与其他第三方根解决方案兼容。

* * *

## 其他变更

### 敏感的电话号码

LineageOS 现在提供了一个帮助热线联系人列表，可以在股票拨号器应用程序的 3 点菜单中访问。列表中的所有号码都被认为是“敏感”的，这意味着[它们会自动从通话记录中隐藏](https://www.xda-developers.com/lineageos-changelog10-sensitive-numbers-small-fixes-and-cve-tracker/)。GitHub 上提供了针对特定国家的敏感号码列表[，任何想要添加新号码的人都可以通过 Gerrit 提交更改。](https://github.com/LineageOS/android_vendor_lineage/blob/lineage-18.1/prebuilt/common/etc/sensitive_pn.xml)

### Addon.d-v3

addon.d 模块现在支持额外的系统分区，包括`/vendor`、`/product`和`/system_ext`。这一更改是为了简化这些分区中的所有备份和恢复操作。

* * *

## linea geos 18.1–受支持设备的官方版本

现在，来看看宣布支持 LineageOS 18.1 的实际设备。第一批已经相当大，随着时间的推移，更多的开发人员可能会扩大名单，因为他们完成了设备启动并满足设备支持要求章程中规定的要求。请注意，在本文首次发布时，并非所有的构建都是活动的，所以请回来查看您的设备是否有可用的构建。

| 

没有。

 | 

设备和论坛链接

 | 

设备代号和维基链接

 | 

维护者

 |
| --- | --- | --- | --- |
| 1. | [基本 PH-1](https://forum.xda-developers.com/c/essential-phone.6486/) | [马塔](https://wiki.lineageos.org/devices/mata/) | 哈格特克、英特威吉尔、约翰逊、拉希德 |
| 2. | [F(x)tec Pro1](https://forum.xda-developers.com/c/f-x-tec-pro1.9284/) | [pro1](https://wiki.lineageos.org/devices/pro1/) | bgcngm，intervigil，mccreary，npjohnson，tdm |
| 3. | [谷歌 Nexus 6](https://forum.xda-developers.com/c/nexus-6.3706/) | [沙木](https://wiki.lineageos.org/devices/shamu/) | npjohnson 公司 Elektroschmock |
| 4. | [谷歌 Nexus 7 2013 (Wi-Fi，重新分区)](https://forum.xda-developers.com/c/nexus-7-2013.2407/) | [弗洛克斯](https://wiki.lineageos.org/devices/flox/) | 约翰逊，瑟布莱泽，埃莱克特罗斯克 |
| 5. | [谷歌像素 2](https://forum.xda-developers.com/c/google-pixel-2.7067/) | [大眼瞪小眼](https://wiki.lineageos.org/devices/walleye/) | Eamo5 |
| 6. | [谷歌 Pixel 2 XL](https://forum.xda-developers.com/c/google-pixel-2-xl.7074/) | [台门](https://wiki.lineageos.org/devices/taimen/) | Eamo5 |
| 7. | [谷歌 Pixel 3a](https://forum.xda-developers.com/c/google-pixel-3a.8868/) | [萨尔戈](https://wiki.lineageos.org/devices/sargo/) | 约翰逊·德赛 |
| 8. | [谷歌 Pixel 3a XL](https://forum.xda-developers.com/c/google-pixel-3a-xl.8875/) | [鲣鱼](https://wiki.lineageos.org/devices/bonito/) | 约翰逊·德赛 |
| 9. | [谷歌像素 4](https://forum.xda-developers.com/c/google-pixel-4.9014/) | [火焰](https://wiki.lineageos.org/devices/flame/) | cdesai，Eamo5，npjohnson |
| 10. | [谷歌 Pixel 4 XL](https://forum.xda-developers.com/c/google-pixel-4-xl.9021/) | [珊瑚](https://wiki.lineageos.org/devices/coral/) | cdesai，Eamo5，npjohnson |
| 11. | [谷歌像素 4a](https://forum.xda-developers.com/c/google-pixel-4a.10249/) | [翻车鱼](https://wiki.lineageos.org/devices/sunfish/) | 克德赛·彼得克西 |
| 12. | [谷歌像素 4a 5G](https://forum.xda-developers.com/c/google-pixel-4a-5g.11321/) | [树莓](https://wiki.lineageos.org/devices/bramble/) | 阿莱斯托 |
| 13. | [谷歌像素 5](https://forum.xda-developers.com/c/google-pixel-5.11335/) | [redfin](https://wiki.lineageos.org/devices/redfin/) | 阿莱斯托 |
| 14. | [LeEco Le Max2](https://forum.xda-developers.com/c/leeco-le-max-2.5375/) | (T4) x2 (T5) | 曲名 : Tortel, ThemarD |
| 15. | [LeEco Pro3 / Pro3 Elite](https://forum.xda-developers.com/c/leeco-le-pro3.5922/) | [zl1](https://wiki.lineageos.org/devices/zl1/) | 作者 : Codeworkx, Mosimchah |
| 16. | [LG G2 (AT &T)](https://forum.xda-developers.com/f/at-t-lg-g2.3022/) | [d800](https://wiki.lineageos.org/devices/d800/) | 阿莱斯托 |
| 17. | [LG G2(加拿大)](https://forum.xda-developers.com/c/lg-g2.2456/) | [d803](https://wiki.lineageos.org/devices/d803/) | 阿莱斯托 |
| 18. | [LG G2 (国际版)](https://forum.xda-developers.com/c/lg-g2.2456/) | [d802](https://wiki.lineageos.org/devices/d802/) | 阿莱斯托 |
| 19. | [LG G2 (T-Mobile)](https://forum.xda-developers.com/f/t-mobile-lg-g2.3029/) | [d801](https://wiki.lineageos.org/devices/d801/) | 阿莱斯托 |
| 20. | [LG G5(国际版)](https://forum.xda-developers.com/c/lg-g5.5128/) | [h850](https://wiki.lineageos.org/devices/h850/) | aleasto, npjohnson, x86cpu |
| 21. | [LG G5 (T-Mobile)](https://forum.xda-developers.com/c/lg-g5.5128/) | [h830](https://wiki.lineageos.org/devices/h830/) | aleasto, npjohnson, x86cpu |
| 22. | LG G5(US Unlocked) | [rs988](https://wiki.lineageos.org/devices/rs988/) | aleasto, npjohnson, x86cpu |
| 23. | [LG V20 (AT &T)](https://forum.xda-developers.com/c/lg-v20.5871/) | (T40) H910 (T41) | aleasto, npjohnson, x86cpu |
| 24. | [LG V20(全球)](https://forum.xda-developers.com/c/lg-v20.5871/) | [H990(T45)](https://wiki.lineageos.org/devices/h990/) | aleasto, npjohnson, x86cpu |
| 25. | [LG V20(Sprint)](https://forum.xda-developers.com/c/lg-v20.5871/) | [ls997](https://wiki.lineageos.org/devices/ls997/) | aleasto, npjohnson, x86cpu |
| 26. | [LG V20(T-Mobile)](https://forum.xda-developers.com/c/lg-v20.5871/) | (T52) h918 (T53) | aleasto, npjohnson, x86cpu |
| 27. | LG V20 (US Unlocked) (T55) | [us996(T57)](https://wiki.lineageos.org/devices/us996/) | aleasto, npjohnson, x86cpu |
| 28. | LG V20 (Verizon) (T59) | [vs995(T61)](https://wiki.lineageos.org/devices/vs995/) | aleasto, npjohnson, x86cpu |
| 29. | 摩托罗拉 Moto G6 Plus (T63) | (T64) evert (T65) | 关于 Jleeblanch |
| 30. | 摩托罗拉 Moto G7 (T67) | (T68) 河(T69) | 作者 : Erfanoabdi, Npjohnson, SyberHexen |
| 31. | 摩托罗拉 Moto G7 Play (T71) | [频道(T73)](https://wiki.lineageos.org/devices/channel/) | 西碧尔森，死神 96385，Npjohnson 发明了 noabdi |
| 32. | [摩托罗拉摩托车 G7 Plus](https://forum.xda-developers.com/c/moto-g7-plus.8544/) | [湖](https://wiki.lineageos.org/devices/lake/) | jleeblanch，npjohnson |
| 33. | [摩托罗拉摩托车 G7 功率](https://forum.xda-developers.com/c/moto-g7-power.8537/) | [海洋](https://wiki.lineageos.org/devices/ocean/) | 西碧尔森，诺亚迪，Npjohnson |
| 34. | [摩托罗拉摩托车一号动力](https://forum.xda-developers.com/c/motorola-one-power.8159/) | [厨师](https://wiki.lineageos.org/devices/chef/) | rohan hasaabe(hasaaber 8) |
| 35. | [摩托罗拉摩托车 X4](https://forum.xda-developers.com/c/moto-x4.6912/) | [佩顿](https://wiki.lineageos.org/devices/payton/) | 泰晤士河 |
| 36. | [摩托罗拉摩托车 Z2 力](https://forum.xda-developers.com/c/moto-z2-force.6776/) | [nash](https://wiki.lineageos.org/devices/nash/) | npjohnson 发明的 no BDI |
| 37. | [摩托罗拉摩托车 Z3 播放](https://forum.xda-developers.com/c/moto-z3-play.7789/) | [贝克汉姆](https://wiki.lineageos.org/devices/beckham/) | jleeblanchh 先生 |
| 38. | [Nextbit Robin](https://forum.xda-developers.com/f/nextbit-robin.4914/) | [以太](https://wiki.lineageos.org/devices/ether/) | javelinanddart，npjohnson 公司 |
| 39. | [诺基亚 6.1 (2018)](https://forum.xda-developers.com/c/nokia-6-1-2018.7479/) | [PL2](https://wiki.lineageos.org/devices/PL2/) | npjohnson，自己的冲动 |
| 40. | [OnePlus One](https://forum.xda-developers.com/c/oneplus-one.3130/) | [培根](https://wiki.lineageos.org/devices/bacon/) | npjohnson 先生 |
| 41. | [OnePlus 3 / 3T](https://forum.xda-developers.com/f/oneplus-3-3t-cross-device-development.6157/) | [oneplus3](https://wiki.lineageos.org/devices/oneplus3/) | dianlujitao(地名) |
| 42. | [OnePlus 5](https://forum.xda-developers.com/c/oneplus-5.6480/) | [芝士汉堡](https://wiki.lineageos.org/devices/cheeseburger/) | -=伊甸园美剧 http://sfile . ydy . com =-荣誉出品本字幕仅供学习交流，严禁用于商业途径 |
| 43. | [OnePlus 5T](https://forum.xda-developers.com/c/oneplus-5t.7252/) | [倾销](https://wiki.lineageos.org/devices/dumpling/) | amartinz，codeworkx，trautamaki(西班牙语) |
| 44. | [OnePlus 8](https://forum.xda-developers.com/c/oneplus-8.10349/) | [方便面](https://wiki.lineageos.org/devices/instantnoodle/) | 超 NoOb(超 noob) |
| 45. | [OnePlus 8 Pro](https://forum.xda-developers.com/c/oneplus-one.3130/) | [方便面](https://wiki.lineageos.org/devices/instantnoodlep/) | npjohnson 先生 |
| 46. | [OnePlus 8T](https://forum.xda-developers.com/c/oneplus-8t.11579/) | [kebab](https://wiki.lineageos.org/devices/kebab/) | 卢克 1337 |
| 47. | [火箭电话](https://forum.xda-developers.com/c/razer-phone.7245/) | [谢丽尔](https://wiki.lineageos.org/devices/cheryl/) | 迈克约阿尼纳 javelinanddart |
| 48. | [三星 Galaxy S4 (SGH-I337)](https://forum.xda-developers.com/c/at-t-canadian-bell-rogers-telus-virgin-samsung.2257/) | [jtexttt](https://wiki.lineageos.org/devices/jflteatt/) | 弓，npjohnson，侧面 |
| 49. | [三星 Galaxy S4 (SCH-R970，SPH-L720)](https://forum.xda-developers.com/c/sprint-samsung-galaxy-s-4.2272/) | [jtf pr](https://wiki.lineageos.org/devices/jfltespr/) | 弓，npjohnson，侧面 |
| 50. | [三星 Galaxy S4 (SCH-I545)](https://forum.xda-developers.com/f/verizon-samsung-galaxy-s-4.2314/) | [【jfltezw】](https://wiki.lineageos.org/devices/jfltevzw/) | 弓，npjohnson，侧面 |
| 51. | [三星 Galaxy S4 (GT-I9505/G，SGH-I337M，SGH-M919)](https://forum.xda-developers.com/c/samsung-galaxy-s-4-i9500-i9505-i9505g-i9506.2162/) | [【jtextxx】](https://wiki.lineageos.org/devices/jfltexx) | 弓，npjohnson，侧面 |
| 52. | [三星 Galaxy S4 激活](https://forum.xda-developers.com/c/samsung-galaxy-s-4-active.2463/) | [吹牛](https://wiki.lineageos.org/devices/jactivelte/) | 弓，npjohnson，侧面 |
| 53. | [三星 galaxy S4 value edition(gt-I 9515/l)](https://forum.xda-developers.com/c/samsung-galaxy-s4-ve.7761/) | [已经停止](https://wiki.lineageos.org/devices/jfvelte/) | 弓，npjohnson，侧面 |
| 54. | [三星银河 Tab S5e (LTE)](https://forum.xda-developers.com/c/samsung-galaxy-tab-s5e.9164/) | [gts4lv](https://wiki.lineageos.org/devices/gts4lv/) | bgcngm，LuK1337 号文件 |
| 55. | [三星 Galaxy Tab S5e (Wi-Fi)](https://forum.xda-developers.com/c/samsung-galaxy-tab-s5e.9164/) | [gts4lvwifi](https://wiki.lineageos.org/devices/gts4lvwifi/) | luk 1337 bgcngm 公司 |
| 56. | [三星 Galaxy Tab S6 Lite (Wi-Fi)](https://forum.xda-developers.com/c/samsung-galaxy-tab-s6-lite.10969/) | [gta4xlwifi](https://wiki.lineageos.org/devices/gta4xlwifi/) | Linux4 |
| 57. | [索尼体验 10](https://forum.xda-developers.com/c/sony-xperia-10.8651/) | [麒麟](https://wiki.lineageos.org/devices/kirin/) | 卢克 1337 |
| 58. | [索尼体验 10 加](https://forum.xda-developers.com/c/sony-xperia-10-plus.8658/) | [女仆](https://wiki.lineageos.org/devices/mermaid/) | 卢克 1337 |
| 59. | [索尼体验 XA2](https://forum.xda-developers.com/c/sony-xperia-xa2.7890/) | [先驱](https://wiki.lineageos.org/devices/pioneer/) | LuK1337，严格，cdesai |
| 60. | xa 2 plus 体验 | [旅行](https://wiki.lineageos.org/devices/voyager/) | 卢克 1337 |
| 61. | [索尼体验 XA2 超](https://forum.xda-developers.com/c/sony-xa2-ultra.7523/) | [发现](https://wiki.lineageos.org/devices/discovery/) | 卢克 1337 |
| 62. | [小米 5](https://forum.xda-developers.com/c/xiaomi-mi-5.5189/) | [双子座](https://wiki.lineageos.org/devices/gemini/) | bgcngm、defer、h2o64 |
| 63. | [小米 5s 加](https://forum.xda-developers.com/c/xiaomi-mi-5s-plus.6281/) | [钠](https://wiki.lineageos.org/devices/natrium/) | 卢克 1337 |
| 64. | [小米 Mi 8](https://forum.xda-developers.com/c/xiaomi-mi-8.7845/) | [偶极子](https://wiki.lineageos.org/devices/dipper/) | 下述情况 |
| 65. | [小米 8 Lite](https://forum.xda-developers.com/c/xiaomi-mi-8-lite.8493/) | [铂](https://wiki.lineageos.org/devices/platina/) | 塞鲍本图 |
| 66. | [小米米 Mix](https://forum.xda-developers.com/c/xiaomi-mi-mix.5956/) | [锂](https://wiki.lineageos.org/devices/lithium/) | 布伦登巴里卡 011 号 |
| 67. | [小米米 Mix 2S](https://forum.xda-developers.com/c/xiaomi-mi-mix-2s.7602/) | [北极星](https://wiki.lineageos.org/devices/polaris/) | bgcngm |
| 68. | [小米 Mi Note 2](https://forum.xda-developers.com/c/xiaomi-mi-note-2.5950/) | [天蝎座](https://wiki.lineageos.org/devices/scorpio/) | LuK1337 |
| 69. | [小米 Poco F1](https://forum.xda-developers.com/c/xiaomi-poco-f1.8089/) | [铍](https://wiki.lineageos.org/devices/beryllium/) | bgcngm，warabhishek |
| 70. | [小米红米 7](https://forum.xda-developers.com/c/xiaomi-redmi-7.8777/) | [onclite](https://wiki.lineageos.org/devices/onclite/) | Dhina17 |

### 通用目标

随着 LineageOS 18.1 的推出，该团队还发布了另一项重大消息。Android 虚拟设备(AVD)，即 [Android Studio](https://www.xda-developers.com/install-android-studio-windows-macos-linux-chrome-os/) 提供的默认仿真器环境，现在是[官方支持的构建目标](https://wiki.lineageos.org/emulator.html)。也可以使用这些目标在移动和 Android 电视配置中构建 [GSI](https://www.xda-developers.com/unofficial-lineageos-18-0-gsi-android-11-project-treble/) ，尽管官方下载门户不会托管任何这样的预编译版本。尽管如此，这是项目向前迈出的关键一步，因为它清楚地表明了该团队推广自定义 ROM bringup 练习的承诺。

### 如果我的设备没有列在这里，该怎么办？

仅仅因为你的设备没有在这里列出，并不意味着你现在不能享受 LineageOS 18.1。由于它的开源性质，在我们的论坛上有许多设备的非官方版本，随着开发的进展，其中许多最终将成为官方版本。更重要的是:到目前为止，他们中的大多数都是非常稳定的日常司机，偶尔会有小毛病。

如果你想直接进入，查看这个索引，为你的设备寻找非官方的基于 Android 11 的 LineageOS 18.1 版本。然而，如果你害怕出错，那么等待官方版本的到来是明智的。

* * *

## 如何升级到 LineageOS 18.1

如果你不熟悉安装定制 rom 或修改手机的过程，在尝试做任何事情之前，你首先需要解锁设备的引导程序，并安装一个更新的定制恢复，如 LineageOS Recovery 或 [TWRP](https://www.xda-developers.com/how-to-install-twrp/) 。然后，一旦 LineageOS 18.1 版本可用于您的设备，您将需要通过自定义恢复环境安装它们。特定于设备的说明可能会有所不同，所以请提前查看相应的 wiki 页面。

至于谷歌应用程序，它们不会预装在 LineageOS 18.1 版本中。开放 Gapps 项目尚未提供 Android 11 Gapps，因此该团队建议您改为使用 [MindTheGapps 包](http://downloads.codefi.re/jdcteam/javelinanddart/gapps)。

* * *

## LineageOS 17.1 新设备和 LineageOS 16.0 的退役

虽然维护人员努力将设备升级到官方的 LineageOS 18.1，但你仍然可以找到基于 Android 10 的 LineageOS 17.1 仍然支持的一批设备的每周自动构建。到目前为止，一些设备已经获得了 LineageOS 17.1 的官方支持，而像红米 Note 7 这样的智能手机在退出一段时间后，重新获得了官方地位[。如果您有兴趣在这些设备上尝试定制 ROM，您现在可以通过点击各自 Wiki 页面上的“Get the builds here ”(链接如下)下载 recovery flashable 包。](https://www.xda-developers.com/lineageos-17-1-supports-nextbit-robin-moto-g5-moto-e5-plus-drops-galaxy-s9-note-9-redmi-note-7-oppo-find-7/)

### LineageOS 17.1 官方构建列表。点击/单击以展开。

| 

没有。

 | 

设备和论坛链接

 | 

设备代号和维基链接

 | 

维护者

 |
| --- | --- | --- | --- |
| 1. | [华硕 ROG 手机二代](https://forum.xda-developers.com/c/asus-rog-phone-ii.9056/) | [I001D](https://wiki.lineageos.org/devices/I001D/) | 奥登克里格 |
| 2. | [华硕 Zenfone 5Z (ZS620KL)](https://forum.xda-developers.com/c/asus-zenfone-5z.7546/) | [Z01R](https://wiki.lineageos.org/devices/Z01R/) | rohanpurohit，Jackeagle，ThEMarD |
| 3. | BQ Aquaris X | [巴多克](https://wiki.lineageos.org/devices/bardock/) | eloimuns，Quallenauge，团队 aquaris-dev |
| 4. | [BQ Aquaris X Pro](https://forum.xda-developers.com/c/bq-aquaris-x-pro-x2-x2-pro.7775/) | [巴多克普罗](https://wiki.lineageos.org/devices/bardockpro/) | Quallenauge，团队水族馆-开发 |
| 5. | 公平电话 3 | [FP3](https://wiki.lineageos.org/devices/FP3/) | dk1978 |
| 6. | [谷歌像素](https://forum.xda-developers.com/c/google-pixel.5910/) | [旗鱼](https://wiki.lineageos.org/devices/sailfish/) | 采访，razorloves |
| 7. | [谷歌 Pixel XL](https://forum.xda-developers.com/c/google-pixel-xl.5916/) | [马林](https://wiki.lineageos.org/devices/marlin/) | 采访，razorloves |
| 8. | [谷歌像素 3](https://forum.xda-developers.com/c/google-pixel-3.8236/) | 蓝线 | cdesai、intervigil、razorloves |
| 9. | [谷歌像素 3 XL](https://forum.xda-developers.com/c/google-pixel-3-xl.8243/) | [交叉剖面线](https://wiki.lineageos.org/devices/crosshatch/) | cdesai、intervigil、razorloves |
| 10. | [华为荣誉 5X](https://forum.xda-developers.com/c/honor-5x.5021/) | [猕猴桃](https://wiki.lineageos.org/devices/kiwi/) | BadDaemon(守护进程) |
| 11. | [LeEco Le 2](https://forum.xda-developers.com/c/leeco-le-2.5630/) | [s2](https://wiki.lineageos.org/devices/s2/) | codeworkx，timibreakdown |
| 12. | [联想 P2](https://forum.xda-developers.com/c/lenovo-p2.6149/) | [昆陶](https://wiki.lineageos.org/devices/kuntao/) | mikeioannina，高速公路司机 |
| 13. | [LG G3(冲刺)](https://forum.xda-developers.com/f/sprint-lg-g3.3374/) | [ls990](https://wiki.lineageos.org/devices/ls990/) | 水母，水彩-dev 小组 |
| 14. | [摩托罗拉边](https://forum.xda-developers.com/c/bq-aquaris-x-pro-x2-x2-pro.7775/) | [快手](https://wiki.lineageos.org/devices/racer/) | 发明了努巴迪，jleeblanch，syberhexen |
| 15. | [摩托罗拉摩托车和 2015 LTE](https://forum.xda-developers.com/c/moto-e-2015.4071/) | [耳聋](https://wiki.lineageos.org/devices/surnia/) | 木尔夫利，自己的推波助澜，自己的推波助澜，自己的推波助澜，自己的推波助澜，自己的推波助澜，自己的推波助澜，自己的推波助澜，自己的推波助澜 |
| 16. | 摩托罗拉摩托车 E5 Plus (XT1924-3/9) | [【ahannah】](https://wiki.lineageos.org/devices/ahannah/) | Jarl-Penguin，karthick111，electimon，wh0dat .你好，我是 jarl-penguin，kart hick 111，electimon，wh 0dat |
| 17. | 摩托罗拉摩托车 E5 Plus (XT1924-6/7/8) | [汉娜](https://wiki.lineageos.org/devices/hannah/) | Jarl-Penguin，karthick111，electimon，wh0dat .你好，我是 jarl-penguin，kart hick 111，electimon，wh 0dat |
| 18. | 摩托罗拉摩托车 E5 Plus (1924-1/2/4/5) | [雷纳纳](https://wiki.lineageos.org/devices/rhannah/) | Jarl-Penguin，karthick111，electimon，wh0dat .你好，我是 jarl-penguin，kart hick 111，electimon，wh 0dat |
| 19. | [摩托罗拉摩托车 G 2015](https://forum.xda-developers.com/c/moto-g-2015.4379/) | [奥斯巴](https://wiki.lineageos.org/devices/osprey/) | 木法夫利，360 磅 |
| 20. | [摩托罗拉摩托车 G3 涡轮](https://forum.xda-developers.com/c/moto-g-2015.4379/) | [梅林](https://wiki.lineageos.org/devices/merlin/) | 木法夫利 |
| 21. | [摩托罗拉摩托车 G4 比赛](https://forum.xda-developers.com/c/moto-g4-play.5569/) | [竖琴](https://wiki.lineageos.org/devices/harpia/) | 1979 年 jro |
| 22. | [摩托罗拉摩托车 G5](https://forum.xda-developers.com/c/moto-g5.6203/) | [塞德里克](https://wiki.lineageos.org/devices/cedric/) | Jarl 企鹅队 |
| 23. | [摩托罗拉摩托车 G5S](https://forum.xda-developers.com/c/moto-g5s.6804/) | [蒙大拿州](https://wiki.lineageos.org/devices/montana/) | Jarl 企鹅 wiktorek140 |
| 24. | [摩托罗拉摩托车 X 2014](https://forum.xda-developers.com/c/moto-x-2014.3586/) | [胜利](https://wiki.lineageos.org/devices/victara/) | 1979 年，林肯郡，npjohnson |
| 25. | [摩托罗拉摩托车 x 播放](https://forum.xda-developers.com/c/moto-x-play.4372/) | [力士](https://wiki.lineageos.org/devices/lux/) | 水母，水彩-dev 小组 |
| 26. | [z17 云团](https://forum.xda-developers.com/c/zte-nubia-z17.6510/) | [nx563j](https://wiki.lineageos.org/devices/nx563j/) | 贝克尔克 |
| 27. | [OnePlus 2](https://forum.xda-developers.com/c/oneplus-2.4305/) | [oneplus2](https://wiki.lineageos.org/devices/oneplus2/) | ozzyscmacc，aviraxp |
| 28. | [OnePlus 7](https://forum.xda-developers.com/c/oneplus-7.8833/) | [鳄梨酱](https://wiki.lineageos.org/devices/guacamoleb/) | 阿什温 RC |
| 29. | [OnePlus 7T Pro](https://forum.xda-developers.com/c/oneplus-7t-pro.9327/) | [热狗](https://wiki.lineageos.org/devices/hotdog/) | 卢克 1337 |
| 30. | [【one plus north】](https://forum.xda-developers.com/c/oneplus-nord.11081/) | [飞机](https://wiki.lineageos.org/devices/avicii/) | 卡卡卡卡拉卡斯海 |
| 31. | [Realme 2 Pro](https://forum.xda-developers.com/c/realme-2-pro.8399/) | [RMX1801](https://wiki.lineageos.org/devices/RMX1801/) | S7-1200 可编程控制器 |
| 32. | [三星 Galaxy A3 (2016)](https://forum.xda-developers.com/c/samsung-galaxy-a-series.4853/) | [至 3xelte](https://wiki.lineageos.org/devices/a3xelte/) | 丹伍德 76 号，严格 |
| 33. | [三星 Galaxy A5 (2016)](https://forum.xda-developers.com/c/samsung-galaxy-a-series.4853/) | [至 5xelte](https://wiki.lineageos.org/devices/a5xelte/) | 丹伍德 76 号，严格 |
| 34. | [三星 Galaxy A5 (2017)](https://forum.xda-developers.com/c/samsung-galaxy-a-series-2017.6083/) | [a5 和 17lte](https://wiki.lineageos.org/devices/a5y17lte/) | 分支机构 |
| 35. | [三星 Galaxy A7 (2016)](https://forum.xda-developers.com/c/samsung-galaxy-a-series.4853/) | [至 7xelte](https://wiki.lineageos.org/devices/a7xelte/) | 苏拉吉克丹伍德 76 号严格 |
| 36. | [三星 Galaxy A7 (2017)](https://forum.xda-developers.com/c/samsung-galaxy-a-series-2017.6083/) | [至 7e 17lte](https://wiki.lineageos.org/devices/a7y17lte/) | 分支机构 |
| 37. | [三星 Galaxy J7 (2015)](https://forum.xda-developers.com/c/samsung-galaxy-j7.5263/) | [j7elte](https://wiki.lineageos.org/devices/j7elte/) | 达里奥姆伯，丹伍德 76 号，严格 |
| 38. | [三星银河笔记 3 LTE (N9005/P)](https://forum.xda-developers.com/c/samsung-galaxy-note-3.2492/) | [选择](https://wiki.lineageos.org/devices/hlte/) | 哈格特，npjohnson |
| 39. | [三星银河笔记 3 LTE (N9008V)](https://forum.xda-developers.com/c/samsung-galaxy-note-3.2492/) | [hltechn](https://wiki.lineageos.org/devices/hltechn/) | 哈格特，npjohnson |
| 40. | [三星银河笔记 3 LTE (N900K/L/S)](https://forum.xda-developers.com/c/samsung-galaxy-note-3.2492/) | [hltekor](https://wiki.lineageos.org/devices/hltekor/) | 哈格特，npjohnson |
| 41. | [三星银河笔记 3 LTE (N900T/V/W8)](https://forum.xda-developers.com/f/t-mobile-samsung-galaxy-note-3.2561/) | [hltetmo](https://wiki.lineageos.org/devices/hltetmo/) | 哈格特，npjohnson |
| 42. | [三星 Galaxy S III Neo(双 SIM)](https://forum.xda-developers.com/c/samsung-galaxy-s3-neo.3727/) | [s3ve3gds](https://wiki.lineageos.org/devices/s3ve3gds/) | 皮顿有限公司，fcuzzocrea，Teledurak |
| 43. | [Samsung Galaxy S III Neo (Samsung Camera)](https://forum.xda-developers.com/c/samsung-galaxy-s3-neo.3727/) | [s3ve3gjv](https://wiki.lineageos.org/devices/s3ve3gjv/) | PythonLimited,fcuzzocrea,Teledurak |
| 44. | [Samsung Galaxy S III Neo (Sony Camera)](https://forum.xda-developers.com/c/samsung-galaxy-s3-neo.3727/) | [s3ve3gxx](https://wiki.lineageos.org/devices/s3ve3gxx/) | PythonLimited,fcuzzocrea,Teledurak |
| 45. | [Samsung Galaxy S5 Neo (T9)](https://forum.xda-developers.com/c/samsung-galaxy-s5-neo.6571/) | [s5neolte](https://wiki.lineageos.org/devices/s5neolte/) | danwood76, 严格 |
| 46. | 三星 Galaxy S5 Active (G870F) | [klteactivexx (T13)](https://wiki.lineageos.org/devices/klteactivexx/) | 作者 javelinanddart, npjohnson |
| 47. | [Samsung Galaxy S5 LTE (G9006V/8V)](https://forum.xda-developers.com/c/samsung-galaxy-s-5.2792/) | (T16) kltechn (T17) | 饰 Haggertk |
| 48. | 三星 Galaxy S5 LTE(G900F/M/R4/R7/T/V/W8) | [klte](https://wiki.lineageos.org/devices/klte/) | 饰 Haggertk |
| 49. | [Samsung Galaxy S5 LTE (G900I/P)](https://forum.xda-developers.com/c/samsung-galaxy-s-5.2792/) | [kltedv (T25)](https://wiki.lineageos.org/devices/kltedv/) | 饰 Haggertk |
| 50. | [Samsung Galaxy S5 LTE (G900K/L/S)](https://forum.xda-developers.com/c/samsung-galaxy-s-5.2792/) | [kltekor (T29)](https://wiki.lineageos.org/devices/kltekor/) | 饰 Haggertk |
| 51. | 三星 Galaxy S5 LTE (SC-04F/SCL23) | (T32) kltekdi (T33) | 饰 Haggertk |
| 52. | 三星 Galaxy S5 LTE Duos(G9006W/8W) | (T36) kltechnduo (T37) | 饰 Haggertk |
| 53. | 三星 Galaxy S5 LTE Duos(G900FD/MD) | (T40) klteduos (T41) | 饰 Haggertk |
| 54. | 索尼 Xperia XZ2 (T43) | (T44) akari (T45) | olivier97, sjllls |
| 55. | 索尼 Xperia XZ2 Compact (T47) | [xz2c](https://wiki.lineageos.org/devices/xz2c/) | olivier97, sjllls |
| 56. | 索尼 Xperia Z3 (T51) | (T52) z3 (T53) | Tom1000, Myself5 |
| 57. | 索尼 Xperia Z3 Compact (T55) | [z3c](https://wiki.lineageos.org/devices/z3c/) | 阿里安 K16a |
| 58. | 索尼 Xperia Tablet Z2 LTE (T59) | [海狸(T61)](https://wiki.lineageos.org/devices/castor/) | SNC |
| 59. | (T62) Wileyfox Swift(T63) | [爆裂声](https://wiki.lineageos.org/devices/crackling/) | 115ek |
| 60. | [永泰红米 2](https://forum.xda-developers.com/c/xiaomi-redmi-2.5103/) | [wt88047](https://wiki.lineageos.org/devices/wt88047/) | nicknitewolf |
| 61. | [小米米 6X](https://forum.xda-developers.com/c/xiaomi-mi-a2-mi-6x.7963/) | [韦恩](https://wiki.lineageos.org/devices/wayne/) | 艾萨克·陈 |
| 62. | [小米米 A1](https://forum.xda-developers.com/c/xiaomi-mi-a1.7044/) | [天梭](https://wiki.lineageos.org/devices/tissot/) | abhinavgupta371 |
| 63. | [小米米 A2](https://forum.xda-developers.com/c/xiaomi-mi-a2-mi-6x.7963/) | [茉莉 _ 萌芽](https://wiki.lineageos.org/devices/jasmine_sprout/) | 米哈伊尔·奥尼娜 |
| 64. | [小米米 Note 3](https://forum.xda-developers.com/c/xiaomi-mi-note-3.7428/) | 杰森 | 电路集陶 |
| 65. | [小米红米 K20 /米 9T](https://forum.xda-developers.com/c/redmi-k20-xiaomi-mi-9t.8946/) | [达芬奇](https://wiki.lineageos.org/devices/davinci/) | 猪 |
| 66. | [小米红米 Note 5 Pro](https://forum.xda-developers.com/c/xiaomi-redmi-note-5-pro.7419/) | 为什么红色的 | 塞鲍本图·斯法里亚斯 |
| 67. | [小米红米 Note 6 Pro](https://forum.xda-developers.com/c/xiaomi-redmi-note-6-pro.8406/) | [两唇](https://wiki.lineageos.org/devices/twolip/) | DD3Boh |
| 68. | [小米红米 Note 7](https://forum.xda-developers.com/c/xiaomi-redmi-note-7.8500/) | [薰衣草](https://wiki.lineageos.org/devices/lavender/) | UltraGamerHD |
| 69. | [小米红米 Note 8 / 8T](https://forum.xda-developers.com/c/redmi-note-8.9200/) | [银杏](https://wiki.lineageos.org/devices/ginkgo/) | 黑暗骑士 360 |
| 70. | Yandex 电话 | [琥珀](https://wiki.lineageos.org/devices/Amber/) | 高速之星，vm03 |

随着基于 Android 11 的官方构建的发布，LineageOS 16.0 构建角色将正式终止。事实上，自 2021 年 2 月 15 日起，基于 Android 9 Pie 的官方 16.0 版本将不再发布。然而，现有的 16.0 分支将继续对像安全补丁这样的贡献开放，开发者仍然可以构建新的、非官方的 16.0 版本。如果你对定制 ROM 开发并不陌生，并且你想提交这些设备中的一个以获得官方支持，你可以[遵循这里的说明](https://wiki.lineageos.org/submitting_device.html)。

在此过渡阶段停产的设备的完整列表如下:

### 淘汰的 linegeos 16.0/17.1 设备列表。点击/单击以展开。

## 从 LineageOS 16.0 名册中弃用:

## 从 LineageOS 17.1 名册中弃用:

* * *

## 支撑线

LineageOS 是一个由几个开发人员在业余时间开发的社区项目，不依赖任何商业模式。如果你想支持开发团队，你可以在 PayPal 上向他们捐款，这将有助于服务器成本。如果你想看最新的新闻或者和一些维护者交流，你也应该在 Twitter 或者他们的官方子网站上关注他们。要提交错误报告，请参见此处的。如果你想帮助团队将定制的 ROM 翻译成你的语言，你可以按照这里的[的指示来做。](https://wiki.lineageos.org/translate-howto.html)

**在社交媒体上关注 linegeos**

**捐赠给 linegeos**

*   通过 [PayPal](https://paypal.me/LineageOS) 向 LineageOS 捐款

*特色图片鸣谢:阿什·西蒙斯([瓦兹加德](https://forum.xda-developers.com/m/vazguard.784627/) )*