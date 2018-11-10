# 第三章 量子力学的矩阵形式与表象理论

## 一、态和力学量的表象

### 1 态矢量

#### &ensp;1.1 态的表象
* 坐标表象：$\Psi(\vec{r},t)=\int c(\vec{p},t)\varphi_p(x)dp$，其中$\varphi_p(x)=\frac{1}{(2\pi\hbar)^{3/2}}e^{\frac{i}{\hbar}\vec{p}\cdot\vec{r}}$
* 动量表象：$c(\vec{p},t)=\int\Psi(\vec{r},t)\varphi_p^*(x)dp$，其中$\varphi_p^*(x)=\frac{1}{(2\pi\hbar)^{3/2}}e^{-\frac{i}{\hbar}\vec{p}\cdot\vec{r}}$

#### &ensp;1.2 Q表象
* 态矢量：设力学量Q的本征函数系为$\{u_n(x)\}$，若$\Psi(x,t)=\sum_na_n(t)u_n(x)$，则在Q表象中的态矢量为
$$\Psi(t)=[a_1(t),a_2(t),\cdots,a_n(t),\cdots]^T$$
* 分量：$a_n(t)=(u_n(x),\Psi(x_t))=\int u_n^*(x)\Psi(x,t)dx$
* 归一化条件：$\Psi^H(t)\Psi(t)=\sum_n|a_n(t)|^2=1$
* 注：$|a_n|^2$表示对$\Psi$态测量力学量Q所得结果为$q_n$的概率

### 2 算符矩阵

#### &ensp;2.1 矩阵元素
&emsp;&emsp;设力学量Q的本征函数系为$\{u_n(x)\}$，则算符$\hat{F}$对应的矩阵元素为
$$\begin{aligned}
F_{m,n}&=(u_m(x),\hat{F}u_n(x))\\
&=\int u_m^*(x)\hat{F}(x,-i\hbar\frac{\partial}{\partial x})u_n(x)dx
\end{aligned}$$

#### &ensp;2.2 性质
* 力学量矩阵是厄米矩阵，即对角元素为实数，非对角元素共轭对称；
* 力学量算符在自身表象中为对角矩阵，其对角元素就是其本征值。

#### &ensp;2.3 实例
* 坐标表象中的矩阵元素
$$\begin{aligned}
    F_{x'x''}&=\int\Psi_{x'}^*(x)\hat{F}(x,-i\hbar\frac{\partial}{\partial x})\Psi_{x''}(x)dx\\
    &=\int\delta(x-x')\hat{F}(x,-i\hbar\frac{\partial}{\partial x})\delta(x-x'')dx\\
    &=\hat{F}(x',-i\hbar\frac{\partial}{\partial x'})\delta(x'-x'')
\end{aligned}$$

### 3 表象变换

#### &ensp;3.1 态矢量的变换
* 力学量Q的本征函数为$\{u_n\}$，体系状态为$\Psi=\sum_na_nu_n$，则态矢量为
$$a=(a_1,a_2,\cdots,a_n,\cdots)^T$$
* 力学量Q'的本征函数为$\{u'_m\}$，体系状态为$\Psi=\sum_ma_mu_m$，则态矢量为
$$a'=(a'_1,a'_2,\cdots,a_m,\cdots)^T$$
* 表象变换：$a'=Sa$，其中幺正矩阵S的矩阵元素为
$$S_{m,n}=(u'_m,u_n)$$

#### &ensp;3.2 算符矩阵的变换
* 力学量F在Q表象(本征函数为$\{u_n\}$)下的矩阵元素为
$$F_{m,n}=(u_m,\hat{F}u_n)$$
* 力学量F在Q表象(本征函数为$\{u'_{\alpha}\}$)下的矩阵元素为
$$F'_{\alpha,\beta}=(u'_{\alpha},\hat{F}u'_{\beta})$$
* 表象变换：$u'_{\alpha}=\sum_mS_{m,\alpha}u_m,\,u'_{\beta}=\sum_nS_{n,\beta}u_n$，故
$$\begin{aligned}
F'_{\alpha,\beta}&=(u'_{\alpha},\hat{F}u'_{\beta})=(\sum_mS_{\alpha,m}u_m,\hat{F}\sum_nS_{\beta,n}u_n)\\
&=\sum_m\sum_nS_{\alpha,m}(u_m,\hat{F}u_n)S^*_{\beta,n}\\
&=(SFS^H)_{\alpha,\beta}
\end{aligned}$$
* 算符变换：$F'=SFS^H==SFS^{-1}$
* 表象变换不改变算符的本征值

## 二、量子力学的矩阵形式

### 1 平均值
$$\overline{F}=(\Psi,\hat{F}\Psi)=\Psi^HF\Psi$$

### 2 本征方程
$$F\Psi=\lambda\Psi\Rightarrow det(F-\lambda I)=0$$
解得$\{\lambda_n\}$和$\{\Psi_n\}$

### 3 薛定谔方程
* 矩阵形式：
$$i\hbar\frac{d\Psi}{dt}=H\Psi$$
* 分量形式：
$$i\hbar\frac{da_m(t)}{dt}=\sum_nH_{m,n}a_n(t),\,n=1,2,3,\cdots$$
其中
$$H_{m,n}=(u_m,\hat{H}u_n)=\int u^*_m(x)\hat{H}u_n(x)dx$$

## 三、狄拉克符号

### 1 态矢量
* 右矢：$|\,\rangle,|\Psi\rangle,|n\rangle,\cdots$
* 左矢：$\langle\,|,\langle\Psi|,\langle n|,\cdots$
* 共轭关系：$\langle\Psi|=|\Psi\rangle^H$

### 2 内积

#### &ensp;2.1 定义
$$\langle\Psi|\Phi\rangle=(\Psi,\Phi)=\int\Psi^*\Phi d\tau$$

#### &ensp;2.2 性质
* 正则性：$\langle\Psi|\Psi\rangle\geq0$，当且仅当$|\Psi\rangle=0$时取等号
* 共轭对称性：$\langle\Psi|\Phi\rangle=\langle\Phi|\Psi\rangle^*$
* 线性：$\langle\Psi|[c_1|\Phi_1\rangle+c_2|\Phi_2\rangle]=c_1\langle\Psi|\Phi_1\rangle+c_2\langle\Psi|\Phi_2\rangle$

#### &ensp;2.3 正交归一性
* 归一性：$\langle\Psi|\Psi\rangle=1$
* 正交性：$\langle\Psi|\Phi\rangle=0$

### 3 算符

#### &ensp;3.1 算符对态矢作用
* 对右矢向右作用，对左矢向左作用：
$$\langle\Phi|\hat{A}|\Psi\rangle=\langle\Phi|[\hat{A}|\Psi\rangle]=[\langle\Phi|\hat{A}]|\Psi\rangle$$
* 对于厄米算符：$[\langle\Psi|\hat{A}]^H=\hat{A}|\Psi\rangle$

#### &ensp;3.2 力学量平均值
$$\overline{A}=\langle\Psi|\hat{A}|\Psi\rangle$$

#### &ensp;3.3 投影算符
* 向态矢$|\xi\rangle$的投影算符：
$$P_{\xi}=|\xi\rangle\langle\xi|$$
* 向态矢$|\xi\rangle$投影：
$$P_{\xi}|\Psi\rangle=|\xi\rangle\langle\xi||\Psi\rangle=\langle\xi|\Psi\rangle|\xi\rangle=a_{\xi}|\xi\rangle$$
* 封闭关系：
$$\sum_{\xi}|\xi\rangle\langle\xi|=I$$

#### &ensp;3.4 常用投影
* $\langle x|\Psi\rangle=\Psi(x)$
* $\langle x|x_0\rangle=\delta(x-x_0)$
* $\langle x|p\rangle=\frac{1}{\sqrt{2\pi\hbar}}e^{\frac{i}{\hbar}px}$
* $\langle p|x\rangle=\langle x|p\rangle^*=\frac{1}{\sqrt{2\pi\hbar}}e^{-\frac{i}{\hbar}px}$

### 4 本征方程与本征态

#### &ensp;4.1 分立谱
* 本征方程：$\hat{F}|n\rangle=\lambda_n|n\rangle$
* 正交归一性：$\langle m|n\rangle=\delta_{m,n}$
* 封闭关系：$\sum_n|n\rangle\langle n|=I$
* 态的展开：$|\Psi\rangle=\sum_n|n\rangle\langle n|\Psi\rangle=\sum_na_n|n\rangle$，其中
$$a_n=\langle n|\Psi\rangle=\int_{-\infty}^{+\infty}\varphi^*_n(x)\Psi(x)dx$$

#### &ensp;4.2 连续谱
* 本征方程：$\hat{F}|\lambda\rangle=\lambda|\lambda\rangle$
* 正交归一性：$\langle\lambda|\lambda'\rangle=\delta(\lambda-\lambda')$
* 封闭关系：$\int_{-\infty}^{+\infty}|\lambda\rangle\langle\lambda|d\lambda=I$
* 态的展开：$|\Psi\rangle=\int_{-\infty}^{+\infty}|\lambda\rangle\langle\lambda|\Psi\rangle d\lambda=\int_{-\infty}^{+\infty}a(\lambda)|\lambda\rangle d\lambda$，其中
$$a(\lambda)=\langle\lambda|\Psi\rangle=\int_{-\infty}^{+\infty}\varphi^*_{\lambda}(x)\Psi(x)dx$$

### 5 力学量的矩阵表示

#### &ensp;5.1 矩阵元素
&emsp;&emsp;设力学量Q的本征函数系为$\{|\lambda_n\rangle\}$，则算符$\hat{F}$对应的矩阵元素为
$$F_{m,n}=\langle\lambda_m|\hat{F}|\lambda_n\rangle$$

#### &ensp;5.2 坐标表象
* 坐标x的矩阵表示：
$$x_{x_1,x_2}=\langle x_1|\hat{x}|x_2\rangle=x_1\delta(x_1-x_2)$$
* 动量p的矩阵表示：
$$p_{x_1,x_2}=\langle x_1|\hat{p}|x_2\rangle=-i\hbar\frac{\partial}{\partial x_1}\delta(x_1-x_2)$$

#### &ensp;5.3 动量表象
* 动量p的矩阵表示：
$$p_{x_1,x_2}=\langle x_1|\hat{p}|x_2\rangle=p_1\delta(p_1-p_2)$$
* 坐标x的矩阵表示：
$$x_{p_1,p_2}=\langle p_1|\hat{x}|p_2\rangle=i\hbar\frac{\partial}{\partial p_1}\delta(p_1-p_2)$$

### 6 薛定谔方程

#### &ensp;5.1 狄拉克符号表示
$$i\hbar\frac{\partial}{\partial t}|\Psi(t)\rangle=H|\Psi(t)\rangle$$

&emsp;&emsp;其中
$$H=\frac{p^2}{2m}+V(x)$$

#### &ensp;5.2 坐标表象
&emsp;&emsp;用$\langle x|$左乘上式，得
$$i\hbar\frac{\partial}{\partial t}\langle x|\Psi(t)\rangle=\langle x|H|\Psi(t)\rangle$$

&emsp;&emsp;化简可得
$$i\hbar\frac{\partial}{\partial t}|\Psi(x,t)\rangle=-\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}\Psi(x,t)+V(x)\Psi(x,t)$$

#### &ensp;5.3 动量表象
&emsp;&emsp;用$\langle p|$左乘上式，得
$$i\hbar\frac{\partial}{\partial t}\langle p|\Psi(t)\rangle=\langle p|H|\Psi(t)\rangle$$

&emsp;&emsp;化简可得
$$i\hbar\frac{\partial}{\partial t}|\Psi(p,t)\rangle=\frac{p^2}{2m}\Psi(p,t)+V(i\hbar\frac{\partial}{\partial p})\Psi(p,t)$$
