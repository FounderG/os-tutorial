os-tutorial
============

如何从头开始建立一个操作系统！

我总是想去学习如何从头开始创建一个操作系统。在大学里我学习了如何实现高级功能（分区、信号、内存管理等等），但是：
- 我从未从我的引导扇区从头开始操作过
- 大学里学习的东西都很难所以其中大部分东西我都不记得了
- 我已经厌倦了那些认为阅读一个已经有的操作系统内核去学习操作系统的人的这种想法，哪怕是一个很小的内核。

受到这个[文档](http://www.cs.bham.ac.uk/~exr/lectures/opsys/10_11/lectures/os-dev.pdf)和这个[OSDev wiki](http://wiki.osdev.org/)的启发，我尝试去给所有关注这个项目的人做一个步骤式的指导文档和代码案例。实话说，这个指南基本上是一个初期的文档的但是它被分成了很多小的部分同时也不带有任何的理论。

更新：更多的资源：[the little book about OS development](https://littleosbook.github.io)，[JamesM's kernel development tutorials](https://web.archive.org/web/20160412174753/http://www.jamesmolloy.co.uk/tutorial_html/index.html)

特点
=============
- 这个课程呢是一个代码的教程，其目标人群是那些不希望有太高的计算机水平，比如说，对于操作系统的工作方式感到好奇但是没有时间或者毅力去开始完整阅读Linux内核的人程序员。
- 理论话题很少，这正是这个课程的特点之一，谷歌就是你的理论知识老师，一旦你从大学毕业了，过多的的理论知识比没有理论更糟糕因为它会使得事情感觉上比实际情况更复杂。
- 每一节课程都很短小，大概花费5-15分钟就可以完成。相信我同时也相信自己，你可以做到！

如何使用这个教程
=============
1. 从最开始的文件夹一步步向下走。他们都建立在之前的代码上所以如果你跳跃到第五个文件夹又不知道为什么这里会有一个`mov ah, 0x0e`，这就是因为你错过了课程2。所以真的，按照顺序去学习，你可以选择跳过那些你已经知道的东西。
2. 打开每一个README文档然后阅读第一行字，这里呢给出了一些你需要在阅读之前熟悉的概念，如果有你不熟悉的概念，谷歌一下。第二行字说明了课程的目标，阅读它因为它解释了我们在干什么，“为什么”往往比“怎么做”更重要。
3. 阅读剩下的README文档，**它非常清晰易懂**。
4. （可选）尝试在阅读完README文档后自己写一下代码。
5. 看那些代码示例，他们都做了很好的注释。
6. （可选）尝试运行这些代码示例，尝试去中断它们，确认你搞懂了代码的方式就是去中断它们或者是用其他的命令来复制它们的效果。

综上所述：先阅读README文档，再看那些代码文件，如果你足够勇敢的话，尝试自己编写这些代码。

规划
=============
我们可以用我们的操作系统做很多事情：

- 从头开始启动，不依赖GRUB -可以！
- 进入32位模式 -可以！
- 从汇编语言跳到C语言 -可以！
- 中断处理 -可以！
- 显示和键盘输入 -可以！
- 一个可以随着你需求扩充的微型的、基础的`libc` -可以！
- 内存管理 -可以！
- 写一个文件系统去储存文件 -可以！
- 创造一个很简单的shell壳程序 -可以！
- 用户模式 -可以！
- 也许我们还能写一个简单的文本编辑器 -可以！
- 多进程和进程调度 -可以！

我们可能会按照这个顺序进行，这一会儿会讲到。

如果我们足够有斗志，我们还可以做到：

- 一个BASIC语言解释器，就像在70年代一样！
- 一个图形界面
- 网络功能

贡献
================
这是一个个人学习用的项目，尽管这个项目已经很长时间没有更新了，我仍然会被希望在某些时间点可以重新参与。

我非常感谢那些指出bug以及提交requests的人，我需要时间去review这些内容但是我现在不能保证这个时间。

如果你想fork这个repo，请随意。如果有人有兴趣继续进行这个项目，请让我知道我会把“主fork”链接在这里。