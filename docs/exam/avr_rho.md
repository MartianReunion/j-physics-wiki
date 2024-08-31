
# 平均密度

## 介绍

在解决结合体漂浮/悬浮/沉底类问题（比如最经典的蜡烛问题）时，平均密度是很有用并且快速的方法——不需要列方程。

## 公式推导

我们先设一个结合体是由A/B两种物质结合的。其中 $\rho_B \le \overline{\rho} \le \rho_A$（上横线代表平均）。

然后我们知道：

$$\overline{\rho} = \frac{m_{总}}{V_{总}} = \frac{\rho_A V_A + \rho_B V_B}{V_A + V_B}$$

进而得出：

$$\overline{\rho} V_A + \overline{\rho} V_B = \rho_A V_A + \rho_B V_B$$

$$V_A \times (\rho_A - \overline{\rho}) = V_B \times (\overline{\rho} - \rho_B)$$

所以我们就得出了比例关系：

$$\frac{V_A}{V_B} = \frac{\overline{\rho} - \rho_B}{\rho_A - \overline{\rho}}$$

大功告成。

## 实战

蜡烛问题：有一根蜡烛长为$20cm$，底面积为 $2cm^2$，密度为 $0.8g/cm^3$，有一个铁块质量为 $8g$，$\rho_{铁} = 8 g/cm^3$。将铁块粘在蜡烛下面（忽略结合处质量体积），发现放进水里面漂浮。点燃蜡烛，若蜡烛每秒烧去$0.05cm$，从点燃开始计时，则蜡烛何时熄灭？（水的密度$1g/cm^3$）

解答：

因为熄灭的时候正好悬浮，所以 $\overline{\rho} = \rho_{水}$。

因此我们采用平均密度公式，计算出 $\frac{V_{蜡}}{V_{铁}} = \frac{1}{35}$。因为铁的体积不变，所以 $V_{蜡} = 35cm^3$。的出需要烧去$5cm^3$蜡烛。算出需要$50$秒。




