# 电功率图像问题

## 摘要

本文分为三个部分。分别是以电阻电压和电流为X轴，然后电功率为Y轴的图像问题。

本文所有图像问题均在一个定值电阻 $R$ 和一个滑动变阻器 $R_p$ 串联并且电压 $U$ 不变 的情况下进行。

## R-P 图像

[见这里](https://j-physics-wiki.ares-mars.top/physical-quantities/dlzg/#_7)

## I-P图像

我们假设电流为 $I$。则有如下推导：

$$P_{R_p} = P_{all} - P_{R} = UI - I^2R = -R \times I^2 + U \times I$$

因为电源电压不变以及定值电阻的电阻也不变，所以说 $P_{R_p}$ 可以看作是关于 $I$ 的一个二次函数。

它的图像如下。

[图像（需要geogebra）](https://www.geogebra.org/calculator/axj6e6r6)

我们可以通过对称轴求出它的最大值。

$$I = -\frac{b}{2a} = \frac{U}{2R} , \max = \frac{U^2}{4R}$$

也就是说当电路中的电流等于以上的这个数时，滑动变阻器的电功率最大。通过与上次的R-P图像的比较，我们发现这个推论是正确的。

### 更进一步的推论

由于二次函数的对称性，所以当两个情况的电流不同，但 $P_{R_p}$ 是相等的情况下，这两种情况的电流之和应该是等于对称轴的两倍。这样的结论适用于多情况问题——能够更快地做出解答。

## U-P 图像

我们假设滑动变阻器两端的电压为 $U_p$ ，则有如下推导。

$$P_{R_p} = U_pI = U_p \times \frac{U-U_p}{R} = \frac{U \times U_p - U_p^2}{R} = -\frac{1}{R} \times U_p^2 + \frac{U}{R}\times U_p$$

这是图像——[还是geogebra](https://www.geogebra.org/calculator/qwq7rpss)。

经过推导，我们发现这也是一个二次函数，只不过是关于 $U_p$ 的。同理，我们也可以通过对称轴求出它的最大值。

$$U_p = \frac{1}{2}U , \max = \frac{U^2}{4R}$$

### 更进一步的推论

同上。

## 实战

暂缺。




