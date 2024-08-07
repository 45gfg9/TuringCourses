# 计算机组成与设计
<div class="badges">
<span class="badge cs-badge">CS 专业基础</span>
<span class="badge ai-badge">AI 专业基础</span>
</div>

## 课程学习内容
《计算机组成与设计》是 CS 硬件必修课的第二门，实验难度与《计算机逻辑设计基础》相比提升较大，理论课程难度适中。课程理论部分总体内容是介绍一台计算机的基本构成，章节分为 ISA、 CPU（从单周期到流水线）、 Memory Hierarchy、 IO；课程实验部分的目标是使用 Verilog 语言完成一个单周期 CPU （包括简单中断），在此基础上完成一个流水线 CPU。

《计算机组成》与本课在理论课程部分几乎没有差别，因此在学习理论部分时可以参考相同的资料；本课实验部分难度比《计算机组成》更大。

### 先修要求
要求修读过《计算机逻辑设计基础》或《数字逻辑设计》。但从直接感受上，没有修读过上述课程对本课的理论部分影响不大。

要求尽可能熟练地使用 Verilog 编写实验代码。

## 任课教师
本课目前有姜晓红与刘海风两位老师开设课程，两位老师人都很好。

=== "姜晓红"

    姜晓红老师在计算机组成、体系结构方面的教学有丰富的经验，讲课思路比较清晰，语速较慢，不太会使用电脑软件。最后会公示各个部分的得分。

    实验对验收的要求较高（取决于是否有助教协助验收，如果是姜老师本人验收则要求更严格，具体可见分数构成部分）。从 2023 年的实验部分来看，使用的是潘学长所写框架，在单周期 CPU 中断部分难度更高。

=== "刘海风"

    刘海风老师本身研究方向并不是系统范畴，因此对于这门课的内容不算很熟悉。（但老师已经教授数逻计组多年）老师的讲课水平高于计院老师平均水平，能把 PPT 讲清楚，但偶尔会卡壳。喜欢点人起来回答问题（开火车x）。最后不会公示平时分和期末成绩。
    
    实验验收使用的验收代码比较复杂，可能在实验时要用比较多的时间 debug。笔者会在2023年春夏给刘海风老师做助教，欢迎大家对实验授课以及实验指导提出建议。


## 分数构成
两位老师的分数构成基本相同，仅有细节上的差异。

- 理论部分：70%
    - Quiz + Homework：20%  
        - 姜老师班：有 2~3 次 Quiz，形式是学在浙大上的选择填空题或者线下纸质。还有 6 次作业，由助教批改。
        - 刘老师班：有 2 次 Quiz，形式是线下纸质，同学交换批改。作业不定期检查（交了就行）。2023 年春夏学期取消了期中考试，因此这部分占了 30% 的分数。
    - Midterm test：10%
    - Final exam（闭卷，允许带一张 A4 纸）：40%
- 实验部分：30%
    - 姜老师班：验收 18% + 报告 12%  
    需要注意的是，姜老师对实验验收有特殊的要求，即每个实验只有两次验收机会，如果第一次验收不通过扣除 10% 的分数，第二次验收不通过则直接 0 分。
    - 刘老师班：验收 12% + 报告 18%  
    具体可见 2023 年春夏的[实验文档](https://guahao31.github.io/2023_CO/)

## 参考书目与网站
从2019级开始，我们学校使用的教材均为 **RISC-V** 版本。

- 《计算机组成与设计》*Computer Organization and Design The Hardware Software Interface [RISC-V Edition]*

如果 Verilog 的基本语法比较生疏，可以通过 [HDLBits](https://hdlbits.01xz.net/wiki/Main_Page) 进行学习。

CS61C 课程提供了 [Venus](https://venus.cs61c.org/) 工具，你可以在上边模拟 RISC-V 代码，也可以使用它得到汇编代码对应的机器码。

## 参考笔记与回忆卷

- WellesSun 的[计组笔记](https://github.com/CSWellesSun/ZJUCourse/blob/main/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BB%84%E6%88%90%E4%B8%8E%E8%AE%BE%E8%AE%A1/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BB%84%E6%88%90%E4%B8%8E%E8%AE%BE%E8%AE%A1.md)
- [2022 春夏期末回忆卷](./2021-2022_春夏学期_计算机组成与设计_期末考试回忆卷.pdf)
- xg 计算机系统二流水线 CPU 部分笔记：https://note.tonycrane.cc/cs/system/cs2/topic1/
- QJJ 计算机组成笔记：https://note.hobbitqia.cc/CO/
- [2023 春夏期末回忆卷（98 链接）](https://www.cc98.org/topic/5640722)
- [2024 春夏期末回忆卷（98 链接）](https://www.cc98.org/topic/5922030)

## 课程学习建议
本课由理论和实验两部分组成，从分数上看，实验部分与期末考试几乎是同等重要，本课的学习建议也将分为两部分。
### 理论部分
课程实验主要内容是实现单周期/流水线 CPU，理论部分需要熟知 CPU 的构成与时序。

本课的理论部分难度适中。对于未修读《汇编语言》/《计算机系统概论》的同学来说，是第一次在课堂接触汇编语言，在理解和使用 RISC-V 的指令上需要一些时间；ISA 是本课的第一个重点，期末考试的考察中一定有对指令作用的考察（各种类型指令的格式一般会打印在卷子上）； CPU 相关内容是本课最重要、讨论时间最长的部分，主要是理解每条指令对应的 CPU 控制信号的作用从而理解 datapath，这部分需要认真听讲；流水线 CPU 是我们接触的第一个通过指令级并行获得性能提升的处理方式，需要理解各种 *Hazard* 的成因以及我们高效解决的方式，这部分将是考试的重点；内存层级部分我们需要理解**缓存 (cache)** 的理论基础（局部性原理）并了解提升 cache 性能的方式，这部分在期末考试中会出现计算题。

总的来说，理论部分听老师讲解已经足够，在复习时将琐碎的点都记到 cheating sheet 上即可。如果不喜欢自己老师的讲课风格的可以尝试马德老师的智云课堂，感受“浙大硬件之光”的魅力。

对于考试而言，2022 年春夏和 2023 年春夏题目风格较统一，回忆卷或许能有所帮助。

### 实验部分
实验部分对不少同学来说是噩梦，笔者认为痛苦来源主要是：缺乏理论基础（不知道 CPU 每一部分的功能）以及对 Verilog 基础语法或测试方法掌握不好。

CPU 部分可以先画好 datapath 之后再入手，在知道各部分作用之后可以更合理地排布代码，方便后期查看与修改。

因为 Vivado 套件的综合速度很慢，所以在准备下板前一定进行充分的测试，使用波形来初步查看代码功能是不是正确。更折磨的是明明波形测试没有任何问题，但是下板现象并不符合波形，你可以查看 [Synthesizable Verilog](http://www.ee.ncu.edu.tw/~jfli/vlsidi/lecture/Verilog-2012.pdf) 第 17-31 页并修改自己的代码。

图灵班的计组实验内容比普通班的要求更多更麻烦，不能单纯地抄 PPT 连线。同时计组往往与其他硬课同时进行，因此如果把实验拖到期末可能会有很大压力。笔者建议各位同学可以提早开始 CPU 的设计，不必按部就班地等老师讲到这里再开始。值得一提的是，除开实验上板，东四 509 也是十分适合自习的地方（有空调，有插座）。