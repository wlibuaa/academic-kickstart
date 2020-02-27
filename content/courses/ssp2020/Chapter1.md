---
title: "第一章 晶体结构"
linktitle: Chapter 1
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



## Crystal Structure

### ***1. 晶体结构的基本概念*** 

<img src="/courses/ssp2020/figs/quartz3.jpeg" style="zoom:55%;" name="square"/>

+ 布拉维格子（Bravais lattice）：晶体的美妙算法

  + 在漂亮的晶体之下，是原子有序排列的微观结构。

    | <img src="/courses/ssp2020/figs/grains.jpg" style="zoom:80%;"/> |
    | :----------------------------------------------------------: |
    | 非凡一念：晶体不断细分，由同样晶面角度、与整体具有相似形状的元胞 |

  + **晶体结构=布拉维格子+基元** 

    类似于“程序=算法+语言”：自然界在创造如单晶矿石等晶体物质时候，基元是具体的物质内容，而由抽象的点构成的布拉维格子则是生成晶体的数学“算法”。按照指定的算法，将基元周期排列展开，就形成万千固态材料。

  + 布拉维格子有若干彼此等价的定义：

    (a) 直观定义：布拉维格子是格点的无限周期排列，其中每一个点都等价。即从任何一个格点看出去，晶格都是一模一样的，周边的环境都严格相同。

    (b) 数学定义：布拉维格子中的任意格点都可以表示为$R = \sum_i n_i \textbf{a}_i + r_0$，且公式不产生不属于格子中的点。式中$\{ a_i \}$为$d$个（$d$为空间维度）线性无关的向量，称为初基矢量（primitive vector）。$r_0$为某常数，当原点取在任一格点上时$r_0=0$。

    (c) 抽象定义：在加法下封闭的不共面矢量集合构成布拉维格子。
    
  + 非布拉维格子的描述：

    非布拉维格子中的任意格点都可以表示为$R = \sum_i n_i \textbf{a}_i + \sum_j r_j$，表示先按照初基矢量集合{$\textbf{a}_i$}访问最近的布拉维格点，然后再按照{$r_j$}依次访问基元中$n$个不同的点（$j$从0跑到$n-1$）。

+ 常见二维格子

  + 并非所有周期排列的格子都是布拉维格子。如下图所示，正方和三角为布拉维格子，但六角格子为非布拉维格子。

  + 可以将六角格子中的两个点（下图中红色和蓝色）看做一个基元，按照三角布拉维格子将其“生成”出来。因此，六角格子可以视为两套三角布拉维格子嵌套而成，有时人们称这类非布拉维格子为复式格子。

  + 单元素晶体将原子视为基元，其微观周期结构可能为布拉维格子或复式格子；多元素晶体总需要将多个原子视为基元，按照布拉维格子周期排列生成。

    | <img src="/courses/ssp2020/figs/squarelatt.png" style="zoom:60%;" name="square"/> | ![triangular](/courses/ssp2020/figs/trianlatt.jpeg) | ![honeycomb](/courses/ssp2020/figs/honeycomblatt.jpeg) |
    | ------------------------------------------------------------ | --------------------------------------------------- | ------------------------------------------------------ |
    | 正方格子                                                     | 三角格子                                            | 六角格子                                               |

+ 常见三维格子

  + 常见三维格子有简单立方，面心立方，体心立方，六角密堆积等。

    | <img src="/courses/ssp2020/figs/simplecubic.png" style="zoom:60%;" /> | <img src="/courses/ssp2020/figs/bcc.png" style="zoom:55%;" /> | <img src="/courses/ssp2020/figs/fcc.png" style="zoom:45%;" /> |
    | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
    | 简单立方(Simple Cubic, SC)                                   | 体心立方(Body-Centered Cubic, BCC)                           | 面心立方(Face-Centered Cubic, FCC)                           |

    ​	上述三种三维晶格，简单立方，体心立方，和面心立方，均为布拉维格子，每个基元仅仅包含一个原子。但有时为了方便讨论，会将体心立方与面心立方中的若干原子组合视为基元，按照简单立方布拉维格子展开生成，更好地体现了体心和面心立方的对称性，使用更为方便习惯(conventional)。

  + 密堆积结构是一类非常特殊的晶体结构，常见的有六角密堆积和面心立方（没错，就是上面提到的BCC！）。

    | <img src="/courses/ssp2020/figs/closepacking0.png" style="zoom:75%;"/> | <img src="/courses/ssp2020/figs/hcp.png" style="zoom:60%;"/> | <img src="/courses/ssp2020/figs/fcc2.png" style="zoom:55%;"/> |
    | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
    | 密堆积                                                       | 六方密堆积(Hexagonal Compact Packing, HCP)                   | 面心立方(Face-Centered Cubic, FCC)                           |

    从密堆积方式理解两种结构

    | <img src="/courses/ssp2020/figs/closepacking.png" style="zoom:60%;"/> |
    | ------------------------------------------------------------ |
    | 密堆积的A、B、C三种占位点                                    |
    | <img src="/courses/ssp2020/figs/closepacking2.png" style="zoom:60%;"/> |
    | 两种不同的密堆积分别形成六方密堆积和面心立方（还有无数种密堆积方式） |
  
    
  

****

### 2. 常见晶体结构

下面列举几种常见的晶体材料结构。

+ 金刚石结构

  | <img src="/courses/ssp2020/figs/diamond0.jpg" style="zoom:45%;"/> | <img src="/courses/ssp2020/figs/diamond.png" style="zoom:65%;"/> | <img src="/courses/ssp2020/figs/diamond1.png" style="zoom:95%;"/> | <img src="/courses/ssp2020/figs/zincblende.png" style="zoom:65%;"/> |
  | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
  | 金刚石                                                       | $a=3.57 \overset{\circ}{\rm{A}}$                             | 俯视图                                                       | 类似结构：闪锌矿                                             |

  + 金刚石结构由单质碳（C）组成，具有非常高的硬度。类似的单质结构还有硅（Si，$a=5.43 \overset{\circ}{\rm{A}}$），锗（Ge，$a=5.66 \overset{\circ}{\rm{A}}$）等晶体。

  + 典型的闪锌矿结构晶体包括：碳化硅（SiC，$a=4.35 \overset{\circ}{\rm{A}}$），砷化镓（GaAs，$a=5.65 \overset{\circ}{\rm{A}}$）等晶体。
  + 将每个碳原子视为抽象点，金刚石结构并非布拉维格子
  + 选取2个碳原子组成基元（$r_0=(0,0,0)$和$r_1=(1/4,1/4,1/4)$），对应布拉维格子为面心立方
  + 选取8个碳原子为基元（如何选取 {$r_j$}?），对应布拉维格子为简单立方。

+ NaCl晶体结构

  | <img src="/courses/ssp2020/figs/nacl0.png" style="zoom:90%;"/> | <img src="/courses/ssp2020/figs/nacl.png" style="zoom:60%;"/> | <img src="/courses/ssp2020/figs/nacl1.jpg" style="zoom:180%;"/> |
  | ------------------------------------------------------------ | ------------------------------------------------------------ | :----------------------------------------------------------- |
  | 食盐晶体                                                     | $a=5.63\overset{\circ}{\rm{A}}$                              | 硬球模型                                                     |

  + 具有和食盐类似晶体结构的有：氧化镁（MgO，$a=4.20\overset{\circ}{\rm{A}}$），氯化钾（KCl，$a=6.29\overset{\circ}{\rm{A}}$）等晶体。
  + 氯化钠晶体由Na和Cl两种元素组成，取二者各1组成基元，则布拉维格子为面心立方。

+ CsCl晶体结构

  | <img src="/courses/ssp2020/figs/cscl0.png" style="zoom:50%;"/> | <img src="/courses/ssp2020/figs/cscl.png" style="zoom:60%;"/> | <img src="/courses/ssp2020/figs/cscl1.jpg" style="zoom:190%;"/> |
  | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
  | 氯化铯晶体                                                   | $a=4.11 \overset{\circ}{\rm{A}}$                             | 硬球模型                                                     |

  + 粉末状的样品由微小的单晶组成。

  + 取Cs和Cl两种元素个1个原子组成基元，则布拉维格子为简单立方（注意：CsCl晶体不是体心立方结构）。

+ 二维晶体材料——石墨烯（单层石墨）

  | <img src="/courses/ssp2020/figs/graphene0.png" style="zoom:80%;"/> | <img src="/courses/ssp2020/figs/graphene.jpeg" style="zoom:150%;"/> |
  | ------------------------------------------------------------ | ------------------------------------------------------------ |
  | 石墨烯的扫描隧道显微镜照片                                   | 单层石墨烯结构示意图                                         |

  + 英国物理学家安德烈·盖姆和康斯坦丁·诺沃肖洛夫，用微机械剥离法成功从石墨中分离出石墨烯。共同获得[2010年诺贝尔物理学奖](https://www.nobelprize.org/prizes/physics/2010/summary/)。
  + 石墨烯具有高强度，高电导等优异的材料性能。

+ 双层魔转角石墨烯

| <img src="/courses/ssp2020/figs/BTGNature.jpeg" style="zoom:10%;"/> | <img src="/courses/ssp2020/figs/BTG.jpg" style="zoom:150%;"/> |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| 莫里超晶格                                                   | AA，AB，BA, BB 标记不同区域                                  |

+ 由于双层魔转角石墨烯的独特[电子关联性质](https://www.nature.com/articles/nature26154)和[非常规超导电性](https://www.nature.com/articles/nature26160)，引起了凝聚态物理学界的广泛关注，可以阅读[Physics Today](https://physicstoday.scitation.org/doi/pdf/10.1063/PT.3.4384)的科普文章。

****

### 3. 晶格元胞、填充率与晶面指数

+ 元胞（unit cell）与魏格纳-赛兹元胞（ Wigner-Seitz cell）

  + 元胞是由布拉维格子初基矢量所构造的平行六面体（三维）或平行四边形（二维），元胞通过平移可以覆盖二维布拉维格子。

  + Recipes for defining the **unit cell** of crystal

    1. For a Bravais lattice, an unit cell is the *parallelepiped* constructed out of its *primitive* vectors.
    2. For a general (Bravais or non-Bravais) lattice or real crystals, the unit cell can be constructed by (1) first identifying its underlying Bravais lattice *BL* (coule be itself in the simplest case) and (2) building up the unit cell using the primitive vectors of *BL*.
    3. Some Bravais lattice, e.g., FCC or BCC, conventionally one is used to identify the cube containing more than 1 lattice points as its conventional unit cell.  Otherwise, we always follow rule 2 for defininng an unit cell of crystal structures.

  + Definition of Wigner-Seitz cell

    + The geometric points that are nearest to the origin Bravais lattice point **R**=0 than to  any other Bravais lattice points. 

    + Practical definitionn: the space contained by bisection lines/surfaces of the origin point to other Bravais lattice points. 

      ![2D WS cell](/courses/ssp2020/figs/wscell2d.jpeg)

      ![3D WS cell](/courses/ssp2020/figs/wscell3d.jpg)

****

### 4. 晶系分类与对称性

+ 二维布拉维格子：4大晶系（crystal family）5种布拉维格子

   ![二维布拉维格子](/courses/ssp2020/figs/2DBravLatt.jpg)

  + 单斜晶系(monoclinic net)：元胞为普通平行四边形
  + 正交晶系(orthorhombic net)：元胞为长方形，包含简单长方和面心长方两种
  + 六角晶系(hexagonal net)：元胞为菱形，初基矢量长度相等且夹60度（或120度）角
  + 四角晶系(tetragonal net)：元胞为正方形

+ 三维布拉维格子：7大晶系，14种布拉维格子

   ![三维布拉维格子](/courses/ssp2020/figs/3DBravLatt.jpg)

  + 固体物理八卦一则：Frankenheim (1842) miscounted this number as 15, A. Bravais is the first one get a right counting (1845).

  

## Slides & Video

+ Slides for Chapter 1 can be downloaded (please click the BIG icon below) 

  [![](/courses/ssp2020/figs/coverc1.jpg "Wei Li")](/courses/ssp2020/slides/slidesc1.pdf)

+ Video lectures (two, by Sandro Scandolo, ICTP), please click the icon below.

  + [Lecture 02](https://www.bilibili.com/video/av47845416?p=2)
  
  + [Lecture 03](https://www.bilibili.com/video/av47845416?p=3)
  + [Lecture 04](https://www.bilibili.com/video/av47845416?p=4)

## Discussions

+ An online discussion (c.a. 30 + 30 min, via Wechat or Dingtalk) will be arranged.



## Homework

0. 一维布拉维晶格有多少种？
1. 请阅读关于石墨烯的[公众介绍材料](https://www.nobelprize.org/uploads/2018/06/popular-physicsprize2010.pdf)与[科学背景材料](https://www.nobelprize.org/uploads/2018/06/advanced-physicsprize2010.pdf)，并提交阅读笔记。
2. 作为二维布拉维格子4大晶系的一组，四角晶系为何只有简单正方格子而无面心正方？同样，为何三维布拉维格子中只有体心四方而不存在底心四方格子？为何又存在底心正交？
3. 作为一种有趣的二维材料晶格，kagome格子备受关注。其结构如图所示，请问其布拉维格子属于哪一种？并计算填充率(filling rate)。

![kagome](/courses/ssp2020/figs/kagome.jpg)

