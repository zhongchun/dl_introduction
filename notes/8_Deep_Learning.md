# 深度学习
[TOC]

深度学习是加深了层的深度神经网络。基于之前介绍的网络，只需通过叠加层，就可以创建深度网络。本章我们将看一下深度学习的性质、课题和可能性，然后对当前的深度学习进行概括性的说明。

## 加深网络


## 深度学习的小历史
一般认为，现在深度学习之所以受到大量关注，其契机是 2012 年举办的大规模图像识别大赛 ILSVRC（ImageNet Large Scale Visual Recognition Challenge）。在那年的比赛中，基于深度学习的方法（通称 AlexNet）以压倒性的优势胜出，彻底颠覆了以往的图像识别方法。2012 年深度学习的这场逆袭成为一个转折点，在之后的比赛中，深度学习一直活跃在舞台中央。本节我们以 ILSVRC 这个大规模图像识别比赛为轴，看一下深度学习最近的发展趋势。

### ImageNet
ImageNet[25] 是拥有超过 100 万张图像的数据集。如图 8-7 所示，它包含了各种各样的图像，并且每张图像都被关联了标签（类别名）。每年都会举办使用这个巨大数据集的 ILSVRC 图像识别大赛。

ILSVRC 大赛有多个测试项目，其中之一是“类别分类”（classification），在该项目中，会进行 1000 个类别的分类，比试识别精度。我们来看一下最近几年的 ILSVRC 大赛的类别分类项目的结果。图 8-8 中展示了从 2010 年到 2015 年的优胜队伍的成绩。这里，将前 5 类中出现正确解的情况视为“正确”，此时的错误识别率用柱形图来表示。

图 8-8 中需要注意的是，以 2012 年为界，之后基于深度学习的方法一直居于首位。实际上，我们发现 2012 年的 AlexNet 大幅降低了错误识别率。并且，此后基于深度学习的方法不断在提升识别精度。特别是 2015 年的 ResNet（一个超过 150 层的深度网络）将错误识别率降低到了 3.5%。据说这个结果甚至超过了普通人的识别能力。

![](https://note.youdao.com/yws/api/personal/file/WEBf66009af2a301e67fb5143f04fbe564d?method=download&shareKey=088f2466a30bf4125649031a04299957)
图 8-8　ILSCRV 优胜队伍的成绩演变：竖轴是错误识别率，横轴是年份。横轴的括号内是队伍名或者方法名

ImageNet 挑战，举办从2010年到2017年。

### VGG

### GoogLeNet

### ResNet


## 深度学习的高速化


## 深度学习的应用案例


## 深度学习的未来


## 小结


## Reference
1. [深度学习入门：基于Python的理论与实现](http://www.ituring.com.cn/book/1921)