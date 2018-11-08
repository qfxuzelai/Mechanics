# 第二章波函数与薛定谔方程

## 一、波函数及其统计诠释

### 1 状态的描述

#### &ensp;1.1 经典力学：质点
* 每一时刻具有确定的$\vec{r},\,\vec{p}(v)$
* 其他力学量可表示为$\vec{r},\,\vec{p}$的函数
* 其状态变化服从牛顿运动定律

#### &ensp;1.2 量子力学：波函数
* 粒子不可能同时具有确定的$\vec{r}$和$\vec{p}$
* 粒子的状态由波函数$\Psi(\vec{r},t)$描述
* 其状态变化服从薛定谔方程

### 2 波粒二象性

#### &ensp;2.1 实物粒子的波粒二象性
* 理论：$\lambda=\frac{h}{p},\,\upsilon=\frac{E}{h}$
* 实验：$C_{60}$分子的干涉实验

#### &ensp;2.2 实物粒子二象性的理解
* 粒子性：与物质相互作用时的“整体性”，具有集中的能量$E$和动量$\vec{p}$
* 波动性：在空间传播时的“可叠加性”，具有波长$\lambda$和波矢$\vec{k}$
* 物质波包观点：夸大了波动性，抹杀了粒子性
* 疎密波观点：夸大了粒子性，抹杀了波动性

### 3 波函数的统计诠释

#### &ensp;3.1 概率波
* 粒子的状态可由波函数$\Psi(\vec{r},t)$完全描述
* 其模平方$|\Psi(\vec{r},t)|^2$表示粒子空间分布的概率密度，波函数本身称为概率振幅

#### &ensp;3.2 波函数的归一
* 空间概率密度：$w(\vec{r},t)=|\Psi(\vec{r},t)|^2$
* 归一化条件：$\int_\infty w(\vec{r},t)d\tau=\int_\infty|\Psi(\vec{r},t)|^2d\tau=1$
* 注1：即使归一化后，波函数仍有一整体位相因子$e^{i\delta}$不能确定
* 注2：某些理想（非物理）情况无法归一，如平面波

#### &ensp;3.3 多粒子波函数
* 波函数：$\Psi(\vec{r}_1,\vec{r}_2,\ldots,\vec{r}_N;t)$
* 归一化条件：$\int_\infty^{(N)}\Psi(\vec{r}_1,\vec{r}_2,\ldots,\vec{r}_N;t)d^3\vec{r}_1d^3\vec{r}_2\ldots d^3\vec{r}_N=1$

#### &ensp;3.4 统计诠释对波函数的要求
* 波函数平方可积
* 满足归一化条件，但不排除某些理想波函数
* $|\Psi(\vec{r})|^2$单值，但不要求$\Psi(\vec{r})$单值
* 一般$\Psi$和$\nabla\Psi$连续，但$\nabla\Psi$在势能无限大跳变处可以不连续

## 二、量子态叠加原理

### 1 量子态及其表象

#### &ensp;1.1 态函数
* 动量表象：$c(\vec{p})=\frac{1}{(2\pi\hbar)^{3/2}}\int\psi(\vec{r})e^{-i\vec{p}\cdot\vec{r}/\hbar}d^3\vec{r}$
* 坐标表象：$\psi(\vec{r})=\frac{1}{(2\pi\hbar)^{3/2}}\int c(\vec{p})e^{i\vec{p}\cdot\vec{r}/\hbar}d^3\vec{p}$
* 注：$\psi(\vec{r})$和$c(\vec{p})$构成傅里叶变换对

#### &ensp;1.2 表象
* 含义：量子力学中态和力学量的表示方式
* 常用表象：坐标表象$\psi(\vec{r})$，动量表象$c(\vec{p})$等

### 2 量子态叠加原理

#### &ensp;2.1 原理
&emsp;&emsp;若$\Psi_1,\Psi_2,\ldots,\Psi_n$是体系可能状态，则$\Phi=\sum_nc_n\Psi_n$也是体系的可能状态，其中$c_n$为复常数

#### &ensp;2.2 讨论
* 态矢量集合{$\Psi$}对线性叠加封闭，故构成一个线性空间
* 态叠加原理要求态矢量的时间演化方程为线性齐次方程
* 叠加态$\Phi=\sum_nc_n\Psi_n$处于态$\Psi_k$的概率与$|c_k|^2$成正比

#### &ensp;2.3 与经典叠加原理的区别
* $\Psi$和$c\Psi$描述的是同一个状态
* 波函数无直接物理意义，其叠加为概率波函数的叠加，而非概率密度的叠加

## 三、薛定谔方程

### 1 建立

#### &ensp;1.1 算符
* 能量算符：$E\to i\hbar\frac{\partial}{\partial t}$
* 动量算符：$p\to -i\hbar\nabla$

#### &ensp;1.2 方程
* 能量守恒：$E=\frac{\vec{p}^2}{2m}+U(\vec{r},t)$
* 薛定谔方程：$i\hbar\frac{\partial\Psi}{\partial t}=-\frac{\hbar^2}{2m}\nabla^2\Psi+U(\vec{r},t)\Psi$

### 2 讨论

#### &ensp;2.1 连续性方程
* 空间概率密度：$w(\vec{r},t)=|\Psi(\vec{r},t)|^2=\Psi^*(\vec{r},t)\Psi(\vec{r},t)$
* 概率流密度矢量：$\vec{J}=\frac{i\hbar}{2m}(\Psi\nabla\Psi^* -\Psi^*\nabla\Psi)$
* 连续性方程：$\frac{\partial w}{\partial t}+\nabla\cdot\vec{J}=0$
* 物理意义：概率守恒，单位时间内体积V中增加的概率，等于从边界面流入V的概率通量

#### &ensp;2.2 质量守恒定律与电荷守恒定律
* 质量守恒：$\frac{\partial w_m}{\partial t}+\nabla\cdot\vec{J_m}=0$
* 电荷守恒：$\frac{\partial w_q}{\partial t}+\nabla\cdot\vec{J_q}=0$

#### &ensp;2.3 说明
* 薛定谔方程是量子力学的一个基本假设
* 薛定谔方程是线性偏微分方程，满足态叠加原理

### 3 定态薛定谔方程

#### &ensp;3.1 定态薛定谔方程
* 定义：粒子的势能函数$U$与时间$t$无关的稳定势场问题
* 定态波函数：$\Psi(\vec{r},t)=e^{-\frac{iE}{\hbar}t}\psi(\vec{r})$
* 定态薛定谔方程：$-\frac{\hbar^2}{2m}\nabla^2\psi+U(\vec{r})\psi=E\psi$

#### &ensp;3.2 定态与非定态
* 定态：体系的能量有确定值的状态
* 非定态：由若干个能量不同的本征态叠加所形成的的态，即$\Psi(\vec{r},t)=\sum_Ec_E\psi(\vec{r})e^{-\frac{iE}{\hbar}t}$

#### &ensp;3.3 定态的特征
* 粒子的空间概率密度$\omega(\vec{r})$和概率流密度$\vec{J}$不随时间改变
* 任何不显含时力学量的平均值不随时间改变
* 任何不显含时力学量的测值概率分布不随时间改变

### 4 哈密顿算符
* 薛定谔方程的普遍表达：$i\hbar\frac{\partial\Psi}{\partial t}=\hat{H}\Psi$
* 单粒子的哈密顿算符：$\hat{H}=-\frac{\hbar^2}{2m}\nabla^2+U(\vec{r})$
* 多粒子的汉密顿算符：$\hat{H}=\sum_{i=1}^N(-\frac{\hbar^2}{2m_i}\nabla_i^2+U_i(\vec{r_i}))+V(\vec{r_1},\vec{r_2},\ldots,\vec{r_N})$
* 能量本征方程：$\hat{H}\Psi=E\Psi$

## 四、一维运动问题的一般分析

### 1 一维定态薛定谔方程
* 方程：$[-\frac{\hbar}{2m}\frac{\partial^2}{\partial x^2}+U(x)]\psi(x)=E\psi(x)$
* 其中$E,\,U(x)$均为实数

### 2 一维定态的分类

#### &ensp;2.1 束缚态与非束缚态
* 束缚态：粒子局限在有限的空间中，即$lim_{x\to\pm\infty}\psi(x)=0$
* 非束缚态：粒子可以出现在无限远处的状态，即$lim_{x\to+\infty}\psi(x)>0$或$lim_{x\to-\infty}\psi(x)>0$

#### &ensp;2.2 简并与非简并
* 定义：若对于给定的能级$E$，只有一个线性无关的波函数存在，则称该能级是非简并的；否则称其为简并的
* 简并度：简并态中线性独立的波函数个数称为其简并度

### 3 一维定态薛定谔方程的性质

#### &ensp;定理1 共轭定理
* 若$\psi(x)$是定态方程的解，则$\psi(x)^*$也是方程的解，且能量相同
* 推论：若某能量本征值$E$的解无简并，则可取为实解

#### &ensp;定理2 
&emsp;&emsp;对于任意能量本征值$E$，总可以找到定态方程的一组实解，其线性组合可以表示属于$E$的任何解

#### &ensp;定理3 反射定理

&emsp;3.1 定理

&emsp;&emsp;若$U(x)$具有空间反射不变性，即$U(x)=U(-x)$，那么若$\psi(x)$是方程的解，则$\psi(-x)$也是方程的解，且能量相同

&emsp;3.2 宇称

* 空间反射算符：$\hat{P}\Psi(x)=\Psi(-x)$
* 本征方程：$\hat{P}\Psi(x)=\pi\Psi(x)$
* 宇称：空间反射算符的本征值，$\pi=1$为偶宇称，$\pi=-1$为奇宇称

&emsp;3.3 推论

&emsp;&emsp;若$U(x)=U(-x)$，且某能量本征值$E$的解无简并，则该解必有确定的宇称

#### &ensp;定理4 
&emsp;&emsp;若$U(x)=U(-x)$，则对于任意能量本征值$E$，总可以找到一组有确定宇称的解，其线性组合可以表示属于$E$的任何解

#### &ensp;定理5 
&emsp;&emsp;若$U(x)$的不连续点跳变值有限，则能量本征函数$\psi(x)$及其导数$\psi(x)'$连续

#### &ensp;定理6 Wronskian定理
* Wronskian行列式：$\psi_1(x)'\psi_2(x)-\psi_2(x)'\psi_1(x)$称为$\psi_1(x),\,\psi_2(x)$的Wronskian行列式
* 若$\psi_1(x)$和$\psi_2(x)$均为方程的解且能量相同，则$\psi_1(x),\,\psi_2(x)$的Wronskian行列式为与x无关的常数，即$\psi_1(x)'\psi_2(x)-\psi_2(x)'\psi_1(x)=c$

#### &ensp;定理7 不简并定理
* 定理：设$U(x)$为规则势场（即无奇点），若粒子存在束缚态，则该状态一定是非简并的
* 注：对于常见的非规则势场（如无限深势阱，$\delta$势阱），上述定理仍然成立

## 五、一维无限深势阱和方势阱

### 1 一维无限深势阱

#### &ensp;1.1 势能函数
$$U(x)=\begin{cases} 
		0, & 0<x<a\\
		\infty, & x<0,x>a
\end{cases}$$

#### &ensp;1.2 定态薛定谔方程
* 阱内：$-\frac{\hbar^2}{2m}\frac{d^2}{dx^2}\psi(x)=E\psi(x)$
* 阱外：$(-\frac{\hbar^2}{2m}\frac{d^2}{dx^2}+\infty)\psi(x)=E\psi(x)$

#### &ensp;1.3 列写通解
* 阱内：$\psi(x)=Asin(kx+\delta)$，其中$k=\sqrt{\frac{2mE}{\hbar^2}}$
* 阱外：$\psi(x)=0$

#### &ensp;1.4 边界条件
* 利用边界条件$\psi(0)=0,\,\psi(x)=0$，得$ka=n\pi,\,n=1,2,3,\ldots$
* 能级：$E_n=\frac{\hbar^2\pi^2n^2}{2ma^2},\,n=1,2,3,\ldots$
* 波函数：$\psi_n(x)=A_nsin(\frac{n\pi}{a}x),\,n=1,2,3,\ldots$

#### &ensp;1.5 归一化条件
* 利用归一化条件$\int_0^a|\psi_n(x)|^2dx=1$，得$A_n=\sqrt{\frac{2}{a}}$
* 归一化波函数：
$$\Psi_n(x,t)=\begin{cases} 
		\sqrt{\frac{2}{a}}sin(\frac{n\pi}{a}x)e^{-\frac{iE_n}{\hbar}t}, & 0<x<a\\
		0, & x<0,x>a
\end{cases},\,n=1,2,3,\dots$$

#### &ensp;1.6 讨论
* 能量本征值：无限深势阱的能量是量子化的，其最低能级为$E_1=\frac{\hbar^2\pi^2}{2ma^2}$
* 本征函数系：本征函数是两两正交的，即$\int_0^a\psi_m^*(x)\psi_n(x)dx=\delta_{m,n}$

### 2 有限深对称方势阱

#### &ensp;2.1 势能函数
$$U(x)=\begin{cases} 
		0, & |x|<\frac{a}{2}\\
		U_0, & |x|>\frac{a}{2}
\end{cases}$$

#### &ensp;2.2 定态薛定谔方程
&emsp;&emsp;考虑束缚态，即$0<E<U_0$时
* 阱内：$\frac{d^2\psi(x)}{dx^2}+k^2\psi(x)=0$，其中$k=\sqrt{\frac{2mE}{\hbar^2}}$
* 阱外：$\frac{d^2\psi(x)}{dx^2}-\beta^2\psi(x)=0$，其中$\beta=\sqrt{\frac{2m(U_0-E)}{\hbar^2}}$

#### &ensp;2.3 列写通解
* 阱内：$\psi(x)=Acos(kx)+Bsin(kx)$
* 阱外：$\psi(x)=Ce^{\beta x}+De^{-\beta x}$

#### &ensp;2.4 物理分析
* 束缚态条件：注意到$E<U_0$为束缚态，有$lim_{x\to\pm\infty}\psi(x)=0$，故波函数为
$$\psi(x)=\begin{cases} 
		Ce^{\beta x}, & x<-\frac{a}{2}\\
		Acos(kx)+Bsin(kx), & -\frac{a}{2}<x<\frac{a}{2}\\
        De^{-\beta x}, & x>-\frac{a}{2}
\end{cases}$$
* 势能对称性：注意到$U(x)=U(-x)$，故定态波函数必有确定的宇称，下分偶宇称和奇宇称分别进行讨论

#### &ensp;2.5 边界条件
* 偶宇称：$B=0,\,C=D$，由边界条件得
$$\begin{cases} 
		Acos(\frac{ka}{2})=De^{-\frac{\beta a}{2}}\\
		-kAsin(\frac{ka}{2})=-\beta De^{-\frac{\beta a}{2}}
\end{cases}\Rightarrow k\,tan(\frac{ka}{2})=\beta$$
* 奇宇称：$A=0,\,C=-D$，由边界条件得
$$\begin{cases} 
		Bsin(\frac{ka}{2})=De^{-\frac{\beta a}{2}}\\
		kBsin(\frac{ka}{2})=-\beta De^{-\frac{\beta a}{2}}
\end{cases}\Rightarrow k\,cot(\frac{ka}{2})=-\beta$$
* 图解法：引入$\xi=\frac{ka}{2},\,\eta=\frac{\beta a}{2}$，采用图解法解如下超越方程
$$\begin{cases} 
		\eta=\xi\,tan\xi\\
		\eta^2+\xi^2=\frac{mU_0a^2}{2\hbar^2}
\end{cases}or\,
\begin{cases} 
		\eta=-\xi\,cot\xi\\
		\eta^2+\xi^2=\frac{mU_0a^2}{2\hbar^2}
\end{cases}$$
* 能级：$E_n=\frac{2\hbar^2}{ma^2}\xi_n^2$

#### &ensp;2.6 讨论
&emsp;&emsp;由图解法可得：
* 无论势阱深浅，至少存在一个束缚态（基态）
* 能级的宇称奇偶相间，最低能级为偶宇称
* 有限深势阱的各能级都低于无限深势阱能级；当$n\to\infty$时，各能级趋近于无限深势阱的响应能级
* 束缚态能级总数$N=1+[\frac{a}{\hbar\pi}\sqrt{2mU_0}\,]$

### 3 束缚态与离散谱

#### &ensp;3.1 束缚态能级
&emsp;&emsp;束缚能量本征态的能级是离散的

#### &ensp;3.2 波函数性质
* 在经典允许区，即$U(x)<E$时：波函数为震荡函数（$sin\,kx,cos\,kx$），$\psi(x)$总是向$x$轴弯曲
* 在经典禁区，即$U(x)>E$时：波函数为s单调函数（$e^{\pm\beta x}$），$\psi(x)$总是背离$x$轴弯曲

#### &ensp;3.3 基态与激发态
* 基态：除$\pm\infty$外，在$x$有限的区域内基态波函数无节点
* 激发态：随能级递增，波函数节点数一次增加一个

## 六、量子隧穿效应

### 1 隧穿效应

#### &ensp;1.1 势能函数
$$U(x)=\begin{cases} 
		U_0, & 0<x<a\\
		0, & x<0,\,x>a
\end{cases}$$
&emsp;&emsp;考虑$0<E<U_0$时的情况

#### &ensp;1.2 定态薛定谔方程
$$\begin{cases} 
		\frac{d^2\psi_1(x)}{dx^2}+\frac{2mE}{\hbar^2}\psi_1(x)=0 & x<0\\
		\frac{d^2\psi_2(x)}{dx^2}-\frac{2m(U_0-E)}{\hbar^2}\psi_2(x)=0, & 0<x<a\\
		\frac{d^2\psi_3(x)}{dx^2}+\frac{2mE}{\hbar^2}\psi_3(x)=0 & x>a
\end{cases}$$

#### &ensp;1.3 列写通解
$$\begin{cases} 
		\psi_1(x)=e^{ikx}+Be^{-ikx} & x<0\\
		\psi_2(x)=Ce^{\kappa x}+De^{-\kappa x}, & 0<x<a\\
		\psi_3(x)=Se^{ikx} & x>a
\end{cases}$$
&emsp;&emsp;其中$k=\sqrt{\frac{2mE}{\hbar^2}},\,\kappa=\sqrt{\frac{2m(U_0-E)}{\hbar^2}}$

#### &ensp;1.4 物理分析
* 透射波：从物理上分析，透射波$\psi_3(x)$中只可能存在向右传播的$e^{ikx}$波，因此不存在$e^{-ikx}$项
* 概率流密度：$\vec{J}=\frac{i\hbar}{2m}(\Psi\nabla\Psi^* -\Psi^*\nabla\Psi)$，从而有
$$J_i=|1|^2\frac{\hbar k}{m}=v,\,J_r=|B|^2\frac{\hbar k}{m}=|B|^2v,\,J_t=|S|^2\frac{\hbar k}{m}=|S|^2v$$
* 透射概率：$T=\frac{J_t}{J_i}=|S|^2$
* 反射概率：$R=\frac{J_r}{J_i}=|B|^2$

#### &ensp;1.5 边界条件
* 利用边界条件有：
$$\begin{cases} 
		\psi_1(0)=\psi_2(0)\\
		\psi_1'(0)=\psi_2'(0)\\
		\psi_2(a)=\psi_3(a)\\
		\psi_2'(a)=\psi_3'(a)
\end{cases}\Rightarrow
\begin{cases} 
		1+B=C+D\\
		ik(1-B)=\kappa(C-D)\\
		Ce^{\kappa a}+De^{-\kappa a}=Se^{ika}\\
		\kappa Ce^{\kappa a}-\kappa De^{-\kappa a}=ikSe^{ika}
\end{cases}$$
* 解得：
$$T=|S|^2=\frac{4k^2\kappa^2}{(k^2+\kappa^2)^2sh^2\kappa a+4k^2\kappa^2}\\
R=|B|^2=\frac{(k^2+\kappa^2)^2sh^2\kappa a}{(k^2+\kappa^2)^2sh^2\kappa a+4k^2\kappa^2}
$$

#### &ensp;1.6 讨论
* 概率非负：分析下式可知 $0<T<1$
$$
T=[1+\frac{(k^2+\kappa^2)^2}{4k^2\kappa^2}sh^2\kappa a]^{-1}
=[1+\frac{1}{4\frac{E}{U_0}(1-\frac{E}{U_0})}sh^2\kappa a]^{-1}$$
* 概率守恒：$R+T=1$
* 近似公式：若满足条件$\kappa a\gg1$，利用$sh\,\kappa a\approx\frac{1}{2}e^{\kappa a}\gg1$可得
$$
T\approx\frac{16k^2\kappa^2}{(k^2+\kappa^2)^2}e^{-2\kappa a}\approx T_0e^{-\frac{2a}{\hbar}\sqrt{2m(U_0-E)}}
$$
&emsp;&emsp;分析可知$T$敏感地依赖于势垒高度$U_0$，宽度$a$，粒子质量$m$和能量$E$
* 粒子隧穿一般形状势垒的透射概率：
$$T\approx T_0e^{-\frac{2}{\hbar}\int_a^b\sqrt{2m(U(x)-E)}dx}$$

### 2 共振隧穿
&emsp;&emsp;考虑$E>U_0$时的情况

#### &ensp;2.1 定态薛定谔方程
$$\begin{cases} 
		\frac{d^2\psi_1(x)}{dx^2}+\frac{2mE}{\hbar^2}\psi_1(x)=0 & x<0\\
		\frac{d^2\psi_2(x)}{dx^2}+\frac{2m(E-U_0)}{\hbar^2}\psi_2(x)=0, & 0<x<a\\
		\frac{d^2\psi_3(x)}{dx^2}+\frac{2mE}{\hbar^2}\psi_3(x)=0 & x>a
\end{cases}$$

#### &ensp;2.2 列写通解
$$\begin{cases} 
		\psi_1(x)=e^{ikx}+Be^{-ikx} & x<0\\
		\psi_2(x)=Ce^{ik'x}+De^{-ik'x}, & 0<x<a\\
		\psi_3(x)=Se^{ikx} & x>a
\end{cases}$$
&emsp;&emsp;其中$k=\sqrt{\frac{2mE}{\hbar^2}},\,k'=\sqrt{\frac{2m(E-U_0)}{\hbar^2}}$

#### &ensp;2.3 物理分析
* 注意到在$0<E<U_0$时，$\kappa=\sqrt{\frac{2m(U_0-E)}{\hbar^2}}$，故可将下关系式代入前表达式即可求得透射概率$T$
$$
\kappa=ik,\,sh(ik'a)=i\,sin(k'a)
$$
* 透射概率：
$$
T=[1+\frac{1}{4}(\frac{k}{k'}-\frac{k'}{k})^2)sin^2k'a]^{-1}
$$
&emsp;&emsp;分析可知：当$k'a=n\pi$时，$T=1$

### 3 方势阱的反射、透射与共振

#### &ensp;3.1 物理分析
* 将$U_0=-U_0,\,k’=\sqrt{\frac{2m(E+U_0)}{\hbar^2}}$代入前表达式可得
$$
T=[1+\frac{1}{4}(\frac{k}{k'}-\frac{k'}{k})^2)sin^2k'a]^{-1}
=[1+\frac{sin^2k'a}{4\frac{E}{U_0}(1+\frac{E}{U_0})}]^{-1}
$$

#### &ensp;3.2 讨论
* 若$U_0=0$，则$T=1$
* 若$U_0\neq0$，则$T<1,\,|R|^2\neq0$
* 当$k'a=n\pi,\,n=1,2,3,\ldots$时，$T=1$，称为共振透射，此时有共振能级
$$
E_n=-U_0+\frac{n^2\pi^2\hbar^2}{2ma^2},\,n=1,2,3,\ldots
$$
* 当$k'a=(n+\frac{1}{2})\pi,\,n=1,2,3,\ldots$时，反射最强

## 七、一维谐振子

### 1 势能函数
$$
U(x)=\frac{1}{2}m\omega^2x^2
$$

### 2 定态薛定谔方程
$$
(-\frac{\hbar^2}{2m}\frac{d^2}{dx^2}+\frac{1}{2}m\omega^2x^2)\psi(x)=E\psi(x)
$$

### 3 方程求解

#### &ensp;3.1 无量纲变换
&emsp;&emsp;令$\xi=\sqrt{\frac{m\omega}{\hbar}}x=\alpha x,\,\lambda=\frac{2E}{\hbar\omega}$，则原方程化为
$$
\frac{d^2\psi}{d\xi^2}+(\lambda-\xi^2)\psi(\xi)=0
$$

#### &ensp;3.2 渐近分析
&emsp;&emsp;当$\xi\to\pm\infty$时，有$\frac{d^2\psi}{d\xi^2}\approx\xi^2\psi(\xi)$，从而$\psi(\xi)\sim e^{-\frac{1}{2}\xi^2}$，故设$\psi(\xi)=H(\xi)e^{-\frac{1}{2}\xi^2}$，代入原方程得Hermite方程
$$
\frac{d^2H}{d\xi^2}-2\xi\frac{dH}{d\xi}+(\lambda-1)H=0
$$

#### &ensp;3.3 级数解法
* 对$H(\xi)$做幂级数展开$H(\xi)=\sum_{k=0}^\infty a_k\xi^k$，代入Hermite方程得到递推关系
$$
a_{k+2}=\frac{2k-(\lambda-1)}{(k+2)(k+1)}a_k,\,k=0,1,2,\ldots
$$
* 取$\lambda=2n+1,\,n=0,1,2,\ldots$，则$a_{k+2}=\frac{2(k-n)}{(k+2)(k+1)}a_k$，解得
$$
H_n(\xi)=(-1)^ne^{\xi^2}\frac{d^n}{d\xi^n}e^{-\xi^2},\,n=0,1,2,\ldots
$$
* 简单的Hermite多项式：$H_0(\xi)=1,\,H_1(\xi)=2\xi,\,H_2(\xi)=4\xi^2-2$

### 4 能级和波函数

#### &ensp;4.1 能级
$$
E_n=(n+\frac{1}{2})\hbar\omega,\,n=0,1,2,\ldots
$$

#### &ensp;4.2 波函数
$$
\psi_n(x)=A_nH_n(\xi)e^{-\frac{1}{2}\xi^2}=A_nH_n(\alpha x)e^{-\frac{1}{2}\alpha^2x^2},\,n=0,1,2,\ldots
$$
&emsp;&emsp;其中$\alpha=\sqrt{\frac{m\omega}{\hbar}}$

#### &ensp;4.3 归一化系数
$$
A_n=\sqrt{\frac{\alpha}{\sqrt{\pi}2^nn!}},\,n=0,1,2,\ldots
$$

#### &ensp;4.4 Hermite多项式
$$
H_n(\xi)=(-1)^ne^{\xi^2}\frac{d^n}{d\xi^n}e^{-\xi^2},\,n=0,1,2,\ldots
$$

#### &ensp;4.5 性质
* 宇称：$\psi_n(-x)=(-1)^n\psi_n(x)$
* 正交性：$\int_{-\infty}^{+\infty}\psi_m(x)\psi_n(x)dx=\delta_{mn}$

### 5 讨论
* 零点能：$E_0=\frac{1}{2}\hbar\omega$
* 能量量子化：$E_{n+1}-E_n=\hbar\omega$，源于粒子德布罗意波的自身干涉
* 宇称：能量本征态的宇称奇偶相间，基态为偶宇称
* 节点：$\psi_n(x)$有n个节点
* 与经典谐振子的比较：n较小时，概率分布与经典谐振子完全不同；$n\to\infty$时，概率分布趋于经典概率分布，能量量子化趋于能量取连续值
* 对应原理：在大量子数极限下，量子论将渐近地趋于经典理论
