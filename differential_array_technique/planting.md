# [CSP-J2022 山东] 植树节

## 题目描述

植树节快要到了，学校要组织志愿者去给树苗浇水。

有一排树苗，编号依次是 $0,1,2,\dots$。

现有 $n$ 个志愿者去给树苗浇水，第 $i$ 个志愿者选定了一个区间 $\left[a_{i},b_{i}\right]$ ，表示第 $i$ 个志愿者将 $\left[a_{i},b_{i}\right]$ 这一区间内的每一棵树都浇一次水。

如某个志愿者选择的浇水区间为 $\left[4,9\right]$ ，表示他将给编号为 $4,5,6,7,8,9$ 的树各浇水一次。

当所有的志愿者完成各自所选区间的浇水后，可能有些树苗被不同的志愿者浇水多次，也可能有的树苗一次也没被浇过水。

请你求出浇水最多的树苗被浇了多少次。

## 输入格式

第 $1$ 行，一个整数 $n$ ，表示志愿者的人数。

第 $2$ 行到第 $n+1$ 行，每行两个整数 $a_{i},b_{i} $（$i=0,1,2,\dots n-1$），表示志愿者 $i$ 选择的浇水区间。

## 输出格式

输出 $1$ 行， $1$ 个整数，表示浇水最多的树苗被浇水的次数。

## 样例 #1

### 样例输入 #1

```
4
0 2
2 4
1 4
6 7
```

### 样例输出 #1

```
3
```

## 样例 #2

### 样例输入 #2

```
4
1000000 1000000
1000000 1000000
0 1000000
1 1000000
```

### 样例输出 #2

```
4
```

## 提示

样例三见下发数据目录下的 planting/planting3.in 与 planting/planting3.ans。  
### 数据范围
* 对于所有的数据： $n<10^{5}$；$0\le a_{i}\le b_{i}\le 10^{6}$。  

|测试点编号|$a_{i}\le$|$b_{i}\le$|$n_{i}\le$|特殊性质|
|:-:|:-:|:-:|:-:|:-:|
|$1,2,3$|$10^{3}$|$10^{3}$|$10^{3}$|无|
|$4,5,6,7$|$10^{6}$|$10^{6}$|$10^{5}$|无|
|$8$|$10^{6}$|$10^{6}$|$10^{5}$|$a_{i}=b_{i}$|
|$9$|$10^{6}$|$10^{6}$|$10^{5}$|$a_{i}=1,b_{i}=10^{3}$|
|$10$|$10^{6}$|$10^{6}$|$10^{5}$|无|