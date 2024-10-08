# 单调数据结构优化

咕咕咕。

## 最大字段和问题

我们将问题拆解，分别考虑上下界。

##### 处理长度下界

考虑类似最大字段和的方法一：

$$
F(x)=\max_{y<x}\{S(x)-S(y)\}=S(x)-\min_{y<x}S(y)
$$

我们加上长度下界要求，注意到 $x-y$ 就是长度，

$$
F(x)=S(x)-\min_{x-y\ge L}S(y)=S(x)-\min_{y\le x-L}S(y)
$$

我们枚举 $x$，将 $y=x-L$ 的 $S(y)$ 加入，打擂台维护最小值即可。

##### 处理长度上界

类似的，

$$
F(x)=S(x)-\min_{x-y\le R}S(y)=S(x)-\min_{y\ge x-R}S(y)
$$

注意到是经典的单调队列优化转移的形式。

##### 完整的长度限制

我们总结一下，

$$
F(x)=S(y)-\min_{L\le x-y\le R}S(y)=S(x)-\min_{x-R\le y\le x-L}S(y)
$$

每次枚举加入 $y=x-L$ 维护单调队列，转移即可，时间复杂度是 $\mathcal O(N)$ 的。