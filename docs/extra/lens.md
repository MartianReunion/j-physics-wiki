# 凸透镜成像公式

## 引入

我们在初二就学过凸透镜的成像规律：

| 物距 $u$ | 倒正 | 大小 | 虚实 | 物侧 | 像距 $v$ | 应用 |
|--|--|--|--|--|--|--|
| $u > 2f$ | 倒 | 缩小 | 实 | 异侧 | $f < v < 2f$ | 照相机 |
| $u = 2f$ | 倒 | 等大 | 实 | 异侧 | $v = 2f$ | 测量焦距 |
| $f < u < 2f$ | 倒 | 放大 | 实 | 异侧 | $v > 2f$ | 投影仪 |
| $u = f$（不成像） | N/A | N/A | N/A | N/A | N/A | N/A |
| $u < f$ | 正 | 放大 | 实 | 同侧 | 初中物理不考虑 | 放大镜 |

但是这个表格有点难记，怎么办呢？（我们的宗旨：物理应该是使用 $CPU$或者 $GPU$ 而不是硬盘）

## 公式

所以我们在此介绍成像公式：

$$\frac{1}{u} + \frac{1}{v} = \frac{1}{f}$$

??? note "注意"
    此公式在初中范围内不要求掌握，更不要求推导，请注意！

这个公式将$u,v$的变化范围囊括其中。你可以尝试将 $u,v$ 代入试试看，他完全正常工作。

并且我们也可以注意到，在成实像时，$u,v$ 都是正数；反之为负数。

这个公式也可以解释为什么 $u = f$ 是不成像的条件，因为此时 $\dfrac{1}{v} = 0$，这是不可能的。

至于放大缩小的问题，你只需要用我们的第二个公式（$a \leftarrow b$表示$a$增加$b$就减小，反过来也一样）：

$$v \leftarrow Size,u \rightarrow Size$$

这样就行了。

## 推导

（前置：初中数学：相似三角形）

![图1-1](/assets/extra/lens/1_1.png)

先看图。

我们不难发现，$\Delta A O B \sim \Delta D O E,\Delta C F_{2} O \sim \Delta D F_{2} E$。通过这两个相似三角形，我们得出：

$$AB = OC, AB : DE = AO : OD,OC: DE = OF_{2} : F_{2}D$$

那么替换以下 $AB,OC$，得到$AO : OD = OF_{2} : F_{2}D$。那么在把这些繁琐的线段替换为 $u,v,f$ 的形式，得到：

$$\frac{u}{v} = \frac{f}{v-f}$$

化简：

$$uv-uf = vf$$

$$uv=f \times (u+v)$$

$$\frac{uv}{u+v} = f$$

两边同时取倒数：

$$\frac{u+v}{uv} = \frac{1}{f}$$

那么最终得到这个公式：

$$\frac{1}{u} + \frac{1}{v} = \frac{1}{f}$$

大功告成！

## 扩展

此公式对凹透镜也适用。但是我们要把凹透镜看成一个 $f < 0$ 的凸透镜。

??? note "俄罗斯套娃"
    这都是扩展内容了，还来了个扩展中的扩展（但其实凹透镜在透镜的那节课也是提到了一下的，所以也算初中物理）。