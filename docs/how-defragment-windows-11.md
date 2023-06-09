# 如何在 Windows 11 上整理或修剪您的驱动器

> 原文：<https://www.xda-developers.com/how-defragment-windows-11/>

使用电脑的时间越长，速度就越有可能变慢，尤其是当你在硬盘上堆积了越多的文件时。填满硬盘会显著降低性能，解决这个问题的一个好方法是优化或整理硬盘。在本文中，我们将向您展示如何整理 Windows 11 PC 上的驱动器。

## 什么是碎片整理？

碎片整理意味着 Windows 将搜索物理驱动器不同部分的文件，并将这些文件放在同一个区域，使计算机更容易顺序读取它们。这对硬盘驱动器(HDD)有很大的影响，因为如果旋转的盘片分散在整个驱动器中，它们需要更长的时间来定位文件的不同部分。

然而，这些天你可能不会看到很多关于碎片整理的内容。这是因为今天大多数电脑都配备了固态硬盘(SSD)或 eMMC 存储，其工作方式在文件访问方面非常不同。现在，访问驱动器的不同部分不再需要更多时间，并且碎片整理实际上可能会对 SSD 的寿命产生不利影响，因为它会占用更多的写入周期，这在这种驱动器上是有限的。这曾经是寿命特别短的早期固态硬盘的一个更大的问题，但即使在今天，对固态硬盘进行碎片整理也没有任何好处。

相反， [Windows 11](http://www.xda-developers.com/windows-11/) 通过一种叫做微调的方式来优化固态硬盘。这将驱动器中未使用的部分标记为可供使用，以便在需要时更快地向该段写入新数据。

## 如何整理和优化你的驱动器

整理或优化你的驱动器最简单的方法是使用 Windows 11 中内置的磁盘优化工具。该工具根据您使用的是固态硬盘还是硬盘，自动整理或优化您的硬盘。这是最好的方法，因为它避免了碎片整理磨损固态硬盘。

1.  打开开始菜单，输入**整理**。第一个结果应该是**整理碎片并优化驱动器。**选择它。
2.  选择要优化或整理碎片的驱动器。
3.  点击**分析**检查硬盘是否需要优化或碎片整理。
4.  如果是，点击**优化**。
5.  这个过程可能需要一段时间。如果您正在整理外置驱动器的碎片，请确保它一直插在电源上，直到该过程完成。

## 如何安排驱动器优化

这是所有你需要做的整理你的驱动器一次。但是，您也可以计划定期运行优化。默认为您的 PC 上的内部驱动器设置每周碎片整理计划。如果你想改变这种情况，请遵循以下步骤。

1.  再次打开**碎片整理和优化驱动器**窗口。
2.  点击**日程优化**下的**更改设置**。
3.  如果还没有选中**按计划运行(推荐)**复选框，请将其选中。
4.  您可以将优化频率更改为**每日**、**每周**或**每月**。
5.  点击**选择**选择您希望作为计划优化一部分的驱动器。
6.  您可以选择要优化的驱动器，以及是否希望自动优化新驱动器。
7.  点击**确定**，然后再次点击**确定**保存您的设置。

这就是你需要做的整理你的硬盘的时间表。这绝对是最简单的方法，但还有其他方法。

## 使用命令提示符整理您的驱动器

如果您更愿意使用命令提示符来运行磁盘碎片整理，也可以这样做。但是，请注意，如果是 SSD，这种方法仍然会对您的驱动器进行碎片整理，这是您不想要的。

如果您有硬盘，只需遵循以下步骤。

1.  在开始菜单中搜索 **cmd** ，在**命令提示符下选择**以管理员身份运行**。**
2.  键入**Defrag[驱动器号]** ，用分配给要进行碎片整理的驱动器的盘符替换**[驱动器号]** 。对于您的操作系统驱动器，应该是 C:，所以命令应该是 **Defrag C:**
3.  等待该过程完成，这可能需要一段时间。

如果你想通过调整来优化固态硬盘，你必须使用一个特定的命令。按照上面的解释打开命令提示符，然后输入命令 **Defrag【盘符】/L** 。 **/L** 参数指定您想要重新整理驱动器，这对 SSD 更有意义。

对于不同种类的优化和任务， **Defrag** 命令可以使用许多额外的参数。例如，添加 **/A** 参数可以让您分析驱动器以查看它是否需要优化，而 **/B** 参数可以让您优化引导性能。

* * *

这就是你在 Windows 11 上整理硬盘碎片所需要知道的全部内容。这有助于提高你的[神奇的 PC](https://www.xda-developers.com/best-laptops/) 的性能，尤其是如果你已经用了很长时间的话。然而，Windows 11 已经默认优化了你的驱动器，所以你不需要经常遵循这些步骤。

如果您想了解更多有关节省空间或提高电脑性能的其他方法，您也可以查看[如何清除电脑上的缓存](https://www.xda-developers.com/how-clear-cache-windows-11/)和临时文件。你也可以阅读[如何清除你的电脑的 DNS 缓存](https://www.xda-developers.com/how-clear-dns-windows-11/)，这可以帮助解决一些互联网连接问题。