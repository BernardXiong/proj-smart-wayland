# proj-smart-wayland

## 题目
在RT-Thread Smart操作系统上完成Wayland/Weston的移植，并运行图形terminal终端软件。

* RT-Thread Smart是RT-Thread操作系统的一个特性，它把RT-Thread嵌入式操作系统分成了内核态和用户态。在用户态上，具备完整的POSIX层，可以把很多的Linux/Unix开源软件移植进来。

## 项目描述：

基于RT-Thread Smart嵌入式操作系统，在QEMU/RISCV64或D1s开发板上完成Wayland/Weston移植：
* 在RT-Thread Smart内核层加入drm驱动；
* 在RT-Thread Smart上加入input子系统；
* 移植weston及相关依赖包到RT-Thread Smart用户态环境；
* 可以在图形输出，如LCD上，渲染Weston界面，并能使用Wayland Terminal软件

## 参考资料：

* https://wayland.freedesktop.org
* [qemu-riscv64 bsp](https://github.com/RT-Thread/rt-thread/tree/master/bsp/qemu-virt64-riscv)
* [riscv64 userapps](https://github.com/RT-Thread/userapps)

## 所属赛道
2023全国大学生操作系统比赛的“OS功能挑战”赛道

## 参赛要求
以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2023年春季学期或之后本科毕业的大一~大四的学生）或研究生
如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
请遵循“2023国大学生操作系统比赛”的章程和技术方案要求

## 项目导师
熊谱翔 bernard.xiong at rt-thread.com

* 可以赞助RISCV64的开发板

## 难度
中等 ~ 高 等

## 特征：

1. 需要移植weston及相关依赖软件包到RT-Thread Smart操作系统的用户态；
2. 能够在图形界面上运行wayland terminal软件；
3. 可以使用鼠标对窗口进行拖拽，更改大小；

## 预期目标
#### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标
#### 注：为了避免重复造轮子，本项目既可以从头开发，也可以联系导师在其项目基础上进行进一步的开发

1. 支持到qemu/riscv64软件模拟平台或D1s硬件开发板；
2. 最终需要能够提交到RT-Thread upstream仓库；
