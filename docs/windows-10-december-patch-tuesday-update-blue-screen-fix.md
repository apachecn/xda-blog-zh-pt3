# 最新的 Windows 10 更新可能会导致启动时出现蓝屏，但有一个修复方法

> 原文：<https://www.xda-developers.com/windows-10-december-patch-tuesday-update-blue-screen-fix/>

如果你仍然在电脑上运行 Windows 10，并且安装了最新的更新，标签为 [KB5021233](https://support.microsoft.com/en-us/topic/december-13-2022-kb5021233-os-builds-19042-2364-19043-2364-19044-2364-and-19045-2364-44e774aa-60c4-4e38-b7e7-c886d210db3b) ，并于 12 月 13 日发布，你可能会遇到一个问题，即你的电脑启动后直接进入蓝屏崩溃。如果是这样，不用担心(太过分)，你不是一个人。微软已经正式承认此更新存在问题，并将该问题添加到其发布健康仪表板，以及如何解决该问题的步骤。

据微软称，出现该问题是因为 Windows 安装所在磁盘的 **Windows/system32** 和 **Windows/system32/drivers** 文件夹中存储的一个名为 **hidparse.sys** 的文件版本可能存在差异。这会导致签名验证失败，这意味着电脑无法启动。

谢天谢地，这个问题不用重新安装操作系统或类似的东西就可以解决。您首先需要启动到 Windows 恢复环境(WinRE)，这应该会在您的设备几次无法正确启动后自动发生。从这里开始，遵循以下步骤:

1.  点击**故障排除**，然后**启动恢复、故障排除和诊断工具**。
2.  选择**高级选项**，然后选择**命令提示**。这将重启你的设备进入命令行界面。
3.  看到命令提示符窗口后，输入以下命令(如果 Windows 安装在不同的驱动器上，您可能需要将驱动器号从 C 更改为其他值):

    ```
    xcopy C:\windows\system32\drivers\hidparse.sys C:\windows\system32\hidparse.sys
    ```

    这将把文件从一个文件夹复制到另一个文件夹，确保两个位置具有相同的版本。
4.  键入 **exit** 并按 Enter 键关闭命令提示符窗口并重启计算机。
5.  点击**继续**，你的电脑应该会正常启动进入 Windows。

如果你以前从未做过，遵循这些步骤可能看起来有点痛苦，但这实际上是一个相当无痛的过程，你不必丢失任何数据或等待太长时间才能让你的电脑恢复运行。一旦你做到了这一点，你应该可以走了。尽管如此，微软应该会在即将到来的更新中解决这个问题，但这可能只会在 1 月份发生，因为我们正处于假期季节的中期，12 月下半月没有可选的更新。

没有这样的问题影响 [Windows 11](https://www.xda-developers.com/windows-11/) ，所以如果你有这个版本，你不应该有任何担心。

* * *

**来源:** [微软](https://learn.microsoft.com/en-us/windows/release-health/status-windows-10-22h2#2986msgdesc)