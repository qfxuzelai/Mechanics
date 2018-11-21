# 第五章 自旋与角动量初步

## 一、电子自旋的实验依据

### 1 Stern-Gerlach实验

#### &ensp;1.1 轨道磁矩
* 玻尔磁子：$\mu_B=\frac{e\hbar}{2m_e}$
* 轨道磁矩：$\hat{\vec{\mu_l}}=-\frac{\mu_B}{\hbar}\hat{\vec{L}}$

#### &ensp;1.2 结论
* 原子在磁场中的取向是量子化的；
* 除轨道角动量外，电子还具有角量子数S=1/2的自旋角动量。

## 二、电子自旋的描述与自旋算符

### 1 电子自旋假设
* 电子存在一种内禀的自旋运动，响应地有自旋角动量和自旋磁矩；
* 电子自旋角动量$\vec{S}$的大小为$|\vec{S}|=\sqrt{S(S+1)}\hbar$，其中S为自旋量子数；
* 电子自旋角动量相对外磁场的取向是空间量子化的。特别的，其在z方向的投影只能取两个值，即$S_z=\pm\frac{\hbar}{2}$

### 2 自旋算符

#### &ensp;2.1 自旋算符
* $\hat{\vec{S}}=\vec{i}\hat{S}_x+\vec{j}\hat{S}_y+\vec{k}\hat{S}_z$
* $\hat{S^2}=\hat{S}_x^2+\hat{S}_y^2+\hat{S}_z^2$

#### &ensp;2.2 对易关系
* $\hat{\vec{S}}\times\hat{\vec{S}}=i\hbar\hat{\vec{S}}$
* 
$$\begin{cases}
        [\hat{S}_x,\hat{S}_y]=i\hbar\hat{S}_z \\
        [\hat{S}_y,\hat{S}_z]=i\hbar\hat{S}_x \\
        [\hat{S}_z,\hat{S}_x]=i\hbar\hat{S}_y 
\end{cases}$$
* $[\hat{S^2},\hat{S}_x]=[\hat{S^2},\hat{S}_y]=[\hat{S^2},\hat{S}_z]=0$

#### &ensp;2.3 共同本征态
* $\{\hat{S^2},\hat{S}_z\}$的共同本征态为$|Sm\rangle$
* 自旋量子数：$S=0,1/2,1,3/2,\cdots$
* 自旋磁量子数：$m=-S,-S+1,\cdots,S-1,S$
* 本征方程：
$$\begin{cases}
    \hat{S^2}|Sm\rangle=S(S+1)\hbar^2|Sm\rangle \\
    \hat{S_z}|Sm\rangle=m\hbar|Sm\rangle
\end{cases}$$

#### &ensp;2.4 电子自旋情况
* $S=\frac{1}{2},m=\pm\frac{1}{2}$
* $\hat{S}_x^2=\hat{S}_y^2=\hat{S}_z^2=\frac{\hbar^2}{4}$
* $\hat{S}^2=\frac{3\hbar^2}{4}$
* 共同本征态：$|Sm\rangle=|\frac{1}{2},\pm\frac{1}{2}\rangle=|\pm\rangle$

### 3 泡利算符

#### &ensp;3.1 泡利算符
* $\hat{\vec{S}}=\frac{\hbar}{2}\hat{\vec{\sigma}}$
* $\hat{\sigma}_x^2=\hat{\sigma}_y^2=\hat{\sigma}_z^2=1$
* $\hat{\sigma}^2=3$

#### &ensp;3.2 对易关系
* $\hat{\vec{\sigma}}\times\hat{\vec{\sigma}}=2i\hat{\vec{\sigma}}$
* 
$$\begin{cases}
        [\hat{\sigma}_x,\hat{\sigma}_y]=2i\hat{\sigma}_z \\
        [\hat{\sigma}_y,\hat{\sigma}_z]=2i\hat{\sigma}_x \\
        [\hat{\sigma}_z,\hat{\sigma}_x]=2i\hat{\sigma}_y 
\end{cases}$$
* $[\hat{\sigma^2},\hat{\sigma}_x]=[\hat{\sigma^2},\hat{\sigma}_y]=[\hat{\sigma^2},\hat{\sigma}_z]=0$

#### &ensp;3.3 反对易关系
$$\begin{cases}
        \hat{\sigma}_x\hat{\sigma}_y+\hat{\sigma}_y\hat{\sigma}_x=0 \\
        \hat{\sigma}_y\hat{\sigma}_z+\hat{\sigma}_z\hat{\sigma}_y=0 \\
        \hat{\sigma}_z\hat{\sigma}_x+\hat{\sigma}_x\hat{\sigma}_z=0
\end{cases}$$

#### &ensp;3.4 分量关系
$$\begin{cases}
        \hat{\sigma}_x\hat{\sigma}_y=-\hat{\sigma}_y\hat{\sigma}_x=i\hat{\sigma}_z \\
        \hat{\sigma}_y\hat{\sigma}_z=-\hat{\sigma}_z\hat{\sigma}_y=i\hat{\sigma}_x \\
        \hat{\sigma}_z\hat{\sigma}_x=-\hat{\sigma}_x\hat{\sigma}_z=i\hat{\sigma}_y
\end{cases}$$

#### &ensp;3.5 本征值
&emsp;&emsp;$\hat{\sigma}_x,\hat{\sigma}_y,\hat{\sigma}_z$的本征值均为$\pm1$。

#### &ensp;3.6 泡利矩阵
* x分量：
$$\sigma_x=\left[
\begin{matrix}
    0 & 1 \\
    1 & 0 
\end{matrix}\right],
|+\rangle_x=\left[
\begin{matrix}
    \frac{\sqrt{2}}{2} \\
    \frac{\sqrt{2}}{2}
\end{matrix}\right],
|-\rangle_x=\left[
\begin{matrix}
    -\frac{\sqrt{2}}{2} \\
    \frac{\sqrt{2}}{2}
\end{matrix}\right]$$
* y分量：
$$\sigma_y=\left[
\begin{matrix}
    0 & -i \\
    i & 0 
\end{matrix}\right],
|+\rangle_y=\left[
\begin{matrix}
    \frac{\sqrt{2}}{2} \\
    \frac{\sqrt{2}}{2}i
\end{matrix}\right],
|-\rangle_y=\left[
\begin{matrix}
    \frac{\sqrt{2}}{2}i \\
    \frac{\sqrt{2}}{2}
\end{matrix}\right]$$
* z分量：
$$\sigma_z=\left[
\begin{matrix}
    1 & 0 \\
    0 & -1 
\end{matrix}\right],
|+\rangle_z=\left[
\begin{matrix}
    1 \\
    0
\end{matrix}\right],
|-\rangle_z=\left[
\begin{matrix}
    0 \\
    1
\end{matrix}\right]$$

### 4 电子自旋态

#### &ensp;4.1 电子的二分量波函数
$$\Psi(\vec{r},t)=\left[
\begin{matrix}
    \Psi_1(\vec{r},t) \\ \Psi_2(\vec{r},t)
\end{matrix}\right]
=c_1\psi_1(\vec{r},t)\left[
\begin{matrix}
    1 \\ 0
\end{matrix}\right]
+c_2\psi_2(\vec{r},t)\left[
\begin{matrix}
    0 \\ 1
\end{matrix}\right]$$

&emsp;&emsp;其中$\Psi_1(\vec{r},t)$对应$S_z=\frac{\hbar}{2}$时的波函数，$\Psi_2(\vec{r},t)$对应$S_z=-\frac{\hbar}{2}$时的波函数。

#### &ensp;4.2 二分量波函数的性质
* 归一性：$\int\Psi^H\Psi d\tau=\int(|\Psi_1|^2+|\Psi_2|^2)d\tau=1$
* 空间概率密度：$w(\vec{r},t)=\Psi^H\Psi=|\Psi_1|^2+|\Psi_2|^2$
* 自旋状态的概率：
$$\begin{cases}
    P(S_z=\frac{\hbar}{2})=\int|\Psi_1|^2d\tau=c_1^2 \\
    P(S_z=-\frac{\hbar}{2})=\int|\Psi_2|^2d\tau=c_2^2
\end{cases}$$

#### &ensp;4.4 非耦合状态
&emsp;&emsp;当自旋和轨道运动非耦合时，二分量波函数可以写为
$$\Psi(\vec{r},t)=\Psi_0(\vec{r},t)\chi(s_z)$$
&emsp;&emsp;其中$\chi(s_z)$为电子的自旋波函数，可写为
$$\chi(s_z)=c_1\chi_{1/2}(s_z)+c_2\chi_{-1/2}(s_z)$$

### 5 电子磁矩
* 玻尔磁子：$\mu_B=\frac{e\hbar}{2m_e}$
* 轨道磁矩：$\hat{\vec{\mu_l}}=-\frac{\mu_B}{\hbar}\hat{\vec{L}}$
* 自旋磁矩：$\hat{\vec{\mu_s}}=-\frac{2\mu_B}{\hbar}\hat{\vec{S}}$
* 电子磁矩与外磁场的相互作用能：$W=-(\hat{\vec{\mu_l}}+\hat{\vec{\mu_s}})\cdot\vec{B}$

### 6 电子在外磁场中的运动
* 若忽略电子的轨道运动，则
$$\hat{H}=\mu_B(\hat{\sigma}_xB_x+\hat{\sigma}_yB_y+\hat{\sigma}_zB_z)$$
* 若外磁场沿$(\theta,\varphi)$方向，则对应的本征态为
$$\begin{cases}
    |(\theta,\varphi)+\rangle=
    \left[\begin{matrix}
        cos(\theta/2)e^{-i\varphi/2} \\
        sin(\theta/2)e^{i\varphi/2}
    \end{matrix}\right]\\\\
    |(\theta,\varphi)-\rangle=
    \left[\begin{matrix}
        -sin(\theta/2)e^{-i\varphi/2} \\
        cos(\theta/2)e^{i\varphi/2}
    \end{matrix}\right]
\end{cases}$$
* 将初始状态用本征态展开：
$$\Psi(0)=c_1|(\theta,\varphi)+\rangle+c_2|(\theta,\varphi)-\rangle$$
* 则t时刻自旋状态为
$$\Psi(t)=c_1e^{-\frac{i\mu_BB_0}{\hbar}t}|(\theta,\varphi)+\rangle+c_2e^{\frac{i\mu_BB_0}{\hbar}t}|(\theta,\varphi)-\rangle$$
* t时刻自旋状态为$\psi$的概率为
$$P(\Psi(t)=\psi)=\langle\psi|\Psi(t)\rangle$$

## 三、角动量的合成

### 1 角动量的合成规则

#### &ensp;1.1 总角动量
&emsp;&emsp;设角动量$\hat{\vec{J_1}}$和$\hat{\vec{J_2}}$相互独立，即它们的各分量是互相对易的，也即
$$[\hat{J}_{1i},\hat{J}_{2j}]=0\,\,\,\,\,\,\,i,j=x,y,z$$
&emsp;&emsp;则矢量和$\hat{\vec{J}}=\hat{\vec{J_1}}+\hat{\vec{J_2}}$也是一个角动量算符，称为总角动量，它满足角动量的一般对易关系
$$\hat{\vec{J}}\times\hat{\vec{J}}=i\hbar\hat{\vec{J}}$$

#### &ensp;1.2 对易关系
* $[\hat{J}_z,\hat{J}_1^2]=[\hat{J}_z,\hat{J}_2^2]=0$
* $[\hat{\vec{J}},\hat{J}_1^2]=[\hat{\vec{J}},\hat{J}_2^2]=0$
* $[\hat{J}^2,\hat{J}_1^2]=[\hat{J}^2,\hat{J}_2^2]=0$

#### &ensp;1.3 力学量完全集
* 非耦合表象：$\{\hat{J}_1^2,\hat{J}_{1z},\hat{J}_2^2,\hat{J}_{2z}\}$
* 耦合表象：$\{\hat{J}_1^2,\hat{J}_2^2,\hat{J}^2,\hat{J}_z\}$

### 2 非耦合表象和耦合表象

#### &ensp;2.1 非耦合表象
* 力学量完全集：$\{\hat{J}_1^2,\hat{J}_{1z},\hat{J}_2^2,\hat{J}_{2z}\}$
* 基底：$|j_1m_1j_2m_2\rangle=|j_1m_1\rangle|j_2m_2\rangle$
* 维数：$(2j_1+1)(2j_2+1)$
* 封闭关系：
$$\sum_{m_1=-j_1}^{j_1}\sum_{m_2=-j_2}^{j_2}|j_1m_1j_2m_2\rangle\langle j_1m_1j_2m_2|=I$$
* 本征方程：
$$\begin{cases}
\hat{J}_1^2|j_1m_1j_2m_2\rangle=j_1(j_1+1)\hbar^2|j_1m_1j_2m_2\rangle \\
\hat{J}_{1z}|j_1m_1j_2m_2\rangle=m_1\hbar|j_1m_1j_2m_2\rangle \\
\hat{J}_2^2|j_1m_1j_2m_2\rangle=j_2(j_2+1)\hbar^2|j_1m_1j_2m_2\rangle \\
\hat{J}_{2z}|j_1m_1j_2m_2\rangle=m_2\hbar|j_1m_1j_2m_2\rangle
\end{cases}$$

#### &ensp;2.2 耦合表象
* 力学量完全集：$\{\hat{J}_1^2,\hat{J}_2^2,\hat{J}^2,\hat{J}_z\}$
* 基底：$|j_1j_2jm\rangle$
* 维数：$\sum_{j=j_{min}}^{j_{max}}(2j+1)=(2j_1+1)(2j_2+1)$
* 封闭关系：
$$\sum_{j=j_{min}}^{j_{max}}\sum_{m=-j}^{j}|j_1j_2jm\rangle\langle j_1j_2jm|=I$$
* 本征方程：
$$\begin{cases}
\hat{J}_1^2|j_1j_2jm\rangle=j_1(j_1+1)\hbar^2|j_1j_2jm\rangle \\
\hat{J}_2^2|j_1j_2jm\rangle=j_2(j_2+1)\hbar^2|j_1j_2jm\rangle \\
\hat{J}^2|j_1j_2jm\rangle=j(j+1)\hbar^2|j_1j_2jm\rangle \\
\hat{J}_z|j_1j_2jm\rangle=m\hbar|j_1j_2jm\rangle
\end{cases}$$

#### &ensp;2.3 表象变换
* 矢量耦合系数：
$$C_{j_1m_1j_2m_2}^{jm}=\langle j_1m_1j_2m_2|j_1j_2jm\rangle$$
* 表象变换：
$$\begin{aligned}
|j_1j_2jm\rangle&=\sum_{m_1=-j_1}^{j_1}\sum_{m_2=-j_2}^{j_2}|j_1m_1j_2m_2\rangle\langle j_1m_1j_2m_2|j_1j_2jm\rangle \\
&=\sum_{m_1=-j_1}^{j_1}\sum_{m_2=-j_2}^{j_2}C_{j_1m_1j_2m_2}^{jm}|j_1m_1j_2m_2\rangle
\end{aligned}$$

### 3 总角动量的本征值谱
* $m=m_1+m_2$
* $j_{max}=j_1+j_2$
* $j_{min}=|j_1-j_2|$
* $j=|j_1-j_2|,|j_1-j_2|+1,\cdots,j_1+j_2$

## 四、全同粒子体系

### 1 多粒子体系的描写

#### &ensp;1.1 波函数

$$\Psi=\Psi(q_1,q_2,\cdots,q_N;t)$$

#### &ensp;1.2 哈密顿量

$$\hat{H}=\sum_{i=1}^N-\frac{\hbar^2}{2m_i}\nabla_i^2+U(q_1,q_2,\cdots,q_N;t)$$

#### &ensp;1.3 薛定谔方程

$$i\hbar\frac{\partial}{\partial t}\Psi=\hat{H}\Psi$$

### 2 全同性假设
* 全同粒子：全部内禀性质完全相同的一类微观粒子。
* 全同性假设：全同粒子体系中任一两个粒子交换都不改变体系的物理状态。

### 3 交换算符与对称性

#### &ensp;3.1 交换算符
* 定义：对$\forall i\neq j$有
$$\hat{P}_{ij}\Psi(\cdots,q_i,\cdots,q_j,\cdots)=\Psi(\cdots,q_j,\cdots,q_i,\cdots)$$
* 性质：$\hat{P}_{ij}$是幺正厄米算符。
* 对称性：
$$\hat{P}_{ij}\Psi=\begin{cases}
    \Psi & 对称波函数 \\
    -\Psi & 反对称波函数
\end{cases}$$

#### &ensp;3.2 玻色子
* 交换对称性：$\hat{P}_{ij}\Psi^S=\Psi^S$
* 自旋量子数为整数：$S_b=m\hbar$
* 满足对易规则：$[b(\vec{q}_1),b(\vec{q}_2)]=0$
* 实例：光子，$\alpha$粒子

#### &ensp;3.3 费米子
* 交换反对称性：$\hat{P}_{ij}\Psi^A=-\Psi^A$
* 自旋量子数为半整数：$S_f=(m+\frac{1}{2})\hbar$
* 满足反对易规则：$\{f(\vec{q}_1),f(\vec{q}_2)\}=0$
* 实例：电子，质子，中子

#### &ensp;3.4 复合粒子
* 多个玻色子构成玻色子
* 偶数个费米子构成玻色子
* 奇数个费米子构成费米子

### 4 全同粒子体系哈密顿量
* 性质：任意交换两个全同粒子，体系的哈密顿量不变
* 公式：
$$\hat{P}_{ij}\hat{H}\hat{P}_{ij}^H=\hat{H}\Leftrightarrow [\hat{P}_{ij},\hat{H}]=0$$

### 5 对称与反对称波函数

#### &ensp;5.1 单粒子近似
&emsp;&emsp;对于无耦合体系，其总波函数为单个粒子波函数的乘积
$$\Psi(q_1,q_2,\cdots,q_N)=\Psi_1(q_1)\Psi_2(q_2)\cdots\Psi_N(q_N)$$

#### &ensp;5.2 两粒子体系
* 玻色子：
$$\begin{cases}
    k_1=k_2时 & \Psi_{kk}^S(q_1,q_2)=\psi_{k}(q_1)\psi_{k}(q_2) \\
    k_1\neq k_2时 & \Psi_{k_1k_2}^S(q_1,q_2)=\frac{1}{\sqrt{2}}[\psi_{k1}(q_1)\psi_{k2}(q_2)+\psi_{k1}(q_2)\psi_{k2}(q_1)]
\end{cases}$$
* 费米子：$k_1\neq k_2$时
$$\Psi_{k_1k_2}^A(q_1,q_2)=\frac{1}{\sqrt{2}}[\psi_{k1}(q_1)\psi_{k2}(q_2)-\psi_{k1}(q_2)\psi_{k2}(q_1)]$$

#### &ensp;5.3 N粒子体系
* 玻色子：
$$\Psi_{n_1\cdots n_N}^S(q_1,\cdots,q_N)=\sqrt{\frac{\prod_in_i!}{N!}}\sum_PP[\psi_{k_1}(q_1)\cdots\psi_{k_N}(q_N)]$$
* 费米子：
$$\Psi_{k_1\cdots k_N}^A(q_1,\cdots,q_N)=\frac{1}{\sqrt{N!}}\left|\begin{matrix}
    \psi_{k_1}(q_1) & \psi_{k_1}(q_2) & \cdots & \psi_{k_1}(q_N) \\
    \psi_{k_2}(q_1) & \psi_{k_2}(q_2) & \cdots & \psi_{k_2}(q_N) \\
    \vdots & \vdots & \ddots & \vdots \\
    \psi_{k_N}(q_1) & \psi_{k_N}(q_2) & \cdots & \psi_{k_N}(q_N) \\
\end{matrix}\right|$$

#### &ensp;5.4 泡利不相容原理
&emsp;&emsp;不可能有两个或更多费米子处于完全相同的量子状态。

## 五、自旋单态、三重态及纠缠态

### 1 单体近似下的电子自旋函数

#### &ensp;1.1 单体近似
$$\chi(s_{1z},s_{2z})=\chi_{m_{s1}}(s_{1z})\chi_{m_{s2}}(s_{2z})$$
&emsp;&emsp;其中$m_{s1},m_{s2}=\pm1/2$

#### &ensp;1.2 对称与反对称自旋函数
$$\begin{cases}
    \chi_S^{(1)}=\chi_{1/2}(s_{1z})\chi_{1/2}(s_{2z}) \\
    \chi_S^{(2)}=\chi_{-1/2}(s_{1z})\chi_{-1/2}(s_{2z}) \\
    \chi_S^{(3)}=\frac{1}{\sqrt{2}}[\chi_{1/2}(s_{1z})\chi_{-1/2}(s_{2z})-\chi_{-1/2}(s_{1z})\chi_{1/2}(s_{2z})] \\
    \chi_A=\frac{1}{\sqrt{2}}[\chi_{1/2}(s_{1z})\chi_{-1/2}(s_{2z})+\chi_{-1/2}(s_{1z})\chi_{1/2}(s_{2z})] \\
\end{cases}$$

#### &ensp;1.3 性质
* $\chi_S^{(1)},\chi_S^{(2)},\chi_S^{(3)},\chi_A$组成正交归一系；
* $\chi_S^{(1)},\chi_S^{(2)},\chi_S^{(3)},\chi_A$是$\hat{S}^2,\hat{S}_z$的本征态，可作为耦合表象$\{\hat{S}_1^2,\hat{S}_2^2,\hat{S}^2,\hat{S}_z\}$的基底。

### 2 三重态和单态
* 自旋三重态：两电子自旋相互平行的态是三重简并的；
* 自旋单态：两电子自旋相互反平行的态是单一的。
* 本征值：

|              |$\hat{S}^2$|$\hat{S}_z$|
|:------------:|:---------:|:---------:|
|$\chi_S^{(1)}$|$2\hbar^2$ |  $\hbar$  |
|$\chi_S^{(2)}$|$2\hbar^2$ |  $-\hbar$ |
|$\chi_S^{(3)}$|$2\hbar^2$ |    $0$    |
|   $\chi_A$   |    $0$    |    $0$    |