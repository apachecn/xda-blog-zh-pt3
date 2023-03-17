# 如何备份和恢复 Linux (WSL)发行版的 Windows 子系统

> 原文：<https://www.xda-developers.com/how-back-up-restore-wsl/>

定期备份电脑是明智之举。无论你使用的是 Windows、Mac、Linux 还是 Chrome 操作系统，你都要非常小心。这同样适用于[Linux(WSL)](https://www.xda-developers.com/how-to-install-wsl-2-windows/)的 Windows 子系统，它运行在 Windows 之上，但有点独立于 Windows。

WSL 实例很容易设置，但是如果没有备份，如果出现问题，您将不得不手动重做一切。WSL 备份也是在机器之间转移环境的一种简单方法。

幸运的是，在 WSL 上备份 Linux 发行版是一个非常简单的过程，如果需要的话还可以恢复它。

## 如何备份 Linux (WSL)发行版的 Windows 子系统

由于 WSL 不是运行在裸机上的 Linux，我们不需要在发行版内部做任何事情来启动备份。相反，该操作完全从 PowerShell 运行。你需要做的是:

1.  在 PowerShell 配置文件中打开 Windows 终端(这应该是默认行为)。
2.  在 PowerShell 中运行命令 **wsl -l -v** 来打印所有当前安装的 Linux 发行版的列表。知道**确切的**名称来创建备份很重要。例如，你可能有 **Ubuntu-22.04** 而不仅仅是 Ubuntu。
3.  选择要保存备份的目录。在 PowerShell 窗口中，输入 **cd(目录)**，将**(目录)**替换为您想要存储备份文件的路径。例如，我们在我们的**文档**库中选择一个名为 **WSL backups** 的文件夹，所以我们将输入这个命令:

    ```
    cd "C:\Users\joaoc\Documents\WSL backups"
    ```

4.  输入以下命令来导出发行版:

    ```
     wsl --export (distribution) (filename.tar) 
    ```

5.  或者，您可以在导出过程中指定文件位置和文件名，而不是使用 **cd** 进入正确的目录。比如:

    ```
     wsl --export Ubuntu C:\Users\joaoc\Documents\WSL backups\Ubuntubackup.tar 
    ```

这就是备份过程。您现在创建的文件既可以在同一台 PC 上使用，也可以在另一台 PC 上使用，来创建您的 Linux 发行版的精确副本。您可以使用 Powershell 中的 import 命令来完成此操作。

## 如何从备份中导入 WSL 发行版

如果您正在导出您的 Linux 发行版，您可能希望在某个时候恢复它。在 WSL 中，这是使用 import 命令完成的。如果您在同一台 PC 上使用它，我们假设您已经使用了**-degree register**命令来删除您当前的实例。如果你仍然安装了它，从备份导入不会覆盖，使用相同的发行版名称会产生冲突。

它比 export 命令长一点，因为您需要指定它的安装位置以及要使用的文件。导入命令遵循以下模板:

```
 wsl --import (distribution) (install location) (file path) 
```

因此，使用上面第 5 步中的示例导出，您将得到如下结果:

```
 wsl --import Ubuntu c:\wsl c:\users\richard\desktop\ubuntumay27.tar 
```

过一会儿，你的发行版就安装好了，可以运行了。使用导出和导入的好处在于，您可以在很短的时间内在多台机器上设置相同的环境。您的用户和密码将被保留，就像您通过软件包管理器安装的任何东西一样。

如果你想在关闭 PowerShell 窗口之前确认它安装正确，只需再次运行 **wsl -l -v** ，你应该会看到新导入的发行版。