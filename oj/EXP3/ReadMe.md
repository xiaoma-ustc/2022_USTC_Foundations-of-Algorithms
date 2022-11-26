# 算法基础-EXP3
# 2022-E3-1 最大和
## Description

对于一个长度为n的整数数组，请你找出一个具有最大和的连续子数组，输出其最大和。

## Input
第一行一个整数n

接下来一行n个整数表示整数数组

对于30%的数据，
$n \leq 15$
，数组内元素绝对值不超过15

对于100%的数据，
$n \leq 10^5$
，数组内元素绝对值不超过
$10^8$

## Output

拥有最大和的连续子数组的最大和

## Sample Input
```C++
11
-3 15 9 -3 9 6 3 9 7 -4 -14
```

## Sample Output
```C++
55
```

# 2022-E3-2 最小路径
## Description

对于一个元素均为正整数，大小为n*m的网格，Alice从左上角(1,1)出发，每次只能选择向右或向下走一格，最终到达网格右下角停止。

到达网格右下角存在若干路径，请你找出路径上各点的数字总和最小的路径，输出其数字总和。

## Input
第一行输入两个数字n m

接下来n行代表网格

对于30%的数据，
$n,m \leq 10$
，网格内元素
$\leq 10$

对于100%的数据，
$n,m \leq 200$
，网格内元素
$\leq 1000$

## Output

最小路径的数字总和

## Sample Input
```C++
6 5
4 1 1 5 2
4 3 2 5 2
2 4 1 4 2
1 5 3 4 3
3 2 1 2 2
2 3 3 1 3
```

## Sample Output
```C++
19
// 最小路径为4-1-1-2-1-3-1-2-1-3，总和为19
```
# 2022-E3-3 多重背包
## Description

现有一个背包可以容纳总重量为WW的物品，有nn种物品可以放入背包，其中每种物品单个重量为
$w_i$
​，价值为
$v_i$
，可选数量为
$num_i$
。

输出可以放入背包的物品的最大总价值。

## Input
第一行两个整数n,Wn,W，分别表示物品件数和背包容量。

然后nn行数据描述每种物品的重量、价值和可选数量。

每行的格式为 
$w_i\quad  v_i\quad  num_i$
。

数据规模：

$1\leq n\leq 200$

$1\leq W\leq 10000$

$1\leq w_i\leq 1000$ 

$1≤num_i≤10000$

所有输入数据均为整数。

## Output

输出一个整数表示可以装入背包的最大价值。

## Sample Input
```C++
5 100
7 3 68
10 3 161
10 6 55
5 2 14
3 10 165
```

## Sample Output
```C++
330
```

# 2022-E3-3 正方形计数
## Description

现有一个
$n\times m$
的矩形区域，其中每个单位区域可能有损坏。

要求找到地面上所有不包含损坏区域的正方形的个数。

## Input
第一行两个整数n,m表示矩形区域的大小。

接下来共有n行输入数据，每行包含m个0或1的整数，其中0表示该地面完好，1表示该地面已损坏。

数据规模：

$20000<n \quad m≤2000$

## Output

输出一个整数表示区域内的正方形个数。

输入数据保证结果不会超出int32的范围。

## Sample Input
```C++
5 5
1 0 0 0 0 
1 0 0 1 1 
0 1 0 0 0 
0 1 0 1 0 
1 0 0 0 0
```

## Sample Output
```C++
18
```