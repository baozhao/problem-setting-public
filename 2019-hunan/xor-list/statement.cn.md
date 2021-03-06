# 双向链表练习题

Bobo 有 $n$ 个列表 $L_1, L_2, \dots, L_n$.
初始时，$L_i$ 仅包含元素 $i$, 即 $L_i = [i]$.
他依次执行了 $m$ 次操作。第 $i$ 次操作由两个整数 $a_i, b_i$ 指定, 每次操作分为两步：

1. $L_{a_i} \leftarrow \mathrm{reverse}(L_{a_i} + L_{b_i})$, 其中 $\leftarrow$ 表示赋值，$+$ 表示列表的连接，$\mathrm{reverse}$ 表示列表的反转。例如，$\mathrm{reverse}([1, 2] + [3, 4, 5]) = [5, 4, 3, 2, 1]$.
2. $L_{b_i} \leftarrow []$. 其中 $[]$ 表示空的列表。

输出 $m$ 次操作后， $L_1$ 的元素。

## 输入格式

输入文件包含多组数据，请处理到文件结束。

每组数据的第一行包含两个整数 $n$ 和 $m$.

接下来 $m$ 行，其中第 $i$ 行包含 $2$ 个整数 $a_i, b_i$.

* $1 \leq n, m \leq 10^5$
* $1 \leq a_i, b_i \leq n, a_i \neq b_i$
* $n$ 的总和，$m$ 的总和都不超过 $5 \times 10^5$.

## 输出格式

对于每组数据，先输出 $L_1$ 的长度 $|L_1|$，再输出 $|L_1|$ 个整数，表示 $L_1$ 的元素。

<!--SAMPLES-->
