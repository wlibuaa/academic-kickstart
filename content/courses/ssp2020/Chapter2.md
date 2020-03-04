---
title: "第二章 晶体衍射"
linktitle: Chapter 2
toc: true
type: docs
date: "2020-02-22T00:00:00+01:00"
draft: false
menu:
  ssp2020:
    parent: SSP2020
    weight: 1

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 1
---



## Crystal Diffraction

| <img src="/courses/ssp2020/figs/dioptase.jpeg" style="zoom:50%;" name="square"/> |
| ------------------------------------------------------------ |
| *翠铜矿 dioptase*                                            |

+ 晶体从外观上能够识别吗？需要从微观层面考察晶体的微观结构！

| ![紫水晶](/courses/ssp2020/figs/amethyst.jpg) | ![金属](/courses/ssp2020/figs/ion.jpg) | <img src="/courses/ssp2020/figs/turquoise.png" style="zoom:42%;" name="square"/> | <img src="/courses/ssp2020/figs/glasscrystal.jpg" style="zoom:100%;" name="square"/> |
| --------------------------------------------- | -------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 紫水晶                                        | 金属铁                                 | 绿松石                                                       | 玻璃制品                                                     |

+ 扫描隧道显微镜（STM, 1981）通过针尖的量子隧穿电流的大小可以直接“读取”电子密度、形貌特征等，使得人们第一次可以直接观察到原子的**有序排列**。但是，STM**仅限于观察金属的表面**，无法观察到体态（bulk）的微观结构。

  <img src="/courses/ssp2020/figs/stm.jpeg" style="zoom:120%;" name="square"/>

+ 其他局域观测方法包括X-射线光电子能谱（XPS）等。

+ 要观察体态的微观结构，需要采用衍射方法，包括电子显微镜，中子衍射，**X-射线衍射**等，这些方法采用电子/中子/光子的波动性，观察晶格的倒空间。

+ 通过X射线衍射实验（劳厄，1912年，慕尼黑大学），人们第一次确认了晶体的周期结构。

<img src="/courses/ssp2020/figs/LauerMunich.jpg" style="zoom:100%;" name="square"/>

+ **衍射的亮斑对应倒空间的格矢，并进一步对应实空间的一族晶面。**

****

### 1. 劳厄方程与倒易点阵 (Reciprocal lattice)

+ 为引入倒格矢，考虑在布拉维格子上的X-射线衍射问题：入射波为$e^{i (\bf{k}\cdot\bf{r} - \omega t})$，在格点$\bf{r=R}$处发生反射，沿着$\bf{k'}$继续传播，波函数为$e^{i (\bf{k'}\cdot\bf{r} - \omega' t})$。

  + 弹性散射，原子附近的电子云随入射波震荡，并发射相同波长/频率的反射波，$\omega' = \omega$，且$|\bf{k}|=|\bf{k'}|$。

  + 波从$\bf r_0$出出发，经原子反射后反射到达$\bf r_f$处，波函数为：

    $ e^{i  k \cdot (R-r_o) } \times e^{i  \bf{k'} \cdot (r_f-R) }  = e^{i(\bf{k'} \cdot r_f - k \cdot r_0)} \times e^{i  (\bf{k'} - k) \cdot R }$

  + 假设观察者足够远，看到$k'$方向的彼此平行的出射波，其强度需要对任意$\bf{R}$求和，即$\bf |\sum_I e^{i  (\bf{k'} - k) \cdot R_I} |<sup> 2 </sup>$。

  + 对于满足**劳厄方程**$\bf e^{i  (\bf{k'} - k) \cdot R } \equiv 1$条件的衍射情况，将在$\bf{k'}$方向看到**相干衍射**。

    <img src="/courses/ssp2020/figs/lauerformula.png" style="zoom:50%;" name=""/>

    因此，想要看到相干衍射峰，对衍射波的波矢变化$\bf \Delta k =  k'-k$是有严格要求的。下面我们会看到，这个实际上是约定了一组特殊的矢量集，称为倒格矢集合{$G$}。

+ 满足下面条件的矢量$G$ 被定义为倒格矢：对于布拉维格子的任意格矢$R_I$，都满$G \cdot R_I = 2 \pi n$，其中$n$为整数，使得$e^{i G \cdot R_I} = 1$。

  + 倒格矢集合$G$构成布拉维格子，称为倒易点阵。倒易点阵必为布拉维格子（*证明？*）

  + 倒格子初基矢量（$b_j$）与正格子初基矢量（$a_i$）满足关系：

    $a_i \cdot b_j =2 \pi \delta_{ij}$

    例如，$a_1 \cdot b_1 = 2 \pi$，而$a_1 \cdot b_2 =  a_1 \cdot b_3 = 0$。

  + 倒格子初基矢量计算公式（*验证是否满足倒格子初基矢量关系*）

    $ b_i = 2\pi \frac{a_j \times a_k}{\Omega} $

    其中$\Omega = a_i \cdot (a_j \times a_k)$，且$i,j,k=1,2,3$满足轮换关系，如当$i=1,j=2$时，$k=3$。

  + 利用倒格子初基矢量$b_j$可以将倒格矢展开$G_{h,k,l}= h b_1 + k b_2 + l b_3$，其中$h,k,l$为整数（也恰好是与倒格矢$G$相垂直晶面族的晶面指数，见下文介绍）。

+ 倒易点阵举例

  + 一维倒格子：一维布拉维格子只有一种，相应也只有一种倒格子。

    <img src="/courses/ssp2020/figs/Recprc1D.jpg" style="zoom:60%;" name=""/>

    倒格矢为$b_1=\frac{2\pi}{a}$，$a$为晶格常数。

  + 二维倒格子

    <img src="/courses/ssp2020/figs/recprc2d.jpg" style="zoom:100%;" name=""/>

    长方（rectangular）格子的倒格子仍是长方格子，满足$A =\frac{2\pi}{|a|} \hat{a}_1$, $B =\frac{2\pi}{|b|} \hat{b}_2$

    单斜（oblique）格子的倒格子仍是单斜格子，满足$A \perp b$且$A\cdot a = 2\pi$，$B \perp a$且$B \cdot b = 2\pi$

    **问题：** 三角格子的倒格子是什么？（*追问：* 有心长方的倒格子是什么？）

  + 三维倒格子

    + 简单立方为自身的倒格子

    + 面心立方和体心立方互为对方的倒格子

      <img src="/courses/ssp2020/figs/fcc-bcc.jpg" style="zoom:100%;" name=""/>

    + **问题：** 底心正交格子的倒格子是什么？

      <img src="/courses/ssp2020/figs/basecenortho.jpg" style="zoom:100%;" name=""/>

  


### 2. 晶面反射与布拉格定律

+ 晶面族与倒格矢
+ 布拉格定律
+ 两种表述等价性

### 3. 结构因子与消光

+ 一般格子的衍射极大条件与几何结构因子

+ 面心立方、体心立方的结构因子

    

### 4. 实验方法

+ 
+ 



## Slides & Video

+ Slides for Chapter 2 can be downloaded [![here](/courses/ssp2020/figs/coverc2.jpg "Wei Li")](/courses/ssp2020/slides/slidesc2.pdf)  

  [^_^]:[![](/courses/ssp2020/figs/coverc1.jpg "Wei Li")](/courses/ssp2020/slides/slidesc2.pdf) 

+ Video lectures (two, by Sandro Scandolo, ICTP), please click the icon below.

  + [Lecture 05](https://www.bilibili.com/video/av47845416?p=5)
  + [Lecture 06](https://www.bilibili.com/video/av47845416?p=6)
  

## Discussions

+ An online discussion (c.a. 30 + 30 min, via Wechat or Dingtalk) will be arranged.

  

## Homework

+ 1. 请证明倒格子原胞体积$\Omega$<sup>*</sup>与正格子（布拉维格子）原胞体积$\Omega$的乘积为$(2\pi)$<sup>3</sup>。
  2. 证明劳厄方程/布拉格定律的等价表述：入射波波矢$\bf{k}$与倒格矢$\bf{G}$满足关系$\bf{k} \cdot \frac{1}{2} G= (\frac{1}{2}G)^2$，则产生布拉格衍射。并籍此说明该表述的一个直观图像：入射波矢出发点位于原点$O$时，当终点位于布里渊区边界上时，发生布拉格衍射。

