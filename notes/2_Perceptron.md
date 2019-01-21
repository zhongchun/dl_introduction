# 感知机

[TOC]

本章将介绍感知机(严格地讲，本章中所说的感知机应该称为“人工神经元”或“朴素感知机”，但是因为很多基本的处理都是共通的，所以这里就简单地称为“感知机”。)
（perceptron）这一算法。感知机是由美国学者 Frank Rosenblatt 在 1957 年提出来的。为何我们现在还要学习这一很久以前就有的算法呢？因为感知机也是作为神经网络（深度学习）的起源的算法。因此，学习感知机的构造也就是学习通向神经网络和深度学习的一种重要思想。

## 感知机什么
感知机接收多个输入信号，输出一个信号。

感知机的多个输入信号都有各自固有的权重，这些权重发挥着控制各个信号的重要性的作用。也就是说，权重越大，对应该权重的信号的重要性就越高。

## 简单逻辑电路
### 与门
两个条件同为一个为1，为true。

### 与非门
与门相反，任其中一个条件不为true，为true，即两个都不为true时，为true。

### 或门
其中一个条件为true，为true。

## 感知机的实现
### 简单的实现

### 导入权重和偏置

### 使用权重和偏置的实现

## 感知机的局限性
### 异或门

### 线性和非线性
感知机的局限性就在于它只能表示由一条直线分割的空间。
严格地讲，单层感知机无法表示异或门或者单层感知机无法分离非线性空间。

## 多层感知机
### 已有门电路的结合

### 异或门的实现

## 从与非门到计算机
多层感知机可以实现比之前见到的电路更复杂的电路。比如，进行加法运算的加法器也可以用感知机实现。此外，将二进制转换为十进制的编码器、满足某些条件就输出 1 的电路（用于等价检验的电路）等也可以用感知机表示。实际上，使用感知机甚至可以表示计算机！

计算机是处理信息的机器。向计算机中输入一些信息后，它会按照某种既定的方法进行处理，然后输出结果。所谓“按照某种既定的方法进行处理”是指，计算机和感知机一样，也有输入和输出，会按照某个既定的规则进行计算。

人们一般会认为计算机内部进行的处理非常复杂，而令人惊讶的是，实际上只需要通过与非门的组合，就能再现计算机进行的处理。这一令人吃惊的事实说明了什么呢？说明使用感知机也可以表示计算机。前面也介绍了，与非门可以使用感知机实现。也就是说，如果通过组合与非门可以实现计算机的话，那么通过组合感知机也可以表示计算机（感知机的组合可以通过叠加了多层的单层感知机来表示）。

综上，多层感知机能够进行复杂的表示，甚至可以构建计算机。那么，什么构造的感知机才能表示计算机呢？层级多深才可以构建计算机呢？

理论上可以说 2 层感知机就能构建计算机。这是因为，已有研究证明，2 层感知机（严格地说是激活函数使用了非线性的 sigmoid 函数的感知机，具体请参照下一章）可以表示任意函数。但是，使用 2 层感知机的构造，通过设定合适的权重来构建计算机是一件非常累人的事情。实际上，在用与非门等低层的元件构建计算机的情况下，分阶段地制作所需的零件（模块）会比较自然，即先实现与门和或门，然后实现半加器和全加器，接着实现算数逻辑单元（ALU），然后实现 CPU。因此，通过感知机表示计算机时，使用叠加了多层的构造来实现是比较自然的流程。

## 小结
- 感知机是具有输入和输出的算法。给定一个输入后，将输出一个既定的值。
- 感知机将权重和偏置设定为参数。
- 使用感知机可以表示与门和或门等逻辑电路。
- 异或门无法通过单层感知机来表示。
- 使用2层感知机可以表示异或门。
- 单层感知机只能表示线性空间，而多层感知机可以表示非线性空间。
- 多层感知机（在理论上）可以表示计算机。


## Reference
1. [《深度学习入门》第 2 章 感知机 笔记](http://www.ituring.com.cn/article/507311)
