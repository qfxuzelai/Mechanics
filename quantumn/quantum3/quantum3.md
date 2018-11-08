# 第三章 量子力学中的力学量

## 一、算符的运算及对易关系

### 1 算符的构成

#### &ensp;1.1 概念
&emsp;&emsp;算符是作用于波函数后将其变成另一个函数的运算符号，代表力学量$F$的算符将记做$\hat{F}$

#### &ensp;1.2 基本假定
&emsp;&emsp;量子力学中任一可观测力学量$F$都可以用线性厄米算符$\hat{F}$来表示

#### &ensp;1.3 构成
* 坐标算符：$\hat{\vec{r}}=\vec{r}\,(\hat{x}=x,\hat{y}=y,\hat{z}=z)$
* 动量算符：$\hat{\vec{p}}=-i\hbar\nabla\,(\hat{p_x}=-i\hbar\frac{\partial}{\partial x},\hat{p_y}=-i\hbar\frac{\partial}{\partial y},\hat{p_z}=-i\hbar\frac{\partial}{\partial z})$
* 一般力学量算符：$F=f(\vec{r},\vec{p})\Rightarrow\hat{F}=f(\hat{\vec{r}},\hat{\vec{p}})=f(\hat{\vec{r}},-i\hbar\nabla)$

#### &ensp;1.4 常见算符
* 轨道角动量算符：$\hat{\vec{L}}=\hat{\vec{r}}\times\hat{\vec{p}}=\vec{r}\times(i\hbar\nabla)=\vec{i}\hat{L}_x+\vec{j}\hat{L}_y+\vec{k}\hat{L}_z$
$$\begin{cases} 
	\hat{L}_x=y\hat{p}_z-z\hat{p}_y\\
	\hat{L}_y=z\hat{p}_x-x\hat{p}_z\\
	\hat{L}_z=x\hat{p}_y-y\hat{p}_x
\end{cases}$$
* 角动量平方算符：$\hat{L}^2=\hat{L}_x^2+\hat{L}_y^2+\hat{L}_z^2$
* 非相对论动能算符：$\hat{T}=\frac{\hat{\vec{p}}^2}{2m}=-\frac{\hbar^2}{2m}\nabla^2$
* 势能算符：$\hat{U}=\hat{U}(\hat{\vec{r}})$
* 能量算符：$\hat{E}=i\hbar\frac{\partial}{\partial t}$
* 哈密顿算符：$\hat{H}=\hat{T}+\hat{V}$

### 2 算符的运算规则
&ensp;设$\Psi,\Phi$为任意波函数，$C_1,C_2$为任意复常数

#### &ensp;2.1 线性算符
* 定义：$\hat{A}(C_1\Psi+C_2\Phi)=C_1\hat{A}\Psi+C_2\hat{A}\Phi$
* 注：并非所有算符都是线性算符，但刻画可观测量的算符都是线性算符

#### &ensp;2.2 算符相等
$$
	\hat{A}\Psi=\hat{B}\Psi\Rightarrow\hat{A}=\hat{B}
$$

#### &ensp;2.3 单位算符
$$
	\hat{I}\Psi=\Psi
$$

#### &ensp;2.4 算符之和
* 定义：$(\hat{A}+\hat{B})\Psi=\hat{A}\Psi+\hat{B}\Psi$
* 交换律：$\hat{A}+\hat{B}=\hat{B}+\hat{A}$
* 结合律：$\hat{A}+(\hat{B}+\hat{C})=(\hat{A}+\hat{B})+\hat{C}$
* 注：两个线性算符之和仍为线性算

#### &ensp;2.5 算符之积
* 定义：$(\hat{A}\hat{B})\Psi=\hat{A}(\hat{B}\Psi)$
* 幂运算：$\hat{A}^n=\hat{A}\hat{A}\cdots\hat{A}$
* 注：算符之积一般不满足交换律，即$\hat{A}\hat{B}\neq\hat{B}\hat{A}$

#### &ensp;2.6 逆算符
* 定义：若由$\hat{A}\Psi=\Phi$能唯一地解出$\Psi$，则可定义$\hat{A}$的逆算符$\hat{A}^{-1}$，满足$\Psi=\hat{A}^{-1}\Phi$
* 性质1：$\hat{A}\hat{A}^{-1}=\hat{A}^{-1}\hat{A}=\hat{I}$
* 性质2：$(\hat{A}\hat{B})^{-1}=\hat{B}^{-1}\hat{A}^{-1}$
* 注：并非所有算符都有逆算符，如投影算符就不存在逆算符

#### &ensp;2.7 算符的复共轭
* 定义：将$\hat{A}$表达式中的所有量换为其复共轭，即为$\hat{A}^*$
* 注：算符的复共轭$\hat{A}^*$与表象有关

#### &ensp;2.8 算符的厄米共轭
* 定义：$\hat{A}^+$，满足$(\Psi(x),\hat{A}^+\Phi(x))=(\hat{A}\Psi(x),\Phi(x))$
* 性质1：$(\hat{A}^+)^+=\hat{A}$
* 性质2：$(\hat{A}+\hat{B})^+=\hat{A}^++\hat{B}^+$
* 性质3：$(\hat{A}\hat{B})^+=\hat{B}^+\hat{A}^+$

#### &ensp;2.9 厄米算符
* 定义：若$\hat{F}^+=\hat{F}$，则称$\hat{F}$为厄米算符
* 性质1：$(\hat{F}\Psi,\Phi)=(\Psi,\hat{F}\Phi)$
* 性质2：厄米算符的本征值都是实数
* 性质3：厄米算符之和仍为厄米算符
* 性质4：厄米算符之积不一定为厄米算符

#### &ensp;2.10 状态的力学量期望
* 定义：若体系的波函数为$\Psi$，则其力学量$A$的期望为$\overline{A}=(\Psi,\hat{A}\Psi)$
* 性质1：体系的任何状态下，其厄米算符对应力学量的期望为实数
* 性质2：若体系的任何状态下，某力学量的期望均为实数，则该力学量对应的算符为厄米算符
* 性质3：若$\hat{A}$为厄米算符，则$\overline{A^2}=(\Psi,\hat{A}^2\Psi)=(\hat{A}\Psi,\hat{A}\Psi)\geq0$

#### &ensp;2.11 幺正算符
$$
	\hat{A}^+=\hat{A}^{-1}\Leftrightarrow\hat{A}\hat{A}^+=\hat{A}^+\hat{A}=\hat{I}
$$

#### &ensp;2.12 算符的函数
&emsp;&emsp;若给定函数$F(x)=\sum_{n=0}^\infty\frac{F^{(n)}(0)}{n!}x^n$，则可定义算符$\hat{A}$的函数
$$
	F(\hat{A})=\sum_{n=0}^\infty\frac{F^{(n)}(0)}{n!}\hat{A}^n
$$

### 3 算符的本征方程及其意义

#### &ensp;3.1 算符的本征方程
$$
	\hat{F}\Psi_{\lambda}=\lambda\Psi_{\lambda}
$$

#### &ensp;3.2 测量的基本假设
* 算符$\hat{F}$的本征值集${\lambda}$就是力学量$F$的测量值集
* $\hat{F}$的本征函数$\Psi_{\lambda}$代表力学量$F$有确定值$\lambda$的状态

#### &ensp;3.3 算符函数的本征值
&emsp;&emsp;若算符$\hat{A}$的本征值为$\lambda$，则算符函数$F(\hat{A})$的本征值为$F(\lambda)$

### 4 算符的对易关系

#### &ensp;4.1 定义
&emsp;&emsp;记$[\hat{A},\hat{B}]=\hat{A}\hat{B}-\hat{B}\hat{A}$，若$[\hat{A},\hat{B}]=0$，即$\hat{A}\hat{B}=\hat{B}\hat{A}$，则称$\hat{A}$和$\hat{B}$对易

#### &ensp;4.2 运算规则
* $[\hat{A},\hat{B}]=-[\hat{B},\hat{A}]$
* $[\hat{A},\hat{B}+\hat{C}]=[\hat{A},\hat{B}]+[\hat{A},\hat{C}]$
* $[\hat{A},\hat{B}\hat{C}]=\hat{B}[\hat{A},\hat{C}]+[\hat{A},\hat{B}]\hat{C}$
* $[\hat{A}\hat{B},\hat{C}]=\hat{A}[\hat{B},\hat{C}]+[\hat{A},\hat{C}]\hat{B}$
* $[\hat{A},[\hat{B},\hat{C}]]+[\hat{B},[\hat{C},\hat{A}]]+[\hat{C},[\hat{A},\hat{B}]]=0$

#### &ensp;4.3 坐标、动量的对易关系
* $[x,y]=[y,z]=[z,x]=0$
* $[\hat{p}_x,\hat{p}_y]=[\hat{p}_y,\hat{p}_z]=[\hat{p}_z,\hat{p}_x]=0$
* $[x,\hat{p}_x]=[y,\hat{p}_y]=[z,\hat{p}_z]=i\hbar$
* $[x,\hat{p}_y]=[x,\hat{p}_z]=\cdots=0$

#### &ensp;4.4 角动量的对易关系
* 角动量算符：如果一个矢量算符的三个分量满足下述对易关系，则这个算符为角动量算符
$$\begin{cases} 
	[\hat{L}_x,\hat{L}_y]=i\hbar\hat{L}_z\\
	[\hat{L}_y,\hat{L}_z]=i\hbar\hat{L}_x\\
	[\hat{L}_z,\hat{L}_x]=i\hbar\hat{L}_y
\end{cases}$$

* 性质：角动量算符的三个分量都和角动量的平方对易
$$
	[\hat{L}_x,\hat{L}^2]=[\hat{L}_y,\hat{L}^2]=[\hat{L}_z,\hat{L}^2]=0
$$

* 轨道角动量算符：$\hat{\vec{L}}=\vec{r}\times\hat{\vec{p}}=\vec{i}\hat{L}_x+\vec{j}\hat{L}_y+\vec{k}\hat{L}_z$
$$\begin{cases} 
	\hat{L}_x=y\hat{p}_z-z\hat{p}_y\\
	\hat{L}_y=z\hat{p}_x-x\hat{p}_z\\
	\hat{L}_z=x\hat{p}_y-y\hat{p}_x
\end{cases}$$

* 轨道角动量和坐标之间的对易关系：$[\hat{l}_{\alpha},\hat{x}_{\beta}]=\varepsilon_{\alpha\beta\gamma}i\hbar\hat{x}_{\gamma}$
$$\begin{array}{lll}
	[\hat{L}_x,\hat{x}]=0 & [\hat{L}_x,\hat{y}]=i\hbar\hat{z} & [\hat{L}_x,\hat{z}]=-i\hbar\hat{y}\\
	[\hat{L}_y,\hat{x}]=-i\hbar\hat{z} & [\hat{L}_y,\hat{y}]=0 & [\hat{L}_y,\hat{z}]=i\hbar\hat{x}\\
	[\hat{L}_z,\hat{x}]=i\hbar\hat{y} & [\hat{L}_z,\hat{y}]=-i\hbar\hat{x} & [\hat{L}_z,\hat{z}]=0
\end{array}$$

* 轨道角动量和动量之间的对易关系$[\hat{l}_{\alpha},\hat{p}_{\beta}]=\varepsilon_{\alpha\beta\gamma}i\hbar\hat{p}_{\gamma}$
$$\begin{array}{lll}
	[\hat{L}_x,\hat{p}_x]=0 & [\hat{L}_x,\hat{p}_y]=i\hbar\hat{p}_z & [\hat{L}_x,\hat{p}_z]=-i\hbar\hat{p}_y\\
	[\hat{L}_y,\hat{p}_x]=-i\hbar\hat{p}_z & [\hat{L}_y,\hat{p}_y]=0 & [\hat{L}_y,\hat{p}_z]=i\hbar\hat{p}_x\\
	[\hat{L}_z,\hat{p}_x]=i\hbar\hat{p}_y & [\hat{L}_z,\hat{p}_y]=-i\hbar\hat{p}_x & [\hat{L}_z,\hat{p}_z]=0
\end{array}$$

### 5 共同本征函数

#### &ensp;5.1 定理
&emsp;&emsp;若算符$\hat{F}$和$\hat{G}$有一组共同本征函数$\phi_n$，且${\phi_n}$组成完全系，则算符$\hat{F}$和$\hat{G}$对易。

#### &ensp;5.2 逆定理
* 非简并：若算符$\hat{F}$和$\hat{G}$均非简并，且$[\hat{F},\hat{G}]=0$，则$\hat{F}$和$\hat{G}$有一组共同本征函数$\phi_n$，且${\phi_n}$组成完全系。
* 简并：若算符$\hat{F}$和$\hat{G}$存在简并，且$[\hat{F},\hat{G}]=0$，则存在$\phi$，使得$\hat{F}\phi=\lambda\phi$和$\hat{G}\phi=\mu\phi$同时成立。

#### &ensp;5.3 推广
&emsp;&emsp;如果一组算符有共同的本征函数，且这些本征函数组成完全系，则这组算符中的任意两个算符均对易。

#### &ensp;5.4 实例
* $\{\hat{x},\hat{y},\hat{z}\}$的共同本征函数为
$$\Psi_{x_0,y_0,z_0}(x,y,z)=\delta(x-x_0)\delta(y-y_0)\delta(z-z_0)$$
* $\{\hat{p}_x,\hat{p}_y,\hat{p}_z\}$的共同本征函数为
$$\Psi_{p_x,p_y,p_z}(x,y,z)=\frac{1}{(2\pi\hbar)^{3/2}}exp[\frac{i}{\hbar}(p_xx+p_yy+p_zz)]$$
* $\{\hat{L}^2,\hat{L}_z\}$的共同本征函数为球谐函数$Y_{lm}(\theta,\varphi)$
* $\{\hat{H},\hat{L}^2,\hat{L}_z\}$的共同本征函数为$\varPsi_{nlm}(r,\theta,\varphi)$

## 二、算符与力学量之间的关系

### 1 厄米算符

#### &ensp;1.1 本征值
* 分立谱：$\hat{F}\Phi_n(x)=a_n\Phi_n(x),\,n=1,2,3,\cdots$
* 连续谱：$\hat{F}\Phi_{\lambda}(x)=\lambda\Phi_{\lambda}(x)$

#### &ensp;1.2 性质
&emsp;&emsp;厄米算符的本征值为实数。

### 2 力学量完全集

#### &ensp;2.1 定义
* 定义：两两对易的，能对体系状态进行不简并地分类标记的，最少数目的一组力学量算符。
* 力学量完全集：$\{\hat{F}_1,\hat{F}_2,\cdots,\hat{F}_n\}$
* 共同本征函数系：$\{\Phi_{a_1,a_2,\cdots,a_n}\}$
* 本征值：$\{a_1,a_2,\cdots,a_n\}$，一组本征值可完全确定体系的一个可能状态。

#### &ensp;2.2 坐标
* 力学量完全集：$\{\hat{x},\hat{y},\hat{z}\}$
* 共同本征函数系：
$$\Psi_{x_0,y_0,z_0}(x,y,z)=\delta(x-x_0)\delta(y-y_0)\delta(z-z_0)$$
* 本征值：$\{x_0,y_0,z_0\}$

#### &ensp;2.3 动量
* 力学量完全集：$\{\hat{p}_x,\hat{p}_y,\hat{p}_z\}$
* 共同本征函数系：
$$\Psi_{p_x,p_y,p_z}(x,y,z)=\frac{1}{(2\pi\hbar)^{3/2}}exp[\frac{i}{\hbar}(p_xx+p_yy+p_zz)]$$
* 本征值：$\{p_x,p_y,p_z\}$

#### &ensp;2.4 转动
* 力学量完全集：$\{\hat{L}^2,\hat{L}_z\}$
* 球坐标系下的角动量算符：
$$\hat{L}_z=-i\hbar\frac{\partial}{\partial\varphi}$$
$$\hat{L}^2=-\hbar^2[\frac{1}{sin\,\theta}\frac{\partial}{\partial\theta}(sin\,\theta\frac{\partial}{\partial\theta})+\frac{1}{sin^2\theta}\frac{\partial^2}{\partial\varphi^2}]$$

### 3 正交性定理

#### &ensp;3.1 正交
$$\int_{\infty}\Psi_1^*(\vec{r})\Psi_2(\vec{r})d\tau=0$$

#### &ensp;3.2 正交性定理
* 定理：厄米算符不同本征值的本征波函数彼此正交，相同本征值存在一组完备的正交本征波函数。
* 分立谱：
$$
(\Phi_l,\Phi_{l'})=\delta_{l,l'}=
\begin{cases}
	0, & l\neq l'\\
	1, & l=l'
\end{cases}
$$
* 连续谱：
$$(\Phi_{\lambda},\Phi_{\lambda'})=\delta(\lambda-\lambda')$$

### 4 本征函数系的完备性

#### &ensp;4.1 定义
&emsp;&emsp;若一个函数系完备，则任何一个满足适当边界条件和连续性要求的波函数均可用这个函数系作展开。

#### &ensp;4.2 封闭关系
* 分立谱：$\sum_n\Phi_n^*(x')\Phi_n(x)=\delta(x'-x)$
* 连续谱：$\int\Phi_{\lambda}^*(x')\Phi_{\lambda}(x)d\lambda=\delta(x'-x)$
* 注意封闭关系和正交性定理的区别。

### 5 力学量的测量

#### &ensp;5.1 概念
* 测量力学量F时所有可能出现的值，都是相应的线性厄米算符$\hat{F}$的本征值。
* 若体系处于$\hat{F}$的本征态$\Psi_n$，则每次测量力学量A所得的结果是完全确定的，即$\lambda_n$；
* 若体系处于$\hat{F}$的本征态叠加态，则单次测量结果的可能值为本征态的本征值，出现的概率为对应本征态在该体系中的叠加系数的平方。

#### &ensp;5.2 测量概率
* 分立谱：若$\Psi(x)=\sum_nc_n\Phi_n(x)$，则单次测量值为$\lambda_n$的概率为$|c_n|^2$，其中$c_n=(\Psi,\Phi_n)$；
* 连续谱：若$\Psi(x)=\int c_{\lambda}\Phi_{\lambda}(x)d\lambda$，则单次测量值出现在区间$[\lambda,\lambda+d\lambda]$的概率为$|c_{\lambda}|^2d\lambda$，其中$c_{\lambda}=(\Psi,\Phi_{\lambda})$。

### 6 力学量的平均值

#### &ensp;6.1 计算方法一
$$\overline{F}=(\Psi(x),\hat{F}\Psi(x))=\int\Psi^*(x)\hat{F}\Psi(x)dx$$

#### &ensp;6.2 计算方法二
* 分立谱：若$\Psi(x)=\sum_nc_n\Phi_n(x)$，则
$$\overline{F}=\sum_n|c_n|^2\lambda_n$$
* 连续谱：若$\Psi(x)=\int c_{\lambda}\Phi_{\lambda}(x)d\lambda$，则
$$\overline{F}=\int|c_{\lambda}|^2\lambda d\lambda$$

## 三、动量算符和角动量算符

### 1 动量算符

#### &ensp;1.1 算符
$$\hat{\vec{p}}=-i\hbar\nabla$$

#### &ensp;1.2 本征值
$$\vec{p}=(p_x,p_y,p_z)$$

#### &ensp;1.3 本征函数
$$\Psi_{\vec{p}}(\vec{r})=\frac{1}{(2\pi\hbar)^{3/2}}e^{\frac{i}{\hbar}\vec{p}\cdot\vec{r}}$$

### 2 z方向角动量算符

#### &ensp;2.1 算符
$$\hat{L}_z=-i\hbar\frac{\partial}{\partial\varphi}$$

#### &ensp;2.2 本征值
$$L_z=m\hbar,\,m=0,\pm1,\pm2,\cdots$$

#### &ensp;2.3 本征函数
* 本征函数：$\Psi_m(\varphi)=\frac{1}{\sqrt{2\pi}}e^{im\varphi}$
* 周期性边界条件：$\Psi(\varphi+2\pi)=\Psi(\varphi)$
* 归一化条件：$\int_0^{2\pi}|\Psi(\varphi)|^2d\varphi=1$

### 3 角动量平方算符

#### &ensp;3.1 算符
$$\hat{L}^2=-\hbar^2[\frac{1}{\sin\,\theta}\frac{\partial}{\partial\theta}(sin\,\theta\frac{\partial}{\partial\theta})+\frac{1}{sin^2\theta}\frac{\partial^2}{\partial\varphi^2}]$$

#### &ensp;3.2 本征值
* $L^2=l(l+1)\hbar^2,\,l=0,1,2,\cdots$
* $L_z=m\hbar,\,m=0,\pm1,\cdots,\pm l$

#### &ensp;3.3 本征函数
* 球谐函数：$Y_{lm}(\theta,\varphi)=N_{lm}P_l^m(cos\,\theta)e^{im\varphi}$
* 正交性：$\int Y_{l'm'}^*(\theta,\varphi)Y_{lm}(\theta,\varphi)d\Omega=\delta_{l'l}\delta_{m'm}$
* 奇偶宇称：$Y_{lm}^*(\theta,\varphi)=(-1)^mY_{l,-m}^*(\theta,\varphi)$
* 实例：
$$Y_{00}=\sqrt{\frac{1}{4\pi}}$$
$$Y_{10}=\sqrt{\frac{3}{4\pi}}cos\,\theta$$
$$Y_{1,\pm1}=\mp\sqrt{\frac{3}{8\pi}}sin\,\theta e^{\pm i\phi}$$

#### &ensp;3.4 说明
* $Y_{lm}(\theta,\varphi)$是$\hat{L}^2$和$\hat{L}_z$的共同本征函数
* l称为轨道量子数，m称为磁量子数；l=0,1,2,3,...的状态分别称为s,p,d,f,...态
* $\hat{L}^2$的本征值$l(l+1)\hbar^2$是(2l+1)度简并的
* 算符集合$\{\hat{L}^2,\hat{L}_z\}$是描述转动的力学量完全集，用量子数{l,m}可以完全确定转动态

## 四、守恒量

### 1 守恒量

#### &ensp;1.1 定义
&emsp;&emsp;在体系的任何状态下，力学量F的平均值与取值概率分布都不随时间变化，则力学量F为体系的守恒量。

#### &ensp;1.2 判定
&emsp;&emsp;若力学量算法$\hat{A}$不含时，且$[\hat{A},\hat{H}]=0$，则A为守恒量，即
$$\frac{d\overline{A}}{dt}=\frac{\overline{\partial\hat{A}}}{\partial t}+\frac{1}{i\hbar}\overline{[\hat{A},\hat{H}]}=0$$

#### &ensp;1.3 与经典守恒量的区别
* 量子体系的守恒量不一定取确定值，而是有确定的期望值和概率分布；
* 量子体系的守恒量不一定都可以同时取确定值。

#### &ensp;1.4 与定态的区别
* 定态是体系的状态，而守恒量是力学量；
* 在定态上，任意力学量的平均值和取值概率分布均不随时间变化；
* 在任意态上，守恒量的平均值和取值概率分布均不随时间变化。

#### &ensp;1.5 实例
* $\hat{H}$为任意状态的守恒量；
* 自由粒子的守恒量：$\hat{x},\,\hat{\vec{p}},\,\hat{T},\,\hat{P},\,\hat{L}_z,\,\hat{L}^2,\,\hat{H}$；
* 中心力场中粒子的守恒量：$\hat{H},\,\hat{L}^2,\,\hat{L}_z$

### 2 守恒量与能级简并

#### &ensp;2.1 定理
* 定理：如果体系有两个不对易的守恒量，则体系的能级一般是简并的。
* 推论：若体系有一个守恒量$\hat{F}$，且体系的某条能级不简并，即对应于某能量本征值E只有一个本整天$\Psi_E$，则$\Psi_E$必为$\hat{F}$的本征态。

#### &ensp;2.2 意义
&emsp;&emsp;当能级出现简并是，可以根据对体系对称性的分析找出其守恒量；通过找到一组包含$\hat{H}$的对易守恒量完全集及其共同本征态，就可以把能级的各简并态标记清楚。

### 3 位力定理
* 意义：定态体系力学量平均值随时间的变化。
* 定理：设粒子处在势场$V{\vec{r}}$中，即Hamilton量为$H=\frac{p^2}{2m}+V(\vec{r})$，则粒子的动量算符在定态上的平均值为
$$\overline{T}=\frac{1}{2}\overline{\vec{r}\cdot\nabla V}$$
* 推论：若势能为坐标的齐次函数$V=\alpha x^n+\beta y^n+\gamma z^n$时，有
$$\overline{T}=\frac{n}{2}\overline{V}$$

## 五、不确定度关系

### 1 不确定度

#### &ensp;1.1 不确定度
* 偏差算符：$\Delta\hat{A}=\hat{A}-\overline{A}$
* 不确定度：$\Delta A=\sqrt{\overline{(\Delta\hat{A})^2}}=\sqrt{\overline{\hat{A}^2}-\overline{A}^2}$

#### &ensp;1.2 不确定度关系
* 定理：在任意态$\Psi$上任意两个力学量$\hat{A}$和$\hat{B}$的不确定度的乘积存在下限：
$$\Delta A\cdot\Delta B\geq\frac{1}{2}|\overline{[\hat{A},\hat{B}]}|=\frac{1}{2}|\Psi,[\hat{A},\hat{B}]\Psi|$$
* 注1：当$[\hat{A},\hat{B}]\neq0$时，除使得$(\Psi,[\hat{A},\hat{B}]\Psi)=0$的特殊态$\Psi$外，在任何态上$\hat{A}$和$\hat{B}$都不能同时取确定值；
* 注2：当$[\hat{A},\hat{B}]=0$时，$\hat{A}$和$\hat{B}$可以同时取确定值（但未必会取）。

#### &ensp;1.3 坐标与动量的不确定度关系
* 公式：$\Delta x\cdot\Delta p_x\leq\frac{\hbar}{2}$
* 意义：粒子在客观上不能同时具有确定的坐标位置和确定的动量。

#### &ensp;1.4 时间与能量的不确定度关系
* 公式：$\Delta E\cdot\Delta t\leq\frac{\hbar}{2}$
* 意义：若粒子在能量状态E只能停留$\Delta t$时间，则此时间段内能量有一弥散$\Delta E\leq\hbar/(2\Delta t)$

### 2 不确定度关系应用
* 估计能级宽度与激发态寿命
* 证明原子中电子的运动不存在轨道
* 说明谐振子的零点能

## 六、中心力场中的粒子运动

### 1 中心力场
* 特点：势能函数$V(r)$球对称，即$V(r)$与方向$\theta,\phi$无关
* 力学量完全集：${\hat{H},\hat{L}^2},\hat{L}_z$
* 本征值问题：
$$\begin{cases}
\hat{H}\Psi_{nlm}=E_{nl}\Psi_{nlm}\\
\hat{L}^2\Psi_{nlm}=l(l+1)\hbar^2\Psi_{nlm}\\
\hat{L}_z\Psi_{nlm}=m\hbar\Psi_{nlm}
\end{cases}$$

### 2 能量本征方程及其求解
* Hamilton量：$\hat{H}=\frac{\hat{p}^2}{2\mu}+V(r)=\frac{\hat{P}_r^2}{2\mu}+\frac{\hat{L}^2}{2\mu r^2}+V(r)$
* 势函数：$\Psi(r,\theta,\varphi)=R(r)Y_{lm}(\theta,\varphi)$
* 宇称：本征态的宇称为$(-1)^l$

### 3 氢原子的本征函数

#### &ensp;3.1 能量本征方程
* 势函数：$V(r)=-\frac{e^2}{r}$
* 能量本征方程：
$$[-\frac{\hbar^2}{2m_1}\nabla_1^2-\frac{\hbar^2}{2m_2}\nabla_2^2+V(r)]\Psi(\vec{r}_1,\vec{r}_2)=E_T\Psi(\vec{r}_1,\vec{r}_2)$$
* 质心坐标和相对坐标下的能量本征方程：
$$[-\frac{\hbar^2}{2M}\nabla_R^2-\frac{\hbar^2}{2\mu}\nabla^2+V(r)]\Psi(\vec{R},\vec{r})=E_T\Psi(\vec{R},\vec{r})$$

#### &ensp;3.2 径向方程
* 方程：$\frac{d^2\chi_l(r)}{dr^2}+[2E+\frac{2}{r}-\frac{l(l+1)}{r^2}]\chi_l(r)=0$
* 径向函数：$R_{nl}(r)=N_{nl}exp(-\frac{\xi}{2})\xi^lF(-n+l+1,2l+2,\xi)$，其中$\xi=\frac{2r}{na}$，F为合流超几何函数。
* 正交归一化条件：$\int_0^\infty R_{nl}(r)R_{n'l'}(r)r^2dr=\delta_{n,n'}\delta_{l,l'}$
* 实例：
$$\begin{array}{ll}
	n=1, & R_{10}(r)=\frac{2}{\sqrt{a^3}}e^{-\frac{r}{a}}\\
	n=2, & R_{20}(r)=\frac{1}{\sqrt{2a^3}}(1-\frac{r}{2a})e^{-\frac{r}{2a}}\\
	& R_{21}(r)=\frac{1}{2\sqrt{6a^3}}\frac{r}{a}e^{-\frac{r}{2a}}
\end{array}$$

#### &ensp;3.3 本征值与本征波函数
* 本征值：
$$\begin{cases}
E_n=-\frac{e^2}{2an^2}=-\frac{13.6}{n^2}eV, & n=1,2,3,\ldots\\
L^2=l(l+1)\hbar^2, & l=0,1,2,\ldots,n-1\\
L_z=m\hbar, & m=0,\pm1,\pm2,\ldots,\pm l
\end{cases}$$
* 本征波函数：$\Psi_{nlm}(r,\theta,\varphi)=R_{nl}(r)Y_{lm}(\theta,\phi)$
* 归一化条件：$\int\Psi_{nlm}^*(r,\theta,\varphi)\Psi_{n'l'm'}(r,\theta,\varphi)d\tau=\delta_{n,n'}\delta_{l,l'}\delta_{m,m'}$

### 4 氢原子的性质

#### &ensp;4.1 能级简并度
* $l=0,1,2,\ldots,n-1$
* $m=0,\pm1,\pm2,\ldots,\pm l$
* $f_n=\sum_{l=0}^{n-1}(2l+1)=n^2$
* 若考虑自旋，则能级简并度为$f_n=2n^2$

#### &ensp;4.2 概率密度分布
* 概率函数：
$$W_{nlm}(r,\theta,\varphi)d\tau=|\Psi_{nlm}(r,\theta,\varphi)|^2r^2sin\theta drd\theta d\varphi$$
* 径向概率分布：
$$\begin{aligned}
W_{nl}(r)dr&=\int_0^{2\pi}\int_0^{\pi}|R_{nl}(r)Y_{lm}(\theta,\varphi)|^2r^2sin\theta drd\theta d\varphi\\
&=R_{nl}^2(r)r^2dr
\end{aligned}$$
* 角向概率分布：
$$\begin{aligned}
W_{lm}(\theta,\varphi)d\Omega&=\int_0^{+\infty}|R_{nl}(r)Y_{lm}(\theta,\varphi)|^2r^2sin\theta drd\theta d\varphi\\
&=Y_{lm}^2(\theta,\varphi)sin\theta d\theta d\varphi
\end{aligned}$$

#### &ensp;4.3 本征态磁矩
* 轨道磁矩：$\mu_z=-\mu_Bm$
* 轨道磁矩算符：$\hat{\vec{\mu}}_l=-\frac{\mu_B}{\hbar}\hat{\vec{L}}$
* 轨道磁矩与外磁场的作用能：$\hat{W}=-\hat{\vec{\mu}}_l\cdot\vec{B}=\frac{\mu_B}{\hbar}\hat{\vec{L}}\cdot\vec{B}$
