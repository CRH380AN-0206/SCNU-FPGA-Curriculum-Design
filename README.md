# SCNU FPGA 课程设计项目

## 设计任务和要求

### 设计任务

按要求用Verilog语言完成设计，用Quartus II工具编译和综合，在实验板上调试并实现功能和技术指标，撰写实验报告，最后提交验收并答辩。

题目：8位并行乘法器。主要功能要求：
1. 按键1，异步复位
2. 按键2，流水灯，6个数码管显示学号后六位
3. 按键3，调节8位乘法器的输入X，X显示到左边前2个数码管
4. 按键4，调节8位乘法器的输入Y，Y显示到中间2个数码管
5. 按键5，求值，按下后，计算X乘以Y的结果，用Z表示，并显示到数码管
6. 按键6，X从00开始自动递增到FF，Y从00开始自动递增到FF，计算乘法结果，输入输出均要显示，显示尽量有几秒钟的时间，能够在验收时看的清楚（不一定从0开始递增，可自行设定初值）
7. 所有按键应该能够进入和退出，所有按键应消抖处理
8. 数码管应采用动态扫描显示
9. 其余功能可自由发挥

### 设计要求

1. 撰写实验报告，主要内容包含：设计原理、程序设计、仿真、运行结果（例如实验板运行时的照片）、结论/分析、使用说明等，在最后附上源程序。
2. 模块化设计，模块划分合理（采用结构化的描述方式），程序结构清晰，可读性强，关键语句须注释。

## 文件结构

```
scnu-fpga-curriculum-design
|-- source          源代码文件夹
|   |-- modules         各个硬件模块
|   |-- testbench       一些硬件模块的测试
|   |-- cd_top.v    顶层设计文件
|-- quartusii       Quartus II 项目文件夹
|-- README.md       题目要求和项目说明
```

## 使用方法

仅限学习和讨论交流使用，请勿抄袭作为个人作业打发你的教师 :)

## 附加功能

使用BUT7作为BCD/HEX切换按键
