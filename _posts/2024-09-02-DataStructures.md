---
layout: post
title: Data Structures
date: 2024-09-02 10:10 +0800
last_modified_at: 2024-12-25 12:00 +0800
tags: Computer
toc:  true
math: true
---
Welcome to the homepage of **Data Structures** !   
Tips:    
“Out of clutter, find simplicity. From discord, find harmony. In the middle of difficulty lies opportunity.”     
—— Einstein
{: .message }

# Course Introduction

<mark>Course number: 22010020 Credit: 4</mark>  

The teaching content of this course is as follows:   

<table border="1" width="100%">
  <tr>
    <th>Week</th>
    <th>Content</th>
  </tr>
  <tr>
    <td>1: AVL Trees</td>
    <td>
      <ul>
        <li>Operations on AVL Trees</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>2-4: Splay Trees</td>
    <td>
      <ul>
        <li>Basic operations of Splay Trees</li>
        <li>Amortized complexity analysis</li>
        <li>Amortized analysis of Splay Trees</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>5-7: B-Trees & Red-Black Trees</td>
    <td>
      <ul>
        <li>B-Trees</li>
        <li>Insertion and deletion in Red-Black Trees</li>
        <li>Logical relation and analysis between Red-Black Trees and B-Trees</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>8-9: Union-Find</td>
    <td>
      <ul>
        <li>Union-Find algorithms and implementation</li>
        <li>Complexity analysis of Union-Find</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>10-11: Heaps</td>
    <td>
      <ul>
        <li>Binary Heap</li>
        <li>Leftist Heap</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>12-16: Graph Algorithms</td>
    <td>
      <ul>
        <li>Graph representation and traversal</li>
        <li>Minimum Spanning Tree: Prim’s & Kruskal’s Algorithms</li>
        <li>Single-Source Shortest Path</li>
        <li>All-Pairs Shortest Path: Floyd’s Algorithm</li>
        <li>Maximum Matching Algorithm</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>17: Review & Assignment Guidance</td>
    <td>
      <ul>
        <li>Problem-solving discussion</li>
        <li>Final project guidance</li>
      </ul>
    </td>
  </tr>
</table>


-----

# Course Resourse

## Textbook of Data Structures

 [Textbook](https://book.douban.com/subject/26421141/).
 

All rights reserved by 机械工业出版社.

-----

## Courseware of Data Structures

 [Courseware(Part1)](https://xipingo.github.io/resource/DataStructures/Chapter1 搜索树.pdf).   
 [Courseware(Part2)](https://xipingo.github.io/resource/DataStructures/Chapter2 B-树 红黑树.pdf).   
 [Courseware(Part3)](https://xipingo.github.io/resource/DataStructures/Chapter3 渐近复杂性与摊销分析.pdf).   
 [Courseware(Part4)](https://xipingo.github.io/resource/DataStructures/Chapter4 伸展树.pdf).   
 [Courseware(Part5)](https://xipingo.github.io/resource/DataStructures/Chapter5 Scapegoat Trees.pdf).   
 [Courseware(Part6)](https://xipingo.github.io/resource/DataStructures/Chapter6 并查集.pdf).   
 [Courseware(Part7)](https://xipingo.github.io/resource/DataStructures/Chapter7 两个堆.pdf).   
 [Courseware(Part8)](https://xipingo.github.io/resource/DataStructures/Chapter8 图遍历.pdf).   


 All rights reserved by Professer [Zhao Jianhua](https://cs.nju.edu.cn/58/18/c2639a153624/page.htm).

-----

## Notes of Data Structures

 [Notes](https://xipingo.github.io/resource/DataStructures/Notes of Data Structures .pdf).

-----

## OJ of Data Structures

### OJ1  稀疏矩阵乘法

#### 任务描述

给定两个稀疏矩阵 $A$（规模 $p \times q$）与 $B$（规模 $q \times r$），请计算矩阵乘积 $C=A\times B$。输入仅给出两个矩阵的非零元素，请输出结果矩阵中所有非零元素（按行号—列号递增）。

> 注：本题旨在练习“按行/按列链表遍历与尾指针加速”等稀疏矩阵实现技巧，但评测仅依据输出结果对错，不限制具体实现方式。

#### 输入格式

* 第一行：三个正整数 `p q r`，表示矩阵规模（`A` 为 `p×q`，`B` 为 `q×r`）。
* 接着是矩阵 `A` 的输入：

  * 一行一个整数 `mA`，表示 `A` 的非零元素个数。
  * 接下来 `mA` 行，每行三个整数 `i j d`，表示 `A[i][j] = d`。
  * 这 `mA` 行按“行号递增；同一行内按列号递增”给出，且不存在重复位置。
* 接着是矩阵 `B` 的输入：

  * 一行一个整数 `mB`，表示 `B` 的非零元素个数。
  * 接下来 `mB` 行，每行三个整数 `i j d`，表示 `B[i][j] = d`。
  * 同样按“行号递增；同一行内按列号递增”给出，且不存在重复位置。

行号、列号均从 **1** 开始计数。

#### 约束条件

* `1 <= p, q, r <= 100`
* `0 <= mA, mB <= min(p*q, 10000)`
* 元素值 `d` 为 32 位有符号整数范围内数值
* 计算中产生的中间与结果数值也均在 64 位有符号整数范围内

#### 输出格式

* 第一行：一个整数 `cnt`，为结果矩阵 `C` 的非零元素个数。
* 接下来 `cnt` 行：每行三个整数 `i j d`，表示 `C[i][j] = d`，按“行号递增；同一行内按列号递增”输出。
* 若 `cnt = 0`，仅输出一行 `0`（不再输出后续行）。

#### 样例

##### 样例输入

```
2 3 2
3
1 1 1
1 3 2
2 2 3
3
1 2 4
2 1 5
3 2 6
```

##### 样例输出

```
2
1 2 16
2 1 15
```

#### 说明/提示

* 只输出乘积后非零的条目；若乘积为零矩阵，则输出 `0`。
* 可将 `A` 以“行链表”，`B` 以“列链表”存储，并在构建结果时为每一行/列维护尾指针以 $O(1)$ 追加新结点。
* 计算 `C[i][j]` 时，仅遍历 `A` 第 `i` 行的非零元素与 `B` 第 `j` 列的非零元素进行“同步归并”。

---

### OJ2  AVL 树的操作

#### 任务描述

从空 AVL 树开始，依次执行插入/删除操作。每次操作后按指定格式输出当前 AVL 树。

* 插入：`1 Data` —— 将 `Data` 插入到 AVL 树中。
* 删除：`2 Data` —— 将 `Data` 从 AVL 树中删除。若待删结点有两个子结点，则**在结构上删除左子树中的最大值**（即用前驱替换）。

平衡因子定义为：`balanceFactor = height(left) - height(right)`。

#### 输入格式

* 第一行：整数 `N`，表示操作次数。
* 接下来 `N` 行：每行一种操作，格式为：

  * `1 Data` 或
  * `2 Data`

#### 约束条件

* `1 <= N <= 10000`
* `-2^31 < Data < 2^31-1`（互不相同；若删除不存在的 `Data`，视为无变化但仍需按规则输出）

#### 输出格式

* 对于每次操作，**输出一行**当前 AVL 树的表示串：

  * 空树输出**空串**（即输出一个空行）。
  * 非空树按如下递归格式输出：
    `(` 左子树表示串 `root->data``,` `root->balanceFactor` 右子树表示串 `)`
    各部分**不含多余空格**。

#### 样例

##### 样例输入

```
6
1 30492
1 690
1 21634
1 5390
1 13923
2 30492
```

##### 样例输出

```
(30492,0)
((690,0)30492,-1)
((690,0)21634,0(30492,0))
((690,1(5390,0))21634,-1(30492,0))
(((690,0)5390,0(13923,0))21634,-1(30492,0))
((690,0)5390,1((13923,0)21634,-1))
```

#### 说明/提示

* 建议先实现用于自检的函数：树高、平衡因子校验、中序遍历、BST 有序性校验。
* 可先写递归版以验证旋转正确性，再实现**无栈**（迭代）插入与删除。
* 输出格式要求严格：不允许多余空格，逗号与括号位置需与定义一致；每次操作均需输出一行结果。

---

### OJ3  红黑树的操作

#### 任务描述

实现一个红黑树，支持 **插入** 与 **删除** 操作。
操作从空树开始。每次操作后，需要：

1. 按 **中序遍历** 从小到大输出树中所有结点的值；
2. 使用题目提供的检测函数检查是否满足红黑树的约束，并输出 `OK` 或 `ERROR`。

要求：

* 不允许使用 **递归** 或 **栈**；
* 不允许使用 **父指针**；
* 必须调用题目给出的 `checkRedBlackTree` 函数进行验证（字段名可适配，但逻辑不能改）。

#### 输入格式

* 第一行：一个整数 `N`，表示操作次数。
* 接下来的 `N` 行，每行表示一次操作：

  * `1 Data` —— 插入 `Data`；
  * `2 Data` —— 删除 `Data`。

#### 约束条件

* `1 <= N <= 10000`
* 数据范围：`-2^31 < Data < 2^31 - 1`
* 若删除不存在的元素，则树保持不变，但仍需输出检查结果。

#### 输出格式

* 每次操作后，先输出一行当前红黑树的中序遍历结果（结点之间以空格分隔，末尾带空格）。
* 下一行输出检测结果：`OK` 或 `ERROR`。

#### 样例

##### 输入

```
6
1 30492
1 690
1 21634
1 5390
1 13923
2 30492
```

##### 输出

```
30492 
OK
690 30492 
OK
690 21634 30492 
OK
690 5390 21634 30492 
OK
690 5390 13923 21634 30492 
OK
690 5390 13923 21634 
OK
```

#### 提示

* 可以在插入或删除操作的不同阶段调用 `checkRedBlackTree` 辅助定位错误。
* 正确实现的程序应当始终输出 `OK`。

---

### OJ4  左堆的实现

#### 任务描述

实现 **左堆（Leftist Heap）**，支持以下三种操作：

* `Insert`：向指定堆中插入一个整数；
* `RemoveMin`：删除并输出指定堆中的最小值；
* `Merge`：将两个堆合并，结果存放在第一个堆，第二个堆变为空堆。

初始时，给定 `N` 个空堆。

#### 输入格式

* 第一行：两个整数 `N M`，分别表示堆的数量与操作数。
* 接下来 `M` 行，每行表示一次操作：

  * `0 n` —— 从第 `n` 个堆中删除最小值并输出；
  * `1 n data` —— 在第 `n` 个堆中插入 `data`；
  * `2 n1 n2` —— 将第 `n2` 个堆合并到第 `n1` 个堆，第 `n2` 变为空堆。
* 约束：`0 <= n, n1, n2 < N`。

#### 输出格式

* 对于每个 `0 n` 操作，输出删除的最小值（以空格分隔）。

#### 样例

##### 输入

```
3 33
1 0 3
1 0 6
1 0 9
1 0 12
1 1 7
1 1 10
1 2 5
1 2 8
1 2 11
1 1 13
1 0 15
0 0
1 1 4
1 1 1
0 1
0 1
1 2 2
1 2 14
0 2
0 2
2 0 1
2 1 2
2 0 1
0 0
0 0
0 0
0 0
0 0
0 0
0 0
0 0
0 0
0 0
```

##### 输出

```
3 1 4 2 5 6 7 8 9 10 11 12 13 14 15
```

---

### OJ5.1  拓扑排序算法

#### 任务描述

给定一个使用 **出边邻接表** 表示的有向无环图（DAG），请使用 **入度统计法** 完成拓扑排序。
要求：

1. 在实现过程中，需将 **queue、topList、inDegrees** 三个数据结构合并到一个数组中完成；
2. 使用带尾指针的单链表来模拟队列操作，需练习头插、头删、尾插等特殊情况；
3. 为保证输出唯一性，算法限定如下：

   * 初始化时，所有入度为0的顶点按 **从小到大顺序** 插入到 queue 的**头部**；
   * 在处理顶点时，总是从 queue **头部**取出；
   * 当顶点 $v$ 的后继 $w$ 入度减为0时，将 $w$ 插入到 queue **头部**；
   * 遍历后继时，按输入邻接表中的顺序进行。

#### 输入格式

* 第一行：整数 `N`，表示图的顶点数（编号 `0 … N-1`）。
* 接下来的 `N` 行：每行描述一个顶点的出边：

  * 第一个整数 `c`，表示该顶点有 `c` 条出边；
  * 接着 `c` 个从小到大排列的不同整数，表示出边的目标顶点编号。

#### 输出格式

* 一行，`N` 个整数，表示一个合法的拓扑排序序列。

#### 约束条件

* `1 <= N <= 10000`
* 图保证是 DAG（无环）

#### 样例

##### 输入

```
3
1 2
2 0 2
0
```

##### 输出

```
1 0 2
```

##### 输入

```
9
1 1
1 3
1 3
0
1 2
1 2
1 2
1 1
5 0 4 5 6 7
```

##### 输出

```
8 7 6 5 4 2 0 1 3
```

---

### OJ5.2  使用 DFS 求强连通分量

#### 任务描述

给定一个有向图，使用 **DFS 框架 + Visitor 模式** 实现 **强连通分量（SCC）分解**。
每个顶点输出其所属强连通分量的编号。
规定：每个 SCC 的编号为 **该 SCC 中最小顶点编号**。
（因为 Tarjan/Kosaraju 算法输出时编号未必与最小顶点对齐，因此需要额外的转换数组来重新映射。）

要求：

1. 设计一个邻接表类；
2. DFS 框架接口：

   ```cpp
   void DFS(GRAPH ADJList, int color[], int vIdx, Visitor *v);
   ```
3. `Visitor` 为虚基类，接口如下：

   ```cpp
   class Visitor {
   public:
       virtual void pre_order_process(int vIdx) = 0;
       virtual void post_order_process(int vIdx) = 0;
   };
   ```

   可在其子类中添加成员变量与逻辑，以实现不同 DFS 应用（如 SCC）。

#### 输入格式

* 第一行：整数 `N`，表示顶点数（编号 `0 … N-1`）；
* 接下来 `N` 行：每行描述一个顶点的出边：

  * 第一个整数 `k`，表示该顶点有 `k` 条出边；
  * 接着 `k` 个整数，表示出边的目标顶点编号。

#### 输出格式

* 一行 `N` 个整数，第 `i` 个整数为顶点 `i` 所属的强连通分量编号（取该 SCC 中最小的顶点编号）。

#### 约束条件

* `1 <= N <= 10000`
* 图可能有多个强连通分量

#### 样例

##### 输入

```
7
3 1 2 5
2 2 3
0
2 0 2
1 6
2 0 2
1 4
```

##### 输出

```
0 0 2 0 4 0 4
```

#### 说明

* 示例与课件 PPT 一致：顶点命名 A-G 对应编号 0-6；
* 输出中，顶点与其 SCC 最小编号对应。

---

### OJ6  DAG 图中的递归与动态规划

#### 任务描述

给定一个满足下列性质的有向无环图（DAG）$G$（顶点编号为 $0,1,\dots,N-1$）：

1. 存在且唯一的源点 $S$：$S$ 无入边，且从 $S$ 能够到达图中所有顶点；
2. 存在且唯一的汇点 $T$：$T$ 无出边，且图中所有顶点都能到达 $T$。

每条有向边 $(u,v)$ 带有一个非负整数距离（权重） $d$（范围 0 到 99）。管理者希望对每条边收取非负整数通行费，使得任意一条从 $S$ 到 $T$ 的路径的“综合成本”（即每条边的距离加上该边的收费之和）都相等；在满足“所有路径综合成本相同”的前提下，总收费尽可能少。

令 $cost(v)$ 表示从顶点 $v$ 出发到达 $T$ 的综合成本（在收费完成后的统一成本）。由于图是 DAG，可建立递推：

$$
cost(u)=\max_{(u,v)\in E}\big\{\, distance(u,v) + cost(v)\,\big\}
$$

根据上式可以求出所有顶点的 $cost(\cdot)$，再由 $cost(u),cost(v),distance(u,v)$ 得到每条边的收费量（非负数）：

$$
toll(u,v)=cost(u) - (distance(u,v) + cost(v))
$$

（此式恒非负）

本题要求你：读入图，找出 $S$ 与 $T$ 的编号，计算并输出每个顶点的 $cost$ 值。

#### 输入格式

* 第一行：整数 `N`，表示顶点个数（顶点编号为 `0` 到 `N-1`）。
* 接下来的 `N` 行：第 `i` 行（从 `0` 开始）描述顶点 `i` 的出边：

  * 一个整数 `M`，表示出边数；随后有 `2*M` 个整数，按对出现：`tgt dist` 表示一条从 `i` 指向 `tgt`，权重为 `dist` 的边。
  * 每条边的 `dist` 为整数且满足 `0 <= dist <= 99`。

（输入保证图为 DAG，且满足题目中关于唯一 S 与唯一 T 的性质——即恰有一个入度为 0 的顶点和恰有一个出度为 0 的顶点，并且 S 能到达所有顶点、所有顶点能到达 T。）

#### 输出格式

* 第一行：两个整数 `S T`，分别为源点与汇点的编号。
* 第二行：`N` 个整数，用空格分隔，第 `i` 个数为 `cost(i)`，即顶点 `i` 到达 `T` 的综合成本（非负整数）。

#### 约束（建议）

* `1 <= N <= 100000`（或根据评测系统设定范围）；
* 边总数 `M_total` 满足 `0 <= M_total <= 200000`（仅为建议性上界，具体以评测为准）；
* 距离为非负整数且 `0 <= dist <= 99`；
* 中间与结果数值保证在 64 位有符号整数范围内（无需特别处理溢出）。

#### 算法提示

* 先读入图并统计每个顶点的入度与出度，找出 `S`（入度为0）与 `T`（出度为0）；
* 因为图为 DAG，可用 **拓扑排序**（或递归 + 记忆化）从 `T` 反向或从 `S` 正向计算 `cost`：

  * 递推形式为 `cost(T) = 0`；对其它顶点 `u`，`cost(u) = max_{(u,v)} (dist(u,v) + cost(v))`；
  * 若使用拓扑序，从后向拓扑序（使得所有后继的 `cost` 已计算）逐点计算；或用 DFS + 记忆化自顶向下计算；
* 计算完成后，若需要收费数 `toll(u,v)`，可按式 `cost(u) - (dist(u,v) + cost(v))` 计算（题目输出只要求 `cost`，不强制要求输出 toll）。

#### 样例

##### 输入

```
4
2 2 1 3 2
2 2 5 0 8
1 3 3
0
```

##### 输出

```
1 3
4 12 3 0
```

##### 说明（对应样例）

* 顶点 3 无出边，因此 `T = 3`，`cost(3) = 0`。
* 顶点 2 只有一条去 3 的边，长度 3，故 `cost(2)=3`。
* 顶点 0 有两条出边：`0->2 (1)` 与 `0->3 (2)`，对应综合代价分别为 `1 + cost(2) = 4` 与 `2 + cost(3) = 2`，取最大得 `cost(0)=4`（然后可对边 `0->3` 收费 `4-(2+0)=2`）。
* 顶点 1 的两条路径 `1->2` 与 `1->0` 分别总代价为 `5 + cost(2) = 8` 与 `8 + cost(0) = 12`，取最大得 `cost(1)=12`（可对边 `1->2` 收费 `12-(5+3)=4`）。
* 因此输出 `S=1`（入度为 0 的顶点），`T=3`，以及 `cost` 数组 `4 12 3 0`。

---

## Tips of Data Structures

 Not easy(especially OJs), good grades.

-----