### C - Swaps
#### 题目
给出长度为 N 的两个数组 A 和 B 问把 A 排成 $A_i \leq B_i, \forall i$ 的最少对换次数.
#### 题解
首先对原数组, 先把 $B$ 从小到大排一排, 根据 $B$ 的排法得到新的 $A$ 数组
那么这个问题就转变为了把新的 $A$ 在 $N-2$ 步里排序....

可以求排好的 $A$ 下标的置换, 数一数它的轮换个数, 个数大于 $2$ 就是 `Yes`

在轮换个数为 $1$ 的情况下, 如果在排好序的 $A$ 和 $B$ 中, 存在 $a_i \leq b_{i-1}$的情况, 说明原来的$1$个轮换可以被拆为$2$个, 于是也是`Yes`...
