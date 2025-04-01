# learning_os
2025 春夏季开源操作系统训练营学习记录，地址：https://opencamp.cn/os2edu/camp/2025spring

# 第二阶段
## 2025.03.31-2025.04.11
#### 2025.04.01
第一章：https://learningos.cn/rCore-Camp-Guide-2025S/chapter1/index.html
看完了第一章，例子测试通过，只看懂了原理，涉及到rust asm，RISCV，linker.ld的地方比较头脑混沌，暂时先不继续第二章了，先寻找一些资料补充一下基础。
* 回头看导学视频，之前跳着看，现在仔细的看一下其中的一些章节。

#### 2025.03.31
第零章的说明： https://learningos.cn/rCore-Camp-Guide-2025S/0setup-devel-env.html 配置环境，整个过程比较顺利。
* 由于我是在Windows 11上开发，所以需要安装wsl2，安装wsl2和Ubuntu 24.04.1，这一段网上都有现成的教程，没有什么问题。
* qemu安装，原本想试试最新的stable版本9.2.3，但是发现自己是新手，而且依照指南中的提示可能会遇见需要安装额外的依赖包，就继续使用7.0.0版本（其实有7.2.17版本，但是考虑到不熟悉，还是严格遵守教程的7.0.0版本，有兴趣的同学可以自己尝试）。
* 编译qemu过程中，只遇见了缺少Ninja，所以用sudo apt update, sudo apt install ninja-build 安装即可。
* 试运行rCore-Tutorial时，下载cargo nightly-2024-05-02版本很慢，大家要多等待一下，一次性完成编译和运行ch1，很顺利。


# 第一阶段
## 2025.03.24-2025.03.30
因为之前已经自学过Rust，所以导学视频和Rust视频就没仔细的看，挑选的看了一部分。
编程中遇见最大的困难就是那10道算法题，其中bsf，dsf，graph的比较难，结合kimi查阅了文档，编写了出来。
Rust在编写诸如链表之类的数据结构的时候，比较不友好，远没有C那么容易学会。