*上手前你可能需要Google一下的概念：linux，mac，terminal，compiler，emulator，nasm，qemu*

**目标：安装这份教程需要的软件**

我是用Mac工作的，用Linux其实会更好因为它已经把所有标准化的工具给你安装好了。

在Mac上，[安装 HomeBrew](http://brew.sh) 然后再使用命令 `brew install qemu nasm`

如果你安装了Xcode开发者工具中的`nasm`不要使用它，大多数情况下不是很好使。一直使用`/usr/local/bin/nasm`下的nasm比较好。

在有些系统上qemu会被分割成很多的二进制文件，你可以通过`qemu-system-x86_64 binfile`来使用。

前面提到的需要看一下的概念
=============================
**emulator:**

> In computing, an emulator is hardware or software that enables one computer system (called the host) to behave like another computer system (called the guest). An emulator typically enables the host system to run software or use peripheral devices designed for the guest system. Emulation refers to the ability of a computer program in an electronic device to emulate (or imitate) another program or device. 

在计算领域，模拟器指的是一种可以使得一种计算机系统（称之为主机）去模拟另外一个计算机系统（称之为客户机）行为的硬件或者是软件。一个典型的模拟器可以使得主机能够使用为客户机设计的软件或者是外围硬件设备。模拟器通过一些电脑程序或者是电子元器件去模拟其他的程序或者是设备。

> A hardware emulator is an emulator which takes the form of a hardware device. In a theoretical sense, the Church-Turing thesis implies that (under the assumption that enough memory is available) any operating environment can be emulated within any other environment. 

硬件模拟器是一种可以获取硬件模式的模拟器。从理论的角度来说，图灵机理论指出任何的操作环境都可以在其他的操作环境中被模拟。

**nasm：**

> Netwide Assembler （简称 NASM）是一款基于英特尔 x86 架构的汇编与反汇编工具。它可以用来编写16位、32位（IA-32）和64位（x86-64）的程序。 NASM被认为是Linux平台上最受欢迎的汇编工具之一。

**qemu：**

> QEMU（quick emulator）是一款由Fabrice Bellard等人编写的免费的可执行硬件虚拟化的（hardware virtualization）开源托管虚拟机（VMM）。其与Bochs，PearPC类似，但拥有高速（配合KVM），跨平台的特性。QEMU是一个托管的虚拟机镜像，它通过动态的二进制转换，模拟CPU，并且提供一组设备模型，使它能够运行多种未修改的客户机OS，可以通过与KVM（kernel-based virtual machine开源加速器）一起使用进而接近本地速度运行虚拟机（接近真实计算机的速度）。QEMU还可以为user-level的进程执行CPU仿真，进而允许了为一种架构编译的程序在另外一中架构上面运行（借由VMM的形式）。
