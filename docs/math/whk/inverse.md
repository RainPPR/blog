# 反函数

## 定义

对于二元关系 $(f:X\rightarrow Y)$ 和 $(g:Y\rightarrow X)$，

若 $(\forall x\in X)\{g[f(x)]=x\}$ 且  $(\forall y\in Y)\{f[g(y)]=y\}$，

则称 $g$ 为 $f$ 的反函数，记为 $f^{-1}$。

## 人话

设 $f$ 表示一个函数，其定义域为 $X$、陪域为 $Y$，若存在一函数 $g$，其定义域为 $Y$、陪域为 $X$，且对于 $x\in X$ 有 $g(f(x))=x$、对于任意 $y\in Y$ 有 $f(g(y))=y$，则称 $g$ 为 $f$ 的反函数。

函数 $f$ 的反函数记为 $f^{-1}$，注意此处的 $-1$（次方的写法）并不是 $-1$ 次方，比如 $\sin$ 的反函数 $\arcsin$ 也记为 $\sin^{-1}$。

## 判定

### 定义法

若一函数有反函数，便称此函数可逆。

一函数可逆的充分必要条件是该函数为双射，即同时为单射和满射。

若 $f$ 为一实函数，还可通过水平线测试判断其是否为单射、满射或双射。 

### 水平线测试

在数学里，水平线测试为一测试方法，用来判断一函数是否为单射、满射或双射。

设一带有图像的函数为 $f:X\rightarrow Y$，接着使用 $X\times Y$ 上的水平线：

$$
y_0\in Y,\ \{\langle x,y_0\rangle\in f\mid x\in X\}
$$

- 若函数为单射，则其图像绝不会和任何一条水平线相交超过一次。
- 若函数为满射，则每一水平线和图像至少相交一次。
- 若函数为双射，则每一水平线和图像相交于一点且只有一点。

## 求反函数

### 方法指导

记 $g$ 表示函数 $f$ 的反函数，那么从图像的角度考虑，若 $\langle x,y\rangle\in f$，那么 $\langle y,x\rangle\in g$，因此，我们对于 $y=f(x)=\dots x$，只需要将 $x,y$ 互换，得到的就是反函数的解析式。当然也不能写 $x=\dots y$ 的形式，要化为 $y=\dots x$ 的形式。

### 举个例子

求 $f(x)=2x+1$ 的反函数。

有 $y=f(x)=2x+1$；

交换 $x,y$，即 $x=g(y)=2y+1$；

整理，得 $y=g(y)=\dfrac{1}{2}x-\dfrac{1}{2}$。