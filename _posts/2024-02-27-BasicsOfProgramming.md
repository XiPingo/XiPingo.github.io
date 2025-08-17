---
layout: post
title: Basics of Programming
date: 2024-02-27 18:30 +0800
last_modified_at: 2024-06-14 18:00 +0800
tags: Computer
toc:  true
math: true
---
Welcome to the homepage of **Basics of Programming** !   
Tips:    
“C 很容易使你搬起石头砸自己的脚，而 C++ 把这事变得更难，但是如果一定要这么做，那么你的整条腿都会被炸飞。”   
——— Bjarne Stroustrup
{: .message }

# Course Introduction

<mark>Course Number: 22000010 Credit: 3</mark>

The teaching content of this course is as follows:   

<table border="1" width="100%">
  <tr>
    <th>Section</th>
    <th>Content</th>
  </tr>
  <tr>
    <td>1. Introduction to C Programs (4 lecture hours, Cognition and Experience)</td>
    <td>
      <ul>
        <li>Computer hardware, software and languages</li>
        <li>Basic structure of C programs</li>
        <li>Basic elements of C language</li>
        <li>Simple input/output programs</li>
        <li>Variables: definition, assignment and initialization</li>
        <li>Programming style</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>2. Program Flow Control (6 lecture hours, Judgment and Reasoning)</td>
    <td>
      <ul>
        <li>Basic and nested forms of sequential, branch and loop flows and their control methods</li>
        <li>Applications in problem-solving such as classification, enumeration and iteration</li>
        <li>Structured programming methods</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>3. Program Module Design (10 lecture hours, Abstraction and Encapsulation)</td>
    <td>
      <ul>
        <li>Subprograms and process abstraction</li>
        <li>Definition and call of functions</li>
        <li>Function parameters and return values</li>
        <li>Communication between functions (Method 1, global variables and Method 2)</li>
        <li>Nested and recursive calls of functions</li>
        <li>Multi-module programs and header files</li>
        <li>Scope of identifiers</li>
        <li>Storage duration of variables</li>
        <li>Module optimization</li>
        <li>Modular programming methods</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>4. Operation Description in Programs (4 lecture hours, Analysis and Expression)</td>
    <td>
      <ul>
        <li>Basic operators</li>
        <li>Issues related to expressions</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>5. Data Description in Programs (4 lecture hours, Definition and Conversion) and Applications</td>
    <td>
      <ul>
        <li>Information representation in computers</li>
        <li>Basic data types and their selection</li>
        <li>Type conversion and construction</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>6. Derived Data Types and Their Applications (24 lecture hours, Construction and Access)</td>
    <td>
      <ul>
        <li>Arrays and their applications</li>
        <li>Pointers</li>
        <li>Communication between functions (Method 3)</li>
        <li>Dynamic variables</li>
        <li>Supplementary C++ references, communication between functions (Method 4)</li>
        <li>Strings</li>
        <li>Structures, stacks, linked lists and their applications</li>
        <li>Unions and enumerations</li>
        <li>Files</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>7. Nature of Programs and Programming (4 lecture hours, Induction and Promotion)</td>
    <td>
      <ul>
        <li>Introduction to algorithms and data structures and their implementation</li>
        <li>Computer working model</li>
        <li>Programming paradigms</li>
        <li>Programming languages</li>
        <li>Software development process</li>
        <li>Standardized programming methods</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>8. C/C++ Language Program Development Environment (2 practice hours)</td>
    <td>
      <ul>
        <li>Steps for computer practice and use of program development environment</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>9. Statements (4 practice hours, Lab test content: Write C programs with basic processes to solve simple practical problems)</td>
    <td>
      <ul>
        <li>One of the program debugging methods: Location and elimination of syntax errors in programs</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>10. Functions (4 practice hours, Lab test content: Write C programs with 2-3 functions to solve simple practical problems)</td>
    <td>
      <ul>
        <li>Second program debugging method: Location and elimination of logical errors in programs</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>11. Operation and Data Description (4 practice hours, Lab test content: Write C programs, comprehensively use basic operations and flow control methods, and select appropriate basic data types to solve typical simple practical calculation problems)</td>
    <td>
      <ul>
        <li>Comprehensive application of basic operations, flow control and basic data types</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>12. Derived Data Types and Implementation of Common Simple Calculation Methods (14 practice hours, Lab test content: Write C programs for various types of data processing)</td>
    <td>
      <ul>
        <li>Third program debugging method: Identification and elimination of "persistent ailments" in programs</li>
      </ul>
    </td>
  </tr>
</table>

-----

# Course Resourse

## Textbook of Basics of Programming

 [Textbook](https://weread.qq.com/web/bookDetail/c8532fd0813ab802bg01488d).
 

All rights reserved by 机械工业出版社.

-----

## Courseware of Basics of Programming

<mark> You can ask me for the courseware via email. </mark>

 All rights reserved by Professer [Guo Jie](https://cs.nju.edu.cn/51/c2/c56396a86466/page.htm).

-----

## OJ of Basics of Programming

### OJ1.1

#### 任务描述

假设有一张面值为 `n (1 <= n <= 10000)` 的纸币，给定三种不同面额的零钱以及它们的数量：`a` 元、`b` 元和 `c` 元，数量分别为 `x` 张、`y` 张和 `z` 张。  

请问，如果把这张 `n` 元的纸币换成零钱，一共有多少种不同的换法？

#### 输入格式

7 个正整数，以空格分隔，依次表示：

```
n a b c x y z
```

其中约束条件为：

- `1 <= n <= 10000`  
- `1 <= a, b, c <= 100`  
- `0 <= x, y, z <= 100`  

#### 输出格式

一个整数，表示不同的换法的种数。

#### 样例

##### 样例输入

```
5 1 2 3 2 1 1
```

##### 样例输出

```
2
```

---

### OJ1.2

#### 任务描述

在一个遥远的海洋星球上，住着一只聪明而又好奇的小蓝鲸。有一天，小蓝鲸在海底发现了一些神秘的数字石碑。它注意到这些石碑上的数字在海浪的翻滚下有时会倒过来，但奇怪的是，某些数字石碑无论怎样翻转，显示的数字都是一样的。这让小蓝鲸非常好奇。

小蓝鲸决定命名这种特殊的数字为“海洋回文数”。为了验证一块石碑上的数字是否为海洋回文数，小蓝鲸想请你帮忙编写一个程序。程序需要判断给定的整数 `x` 是否是一个海洋回文数。如果是，返回 `true`；否则，返回 `false`。

**“海洋回文数”**是指一个整数，在正序（从左向右）和倒序（从右向左）读都是一样的，就像海底的倒影一样不变。

注意：在海洋星球上，负数由于无法在海浪中完美翻转，因此不被认为是海洋回文数。

#### 输入格式

一个整数 `x`。

#### 输出格式

布尔值 `true` 或 `false`，表示该整数是否为海洋回文数。

#### 样例

##### 样例1

**输入**

```
121
```

**输出**

```
true
```

##### 样例2

**输入**

```
-121
```

**输出**

```
false
```

---

### OJ2.1

#### 任务描述

给定两个非递减顺序排列的整数数组 `nums1`, `nums2`。

请按非递减顺序排列输出合并后的数组。

注意：

- 本题原则上不允许使用 `sort` 函数等排序库函数解答。  
- 非递减顺序数组指的是数组中没有逆序对，即数字按照从小到大的顺序排列，但可以有重复数字的出现。  
- 每个数组的长度 `<= 100`  
- 数组中的元素在整型范围内  

#### 输入格式

共 3 行：

1. 第一行是两个整数 `m, n`，用空格隔开，表示两个数组的长度。  
2. 第二行是 `nums1`，包含 `m` 个整数，用空格隔开。  
3. 第三行是 `nums2`，包含 `n` 个整数，用空格隔开。  

#### 输出格式

共一行，包含 `m+n` 个数字，为合并后非递减的数组，数字间用空格隔开。  

#### 样例

**输入**

```
5 3
1 2 3 4 5
1 2 3
```

**输出**

```
1 1 2 2 3 3 4 5
```

---

### OJ2.2

#### 任务描述

给定一个有重复、非递减的整数数组 `candidates` 和一个目标整数 `target`，找出 `candidates` 中可以使数字和为目标数 `target` 的所有不同组合。你需要以字典序输出结果组合。

注意：

- `candidates` 中出现一次的数字只能至多选取一次，同理，出现 n 次的数字至多只能选取 n 次。  
- 如果至少一个数字的被选数量不同，则两种组合是不同的。  
- 输出的组合需按字典序排列，序列内部数字升序，序列间也按字典序。  
- 若不存在和为 `target` 的组合，则输出空字符串。  

约束条件：

- `1 <= candidates.length <= 50`  
- `1 <= candidates[i] <= 100`  
- `1 <= target <= 100`  
- 保证和为 `target` 的不同组合数少于 150 个  

#### 输入格式

共两行：

1. 第一行是两个整数 `n` 和 `target`，分别表示 `candidates` 的长度和目标值。  
2. 第二行是 `candidates` 的 n 个整数，用空格隔开。  

#### 输出格式

若干行，每行是和为 `target` 的数字序列。  
- 序列内部数字用空格隔开  
- 序列间换行  
- 序列内部、序列间均按字典序排列  
- 每行结尾不要有多余空格  

#### 样例

**样例1**

输入：

```
5 7
2 2 2 3 7
```

输出：

```
2 2 3
7
```

解读：和为 7 有两种组合方式，即 2+2+3 和 7。需要注意的是，`candidates` 中的三个 2 是相同的，因此 2+2+3 的组合只有一种。  

**样例2**

输入：

```
3 8
2 3 5
```

输出：

```
3 5
```

#### 提示

在数字被选数量不同才视为不同的情况下，可以通过**回溯/递归时按索引顺序选择并跳过重复数字**来避免重复加入相同序列。例如：

- 先对 `candidates` 排序  
- 在递归中，对于相同的数字，如果在同一层递归已使用过，则跳过  
- 每次递归传递当前索引，保证组合数字不倒序  

这样可以保证输出的组合唯一且按字典序排列。

---

### OJ2.3

#### 任务描述

最近，两个助教决定进行一场比拼！比拼的内容是统计学。  
助教查阅到一个人类称之为“逆序对”的概念：对于给定的一段正整数序列，逆序对是指序列中存在的有序对 `(a_i, b_j)`，满足 `a_i > b_j` 且 `i < j`。  

比赛的目标是计算给定序列中的逆序对数量。注意序列中可能有重复数字。

#### 输入格式

两行：

1. 第一行包含整数 `n`，表示序列中数字的个数 `(n < 2×10^4)`  
2. 第二行包含 `n` 个正整数，表示序列元素，数字大小不超过 `10^9`  

#### 输出格式

输出一个整数，表示序列中逆序对的数量。

#### 样例

**输入**

```
6
5 4 2 6 3 1
```

**输出**

```
11
```

#### 相关知识

归并排序是一种非常有效的排序方法，不仅能实现 `O(n log n)` 的排序复杂度，还能在归并过程中顺便统计逆序对数量。

---

### OJ2.4

#### 任务描述

编写程序实现对一个 n 位数 `x`，交换其第 `k` 位和第 `n+1-k` 位（从左到右计数，第 1 位为最高位），返回交换后的数值。

例如：

- `12345`，交换第 1 位和第 5 位 → `52341`  
- `2468`，交换第 2 位和第 3 位 → `2648`  

**保证输入的 n 位数 x 不含 0。**

#### 输入格式

一行三个整数：

```
n x k
```

约束条件：

- `1 <= n, k <= 9`  
- `1 <= x <= 999999999 ` 

#### 输出格式

返回交换后的数值。

#### 样例

**样例1**

输入：

```
5 12345 1
```

输出：

```
52341
```

**样例2**

输入：

```
7 1367789 6
```

输出：

```
1867739
```

---

### OJ3.1

#### 任务描述

输入一串数字，表示一个不含前导零的非负整数。请你构造一个链表存储它，并将这个数字链表表示的数翻倍。

> 注意：本题必须使用链表的数据结构完成，否则不得分。

#### 输入格式

一串整数，从左到右表示链表各个节点的值。

#### 输出格式

一串整数，从左到右表示链表翻倍后各个节点的值。

#### 示例

**示例1**

输入：

```
1 8 9
```

输出：

```
3 7 8
```

解释：给出的链表表示数字 189，返回的链表表示数字 189 * 2 = 378。

**示例2**

输入：

```
9 9 9
```

输出：

```
1 9 9 8
````

解释：给出的链表表示数字 999，返回的链表表示数字 999 * 2 = 1998。

#### 提示

1. 链表中节点的数目在范围 `[1, 10^4]` 内  
2. `0 <= ListNode.val <= 9`  
3. 生成的输入保证链表表示一个不含前导零的数字（除了数字 0 本身）  
4. 如何输入一串事先不知道长度的数字？可以使用如下方法读取到 `EOF`：

```cpp
while(std::cin.peek()!= EOF){
    int x; 
    std::cin >> x;
}
````

---

### OJ3.2

#### 任务描述

本题要求将一个以字符串二维数组形式输入的三通道 RGB 图像转换为单通道的灰度图像。

在计算机中，图片通常以像素矩阵（matrix）的形式存在。矩阵的行列数称为该图片的**分辨率**（resolution），矩阵的每个元素称为一个**像素**（pixel）。

每个像素存储一个颜色值，使用 RGB 表示：

```
Color := (R, G, B), 0 ≤ R, G, B ≤ 255, R, G, B ∈ ℤ⁺
```

* 例如白色 RGB 值为 (255, 255, 255)，十六进制表示为 `FFFFFF`
* 红色为 (255, 0, 0)，十六进制表示 `FF0000`
* 黑色为 (0, 0, 0)，十六进制表示 `000000`

当我们将 RGB 图像转换为灰度图像时，需要将 RGB 三通道按以下规则合并为单通道：

```
Gray = R * 0.299 + G * 0.587 + B * 0.114
```

在本题中，结果向下取整，得到一个 0\~255 的整数值，用两位十六进制表示。

#### 输入格式

* 第一行：两个整数 `m, n`，分别表示图像矩阵的行数和列数，`1 ≤ m, n ≤ 2048`
* 接下来的 m 行，每行 n 个颜色字符串，格式为 `#XXXXXX`

  * 井号 `#` 后的前两位表示十六进制 R 值
  * 中间两位表示十六进制 G 值
  * 最后两位表示十六进制 B 值

#### 输出格式

* m 行，每行 n 个灰度值字符串，格式为 `#XX`

#### 样例

**样例输入1**

```
1 1
#98F5FF
```

**样例输出1**

```
#DA
```

解释：`#98F5FF` = (152, 245, 255)，Gray = 152*0.299 + 245*0.587 + 255\*0.114 = 218.333 → 向下取整为 218 → `#DA`

**样例输入2**

```
3 5
#000000 #00003F #00007F #0000BF #0000FF
#000000 #003F00 #007F00 #00BF00 #00FF00
#000000 #3F0000 #7F0000 #BF0000 #FF0000
```

**样例输出2**

```
#00 #07 #0E #15 #1D
#00 #24 #4A #70 #95
#00 #12 #25 #39 #4C
```

**样例输入3**

```
1 1
#CACACA
```

**样例输出3**

```
#CA
```

解释：202 \* 0.299 + 202 \* 0.587 + 202 \* 0.114 = 202 → `#CA`

---

## Tips of Basics of Programming

The difficulty of the midterm and final exams is not particularly large, the key is to grasp the three oj tests.
 
-----