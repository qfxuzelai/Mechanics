# 第六章 微扰论及其他近似方法

## 一、定态微扰论I：非简并情形

### 1 微扰展开
* 哈密顿量：
$$\hat{H}=\hat{H}_0+\hat{H}'$$
* 能级：
$$E_n=E_n^{(0)}+E_n^{(1)}+E_n^{(2)}+\cdots$$
* 本征函数：
$$\psi_n=\psi_n^{(0)}+\psi_n^{(1)}+\psi_n^{(2)}+\cdots$$

### 2 零级公式
* 零级方程：
$$\hat{H}_0\psi_n^{(0)}=E_n^{(0)}\psi_n^{(0)}$$
* $\hat{H}'$在$\{\psi_n^{(0)}\}$表象中的矩阵元：
$$H_{mn}'=\int\psi_m^{(0)*}\hat{H}'\psi_n^{(0)}d\tau$$
* 微扰论适用条件：
$$|\frac{H_{mn}'}{E_n^{(0)}-E_m^{(0)}}|\ll1$$

### 3 一级微扰公式
* 一级方程：
$$(\hat{H}_0-E_n^{(0)})\psi_n^{(1)}=-(\hat{H}'-E_n^{(1)})\psi_n^{(0)}$$
* 一级微扰能：
$$E_n^{(1)}=H_{nn}'=\int\psi_n^{(0)*}\hat{H}'\psi_n^{(0)}d\tau$$
* 一级微扰波函数：
$$\psi_n^{(1)}=\sum_{m\neq n}\frac{H_{mn}'}{E_n^{(0)}-E_m^{(0)}}\psi_m^{(0)}$$

### 4 二级微扰公式
* 二级方程：
$$(\hat{H}_0-E_n^{(0)})\psi_n^{(2)}=-(\hat{H}'-E_n^{(1)})\psi_n^{(1)}+E_n^{(2)}\psi_n^{(0)}$$
* 二级微扰能：
$$E_n^{(2)}=\sum_{m\neq n}\frac{|H_{mn}'|^2}{E_n^{(0)}-E_m^{(0)}}$$

## 二、定态微扰论II：简并情形

### 1 简并情形

#### &ensp;1.1 零级公式
* 零级方程：
$$\hat{H}_0\psi_n^{(0)}=E_n^{(0)}\psi_n^{(0)}$$
* 本征函数(简并度为k)：
$$\hat{H}_0\varphi_{ni}^{(0)}=E_n^{(0)}\varphi_{ni}^{(0)},\,\,\,i=1,2,\cdots,k$$
* $\hat{H}'$在$\{\varphi_{ni}^{(0)}\}$表象中的矩阵元：
$$H_{ji}'=\int\varphi_{nj}^{(0)*}\hat{H}'\varphi_{ni}^{(0)}d\tau$$

#### &ensp;1.2 一级微扰能与零级波函数
* 假设零级波函数为：
$$\psi_n^{(0)}=\sum_{i=1}^kc_i^{(0)}\varphi_{ni}^{(0)}$$
* 久期方程：
$$|H'-E_n^{(1)}I|=0$$
&emsp;&emsp;其中$H'$为$\hat{H}'$在$\{\varphi_{ni}^{(0)}\}$表象中的矩阵
* 一级微扰能：
$$E_n=E_n^{(0)}+E_{ni}^{(1)},\,\,\,i=1,2,\cdots,k$$
&emsp;&emsp;其中$E_{ni}^{(1)}$为久期方程的特征值。若$E_{ni}^{(1)}$无重根，则简并解除；若$E_{ni}^{(1)}$有部分重根，则简并部分解除。
* 零级波函数：
$$\psi_n^{(0)}=\sum_{i=1}^kc_i^{(0)}\varphi_{ni}^{(0)}$$
&emsp;&emsp;其中$c_i^{(0)}$为久期方程特征向量的各分量。

## 三、经典效应

### 1 Stark效应

&emsp;&emsp;原子或分子在外电场作用下能级和光谱发生分裂的现象

### 2 正常Zeeman效应

* 定义：原子或分子在外磁场作用下能级和光谱发生分裂的现象
* 哈密顿量：
$$\hat{H}=\hat{H}_0+\frac{\mu_BB_0}{\hbar}(\hat{L}_z+2\hat{S}_z)$$
* 能级：
$$E_{nlm_lm_s}=E_{nl}^0+\mu_BB_0(m_l+2m_s)$$

### 3 自旋轨道耦合效应
* 定义：价电子的自旋磁矩受电子轨道运动的内磁场作用产生相互作用能的现象
* 哈密顿量修正项（Thomas项）：
$$\hat{H}_{LS}=\xi(r)\hat{\vec{L}}\cdot\hat{\vec{S}}$$
* 能级：
$$E_{nlj}\approx E_{nl}^0+\frac{\hbar^2}{2}(j(j+1)-l(l+1)-\frac{3}{4})\langle\xi\rangle_{nl}$$

### 4 反常Zeeman效应
* 情形：外磁场较弱时不能忽略$\hat{H}_{LS}$
* 哈密顿量：
$$\hat{H}=\hat{H}_0+\hat{H}_{LS}+\omega_L(\hat{J}_z+\hat{S}_z)$$
* 能级：
$$E_{nlm_lm_s}\approx E_{nlj}+\omega_Lm_j\hbar+\omega_L\langle nljm_j|\hat{S}_z|nljm_j\rangle$$

## 四、量子跃迁

* 含时哈密顿量：
$$\hat{H}(t)=\begin{cases}
    \hat{H}_0 & t\leq0 \\
    \hat{H}_0+\hat{H}'(t) & t>0\\
\end{cases}$$

* 跃迁概率：
$$P_{k'k}(t)=\frac{1}{\hbar^2}|\int_0^tH'_{k'k}(\tau)e^{i\omega_{k'k}\tau}d\tau|^2$$

&emsp;&emsp;其中
$$H'_{k'k}(t)=\langle k'|\hat{H}'(t)|k\rangle$$
$$\omega_{k'k}=\frac{E_{k'}-E_k}{\hbar}$$
