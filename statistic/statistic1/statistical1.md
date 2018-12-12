# 第一章 近独立粒子系统的统计分布

## 基本概念
* 统计力学的基本立足点：系统的宏观量等于微观量的统计平均值；
* 统计力学的几率性认识：在一定的宏观条件下，某一时刻系统以几率分布的形式处在各种可能的微观状态中。在平衡状态下，这个几率分布不随时间改变；
* $\mu$空间：以广义坐标和广义动量为坐标基矢的2r维空间，其中r为粒子的自由度；
* 近独立粒子系统：若系统的粒子间相互作用的平均能量远远小于单个粒子的平均能量，则该系统称为近独立粒子系统；
* 系统的微观状态：粒子在各个量子状态上的某种特定的占据方式称为系统的一个微观状态；
* 系统的分布：设$\varepsilon_i$是单粒子的第i个能级，这个能级有$n_i$个粒子占据，则这些$n_i$的集合称为一个分布，即为$\{n_i\}$；
* 等几率假设：对于处在平衡态的孤立系统，各个微观状态出现的几率相等；
* 最可几分布：出现几率最大的分布，即微观状态数最多的分布；
* 最可几方法：将孤立系统处于平衡态时的分布近似为最可几分布；
* 定域系统：每个粒子局限在一定范围内的系统；
* 玻尔兹曼系统：粒子可以分辨，一个量子态可以容纳的粒子数不受限制的系统；
* 玻色系统：由不可分辨的全同近独立玻色子组成的系统。不受泡利不相容原理的约束，即粒子占据态不受限制；
* 费米系统：由不可分辨的全同近独立费米子组成的系统。受泡利不相容原理的约束，即一个个体量子态上的粒子数最多只能是1；
* 玻尔兹曼分布：玻尔兹曼系统的最可几分布；
* 玻色分布：玻色系统的最可几分布；
* 费米分布：费米系统的最可几分布；

## 经典模型

### 1 计算能量区间内的状态数

#### 1.1 三维准自由粒子，$\varepsilon\in[\varepsilon_0,\varepsilon_0+d\varepsilon]$
* 自由度：$r=3$
* 能量：
$$\varepsilon=\frac{p^2}{2m}$$
* 相体积：
$$\begin{aligned}
\mu&=\iiint_Vdxdydz\iiint_{p_0\leq p\leq p_0+dp}dp_xdp_ydp_z\\
&=V\cdot4\pi p_0^2dp
\end{aligned}$$
&emsp;&emsp;由$p=(2m\varepsilon)^{\frac{1}{2}}$，得$dp=\frac{1}{2}(2m)^{\frac{1}{2}}(\varepsilon)^{-\frac{1}{2}}d\varepsilon$，代入有
$$\mu=2\pi V(2m)^{\frac{3}{2}}\varepsilon^{\frac{1}{2}}d\varepsilon$$
* 状态数：
$$W=\frac{\mu}{h^3}=\frac{2\pi V}{h^3}(2m)^{\frac{3}{2}}\varepsilon^{\frac{1}{2}}d\varepsilon$$

#### 1.2 三维准自由粒子，$0\leq\varepsilon\leq\varepsilon_0$
* 自由度：$r=3$
* 能量：
$$\varepsilon=\frac{p^2}{2m}$$
* 相体积：
$$\begin{aligned}
\mu&=\iiint_Vdxdydz\iiint_{p\leq p_0}dp_xdp_ydp_z\\
&=\frac{4\pi V}{3}p_0^3=\frac{4\pi V}{3}(2m\varepsilon)^{\frac{3}{2}}
\end{aligned}$$
* 状态数：
$$W=\frac{\mu}{h^3}=\frac{4\pi V}{3h^3}(2m\varepsilon)^{\frac{3}{2}}$$

#### 1.3 一维线性谐振子，$0\leq\varepsilon\leq\varepsilon_0$
* 自由度：$r=1$
* 能量：
$$\varepsilon=\frac{p^2}{2m}+\frac{1}{2}m\omega^2x^2$$
&emsp;&emsp;可改写为椭圆方程：
$$\frac{p^2}{2m\varepsilon}+\frac{x^2}{2\varepsilon/m\omega^2}=1$$
* 相体积：
$$\begin{aligned}
\mu&=\iint_{\varepsilon\leq\varepsilon_0}dxpx\\
&=\pi\sqrt{2m\varepsilon}\sqrt{2\varepsilon/m\omega^2}=\frac{2\pi\varepsilon}{\omega}
\end{aligned}$$
* 状态数
$$W=\frac{\mu}{h}=\frac{2\pi\varepsilon}{h\omega}$$

#### 1.4 定点转子，$0\leq\varepsilon\leq\varepsilon_0$
* 自由度：$r=$
* 能量：
$$\varepsilon=\frac{1}{2I}(p_{\theta}^2+\frac{p_{\varphi}^2}{sin^2\theta})$$
&emsp;&emsp;可改写为椭圆方程：
$$\frac{p_{\theta}^2}{2I\varepsilon}+\frac{p_{\varphi}^2}{2I\varepsilon sin^2\theta}=1$$
* 相体积：
$$\begin{aligned}
\mu&=\int_0^{2\pi}d\varphi\int_0^{\pi}d\theta\iint_{\varepsilon}dp_{\theta}dp_{\varphi}\\
&=2\pi\int_0^{\pi}2\pi I\varepsilon sin^2\theta d\theta\\
&=8\pi^2I\varepsilon
\end{aligned}$$
* 状态数
$$W=\frac{\mu}{h^2}=W=\frac{8\pi^2I\varepsilon}{h^2}$$

### 2 计算系统的微观状态数和最可几分布

#### 2.1 最可几分布计算方法
* ln()+Lagrange乘子法:
$$F(\{n_i\},\alpha,\beta)=lnW\{n_i\}+\alpha(N-\sum_in_i)+\beta(E-\sum_in_i\varepsilon_i)$$
&emsp;&emsp;令
$$\frac{\partial F}{\partial n_i}=0,\,\,\,i=1,2,3,\cdots$$
* Stirling公式：
$$N!\approx N^Ne^{-N},\,\,\,N\gg1$$
&emsp;&emsp;或写为
$$ln(N!)\approx N(lnN-1),\,\,\,N\gg1$$

#### 2.2 玻尔兹曼系统
* 微观状态数：
$$W_{MB}\{n_i\}=N!\,\Pi_i\frac{g_i^{n_i}}{n_i!}$$
* 最可几分布（玻尔兹曼分布）：
$$n_i=g_ie^{-\alpha-\beta\varepsilon_i}$$

#### 2.3 玻色系统
* 微观状态数：
$$W_B\{n_i\}=\Pi_i\frac{(n_i+g_i-1)!}{n_i!(g_i-1)!}$$
* 最可几分布（玻色分布）：
$$n_i=\frac{g_i}{e^{\alpha+\beta\varepsilon_i}-1}$$

#### 2.2 费米系统
* 微观状态数：
$$W_F\{n_i\}=\Pi_i\frac{g_i!}{n_i!(g_i-n_i)!}$$
* 最可几分布（费米分布）：
$$n_i=\frac{g_i}{e^{\alpha+\beta\varepsilon_i}+1}$$

#### 2.2 半经典近似系统
* 微观状态数：
$$W_S\{n_i\}=\Pi_i\frac{g_i^{n_i}}{n_i!}$$
* 最可几分布（半经典分布）：
$$n_i=g_ie^{-\alpha-\beta\varepsilon_i}$$
