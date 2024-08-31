
# 快速弹簧算法(FSA)
## 介绍
这个算法由[BsoltB](https://github.com/BsoltB)发明，用于解决浮力的弹簧类问题。
## FSA第一部分：加水减水
### 公式推导
先看一张图：![图1-1](https://vip.helloimg.com/i/2024/08/31/66d2b66d1a18e.png)

其中蓝色是原来的水，红色+绿色是加的水。这部分水加进去会影响弹簧长度，则有长度变化量$\Delta L$。并且物体也会移动，则有移动距离$\Delta h_{移}$。

由此我们可以得出第一个式子：

$$\Delta h_{移} \times (S_{容}-S_{物}) + \Delta L \times S_{容} = \Delta V$$

以及第二个式子：

$$\Delta L + \Delta h_{移} = \Delta h_{水}$$

继续看第二张图：

![图1-2](https://vip.helloimg.com/i/2024/08/31/66d2baee6fb17.png)

图中我们对物体进行了受力分析，红色是 $G$，蓝色是 $F_{浮}$，绿色是 $F_{弹}$ ，我们发现物体处于平衡状态。所以 $G = F_{浮} + F_{弹}$（注：弹力也可能是竖直向下的，但不影响，看成负数即可）。进而我们推出 $\Delta F_{浮} = \Delta F_{弹}$。又因为 $\Delta F_{弹} = k \times \Delta L$，所以 $k \times \Delta L = \Delta F_{浮} = \rho_{液}gS_{物} \times \Delta h_{移}$。我们设 $k' = \rho_{液}gS_{物}$，出现我们的第三个式子：

$$k' \times \Delta h_{移} = k \times \Delta L$$（注：$k$ 单位是 $N/cm$，不能取倒数，会出问题）

提示：在多数题目中，$\rho_{液} = \rho_{水} = 10^3 kg/m^3$，且 $g$ 取 $10 N/kg$。而当 $S_{物} = 100 cm^2$时，通过计算发现 $k' = 1$，因此我们可以直接根据$k' = \frac{S_{物}}{100cm^2}$算出。

有了这个比例关系，可以不用方程求解弹簧加水减水问题。

### 实战

题目：
略。

解答：
略





