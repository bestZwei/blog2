---
title: Markdown 数学公式格式
published: 2024-09-20
description: 想让 Markdown 更整洁美观码？
tags: [技术, markdown]
image: "https://testingcf.jsdelivr.net/gh/bestZwei/imgs@master/picgo/%7B97532124-11C7-40D0-869E-3A85E090F4FC%7D.png"
category: Study
draft: false
lang: zh_CN
---
# Markdown 数学公式格式

## 一、常用符号

### 内联公式

在 Markdown 语法中可以书写数学公式，书写数学公式必须要有一个入口——内联公式。

```
$ 数学公式 $
```

即一对美元符号将所要书写的数学公式括起来就可以让编辑器识别并预览。一对美元符号对应一行数学公式，多行数学公式就需要两对美元符号。

```
$$
数学公式\ =\  
\begin{cases}
数学公式\\
数学公式\\
数学公式\\
\end{cases}
$$
```

$$
数学公式\ =\  
\begin{cases}
数学公式\\
数学公式\\
数学公式\\
\end{cases}
$$

其中，编辑器默认一对 `{}` 符号内的内容为一个整体，以斜线 `\` 加空格表示空格，双斜线 `\\` 表示换行。

## 常用符号

|    名称     |   实例    | 预览 |            注释             |
| :---------: | :-------: | :--: | :-------------------------: |
|   上下标    |   a^n_m   |      | 上标^用于指数，下标用于角标 |
| 正负号（±） |  a \pm b  | a±b  |                             |
|     乘      |  \times   |  ×   |                             |
|     除      |   \div    |  ÷   |                             |
|    根号     |   \sqrt   |      |         根号下(a-b)         |
|    大于     |    \gt    |  ＞  |                             |
|    小于     |    \lt    |  ＜  |                             |
|  大于等于   |    \ge    |  ≥   |                             |
|  小于等于   |    \le    |  ≤   |                             |
|   正无穷    |  \infty   |  ∞   |                             |
|   负无穷    |  -\infty  |  -∞  |                             |
|    分数     | \dfrac{a} |      |           a分之b            |
|   省略号    |  \cdots   | ...  |                             |

## 三角函数

| 数学表达式 | 代码 |
| :--------: | :--: |
|    sinθ    | \sin |
|    cosθ    | \cos |
|    tanθ    | \tan |
|    cotθ    | \cot |

## 矢量、累加累乘、极限

|  数学表达式   |    代码     |
| :-----------: | :---------: |
|     矢量      |   \vec{}    |
| 累加（求和∑） | \sum_{}^{}  |
| 累乘（求积∏） | \prod_{}^{} |
|     极限      |   \lim_{}   |

## 希腊字母表

|    代码     | 预览 |   代码   | 预览 |
| :---------: | :--: | :------: | :--: |
|   \alpha    |  α   |   \pi    |  π   |
|    \beta    |  β   |   \rho   |  ρ   |
|   \gamma    |  γ   |   \xi    |  ξ   |
|   \delta    |  δ   |   \nu    |  ν   |
|  \epsilon   |      | \upsilon |  υ   |
| \varepsilon |  ε   | \varphi  |  φ   |
|    \eta     |  η   |   \chi   |  χ   |
|   \theta    |  θ   |   \psi   |  ψ   |
|   \kappa    |  κ   |  \omega  |  ω   |
|    \iota    |  ι   |  \Omega  |  Ω   |
|    \zeta    |      |  \Gamma  |  Γ   |
|   \lambda   |  λ   |  \Delta  |  Δ   |
|     \mu     |  μ   |          |      |
|    \phi     |  φ   |   \Phi   |  Φ   |

## 矩阵

### 简单矩阵

#### 简单矩阵示例1

使用 `\begin{matrix} ... \end{matrix}` 生成，每一行以 `\\` 结尾表示换行，各元素间以 `&` 隔开，右边的数学公式代码块序号用 `\tag{n}` 表示。

$$
\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6\\
7 & 8 & 9\\
\end{matrix}
\tag{简单矩阵 - 示例1}
$$

```
$$
\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6\\
7 & 8 & 9\\
\end{matrix}
\tag{简单矩阵 - 示例1}
$$
```

#### 简单矩阵示例二（带括号）

##### 大括号

$$
\left\{
\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6\\
7 & 8 & 9\\
\end{matrix}
\right\}
\tag{带有大括号的矩阵}
$$

```
$$
\left\{
\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6\\
7 & 8 & 9\\
\end{matrix}
\right\}
\tag{带有大括号的矩阵}
$$
```

或

$$
\begin{Bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{Bmatrix}
\tag{6}
$$

```
$$
\begin{Bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{Bmatrix}
\tag{6}
$$
```

##### 中括号

$$
\left[
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right]
\tag{中括号}
$$

```
$$
\left[
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right]
\tag{中括号}
$$
```

或

$$
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix}
\tag{6}
$$

```
$$
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix}
\tag{6}
$$
```

##### 小括号

$$
\left(
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right)
\tag{小括号}
$$

```
$$
\left(
\begin{matrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{matrix}
\right)
\tag{小括号}
$$
```

##### 包含省略号和希腊字母

行省略号 `\cdots`，列省略号 `\vdots`，斜向省略号（左上至右下） `\ddots`。

$$
\left\{
\begin{matrix}
1      & 2        & \cdots & 5        \\
6      & 7        & \cdots & 10       \\
\vdots & \vdots   & \ddots & \vdots   \\
\alpha & \alpha+1 & \cdots & \alpha+4 
\end{matrix}
\right\}
$$

```
$$
\left\{
\begin{matrix}
1      & 2        & \cdots & 5        \\
6      & 7        & \cdots & 10       \\
\vdots & \vdots   & \ddots & \vdots   \\
\alpha & \alpha+1 & \cdots & \alpha+4 
\end{matrix}
\right\}
$$
```

## 表格

### 简单表格

**开头结尾**：

```
\begin{array} ... \end{array}
```

**定义式**：

例：`{|c|c|c|}`，其中 `c` `l` `r` 分别代表居中、左对齐及右对齐。

**分割线**：

1. **竖直分割线**：在定义式中插入 `|`， （`||` 表示两条竖直分割线）。
2. **水平分割线**：在下一行输入前插入 `\hline`，以下图真值表为例。

其他：每行元素间均须要插入 `&` ，每行元素以 `\\` 结尾。

$$
\begin{array}{|c|c|c|}
\hline 2&9&4\\
\hline 7&5&3\\
\hline 6&1&8\\
\hline
\end{array}
$$

```
$$
\begin{array}{|c|c|c|}
\hline 2&9&4\\
\hline 7&5&3\\
\hline 6&1&8\\
\hline
\end{array}
$$
```

### 真值表

$$
\begin{array}{cc|c}
A & B & F \\
\hline 0 & 0 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 1 \\
\end{array}
$$

```
$$
\begin{array}{cc|c}
A & B & F \\
\hline 0 & 0 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
1 & 1 & 1 \\
\end{array}
$$
```

## 方程组、表达条件式

### 方程组

$$
\begin{cases}
3x + 5y + z \\
7x - 2y + 4z \\
-6x + 3y + 2z
\end{cases}
$$

```
$$
\begin{cases}
3x + 5y + z \\
7x - 2y + 4z \\
-6x + 3y + 2z
\end{cases}
$$
```

### 表达条件式

$$
f(n) =
\begin{cases} 
n/2, & \text{if } n \text{ is even} \\
3n+1, & \text{if } n \text{ is odd}
\end{cases}
$$

```
$$
f(n) =
\begin{cases} 
n/2, & \text{if } n \text{ is even} \\
3n+1, & \text{if } n \text{ is odd}
\end{cases}
$$
```

## 格式

### 代码块内多行代码对齐

$$
\begin{aligned}
a &= b + c \\
  &= d + e + f
\end{aligned}
$$

```
$$
\begin{aligned}
a &= b + c \\
  &= d + e + f
\end{aligned}
$$
```

### 间隔（空格、跟随）

跟随 `\!`

无空格 小空格 `\,` 中空格 `\;` 大空格 `\`

真空格 `\quad` 双真空格 `\qquad`

$$
a\!b + ab + a\,b + a\;b + a\ b + a\quad b + a\qquad b
$$

```
$$
a\!b + ab + a\,b + a\;b + a\ b + a\quad b + a\qquad b
$$
```