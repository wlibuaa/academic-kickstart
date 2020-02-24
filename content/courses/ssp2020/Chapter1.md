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

+ 晶体从外观上能够识别吗？需要从微观层面考察晶体的微观结构！

  | ![紫水晶](/courses/ssp2020/figs/amethyst.jpg) | ![金属](/courses/ssp2020/figs/ion.jpg) | ![玻璃](/courses/ssp2020/figs/glasscrystal.jpg) |
  | --------------------------------------------- | -------------------------------------- | ----------------------------------------------- |
  | 紫水晶                                        | 金属铁                                 | 玻璃制品                                        |

+ 布拉维格子（Bravais lattice）：晶体生成的美妙算法

  + 在漂亮的晶体之下，是原子有序排列的微观结构。

  + **晶体结构=布拉维格子+基元** 

    此表述十分类似于“程序=算法+语言”。自然界在创造如单晶矿石等晶体物质时候，基元是具体的物质内容，而由抽象的点构成的布拉维格子则是生成晶体的数学“算法”。按照指定的算法，将基元周期排列展开，就形成万千固态材料。

  + 布拉维格子有若干彼此等价的定义：

    (a) 直观定义：布拉维格子是格点的无限周期排列，其中每一个点都等价，即从任何一个格点看出去，周边的环境（从最近邻格点一直到无穷远处）都严格相同。

    (b) 数学定义：布拉维格子中的任意格点都可以表示为$R = \sum_i n_i \textbf{a}_i + r_0$，且公式不产生不属于格子中的点。式中$\{ a_i \}$为$d$个（$d$为空间维度）线性无关的向量，称为初基矢量（primitive vector）。$r_0$为某常数，当原点取在任一格点上时$r_0=0$。

    (c) 抽象定义：在加法下封闭的不共面矢量集合构成布拉维格子。

+ 一般格子

  + 常见二维格子有正方格子，三角格子，六角格子等。

  + 正方和三角为布拉维格子，六角格子为非布拉维格子，可以将两个点（下图中红色和蓝色）看做一个基元，按照其三角布拉维格子将其“生成”出来。因此，不难看出，六角格子是两套三角布拉维格子嵌套而成，有时人们称这类非布拉维格子为复式格子。

  + 单元素晶体将原子视为基元，其微观周期结构可能为布拉维格子或复式格子；多元素晶体总需要将多个原子视为基元，按照布拉维格子周期排列生成。

    | <img src="/courses/ssp2020/figs/squarelatt.png" style="zoom:60%;" name="square"/> | ![triangular](/courses/ssp2020/figs/trianlatt.jpeg) | ![honeycomb](/courses/ssp2020/figs/honeycomblatt.jpeg) |
    | ------------------------------------------------------------ | --------------------------------------------------- | ------------------------------------------------------ |
    | 正方格子                                                     | 三角格子                                            | 六角格子                                               |

  + 常见三维格子有简单立方，面心立方，体心立方，六角密堆积等。

### 2. 晶系分类

+ 二维布拉维格子：4大晶系（crystal family）5种布拉维格子

   ![二维布拉维格子](/courses/ssp2020/figs/2DBravLatt.jpg)

  + 单斜晶系(monoclinic net)：元胞为普通平行四边形
  + 正交晶系(orthorhombic net)：元胞为长方形，包含简单长方和面心长方两种
  + 六角晶系(hexagonal net)：元胞为菱形，初基矢量长度相等且夹60度（或120度）角
  + 四角晶系(tetragonal net)：元胞为正方形

+ 三维布拉维格子：7大晶系，14种布拉维格子

   ![三维布拉维格子](/courses/ssp2020/figs/3DBravLatt.jpg)

  + 固体物理八卦一则：Frankenheim (1842) miscounted this number as 15, A. Bravais is the first one get a right counting (1845).

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

1. 作为二维布拉维格子4大晶系的一组，四角晶系为何只有简单正方格子而无面心正方？同样，为何三维布拉维格子中只有体心四角而不存在底心四角格子？为何又存在底心正交？
2. 作为一种有趣的二维材料晶格，kagome格子备受关注。其结构如图所示，请问其布拉维格子属于哪一种？并计算填充率(filling rate)。

![kagome](/courses/ssp2020/figs/kagome.jpg)

