# [更新:修复] Nvidia 最新的 GeForce 游戏就绪驱动程序包含一个错误，使其有点占用 CPU

> 原文：<https://www.xda-developers.com/nvidia-geforce-game-ready-driver-cpu-bug/>

### 更新:美国东部时间 2023 年 3 月 7 日 12:14 TIMI·坎蒂萨诺

***固定不变。***

已经发布了修复该问题的新修补程序，现在可以下载。我们已经在源代码中链接了驱动程序下载。

大约一周前，Nvidia 发布了一个新的 [GeForce 游戏就绪驱动程序](https://www.xda-developers.com/nvidia-geforce-rtx-gpus-video-super-resolution-available/)，提供了广泛的增强功能，但更重要的是，提供了 RTX 视频超分辨率，这是一个新功能，当与 GeForce RTX 30 或 40 系列 GPU 配合使用时，可以改善使用谷歌 Chrome 或微软 Edge 传输的视频。虽然新的更新有一些问题，但在某些情况下，似乎有一个问题甚至会吃掉一些宝贵的 CPU，一些用户报告说这个数字高达 14%。

如果你已经安装了 GeForce Game Ready 驱动程序版本 531.18，那么你可能会注意到在过去的一周中 CPU 的使用有所增加。这是因为驱动程序中有一个错误，导致退出游戏后可能会出现额外的 CPU 使用率。The Verge [的 Tom Warren 也声称](https://twitter.com/tomwarren/status/1632680688968138752)当登录电脑时也会出现这个问题。虽然[官方反馈线程](https://www.nvidia.com/en-us/geforce/forums/game-ready-drivers/13/512048/geforce-grd-53118-feedback-thread-released-22823/)没有具体说明人们可以预期多少额外的 CPU 使用率，但许多用户都加入了进来，给出了从 10%到 10%以上的范围。

当然，像这样的事情可以等到新的驱动程序发布，或者你也可以回滚到旧的驱动程序。当然，如果您回滚，您将会失去最新更新中发布的特性。但在这种情况下，妥协可能是一个好主意，因为当涉及到 PC 性能时，至少损失 10%的 CPU 可能会是一个相当大的打击。此外，最新的驱动程序确实存在其他问题，如在非原生分辨率下切换 HDR 时的稳定性问题，启用 DSR/DLDSR 时的显示器闪烁，游戏问题，如*看门狗 2* 和*光环战争 2* 等。

如果你还没有更新，推迟可能是个好主意。不幸的是，虽然司机通常可以增强体验，但有时也可能在这个过程中破坏东西。在这种情况下，这是一件大事，尤其是对于那些试图最大限度地提高电脑性能的人来说。

* * *

**来源** : [Nvidia](https://www.nvidia.com/en-us/geforce/forums/game-ready-drivers/13/512048/geforce-grd-53118-feedback-thread-released-22823/) ，[补丁下载](https://nvidia.custhelp.com/app/answers/detail/a_id/5450/kw/hotfix)

**Via** : [汤姆·沃伦](https://twitter.com/tomwarren/status/1632680688968138752)(推特)