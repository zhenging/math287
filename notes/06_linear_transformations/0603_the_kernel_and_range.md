### 6.3 The kernel and range of a linear transformation

**Kernel**
Let $T:V \to W$ be a linear transformation. The set of all vectors $v$ in $V$ such that $T(v) = 0$ is called the kernel of the $T$ and is denoted by $\text{Ker}(T)$.

**Range**
The **range** of $T:V \to W$ is the subset of $W$ consisting of all transformed vectors from $V$. The range of T is denoted by $\text{Rng}(T)$.

If $T:V \to W$ is a linear transformation, then
+ $\text{Ker}(T)$ is a subspace of $V$.
+ $\text{Rng}(T)$ is a subspace of $W$.

If $T:\R^n \to \R^m$ is a linear transformation, then
+ $\text{Ker}(T) = \text{nullspace}(A)$, which is a subspace of $\R^n$
+ $\text{Rng}(T) = \text{colspace}(A)$, which is a subspace of $\R^m$

**General Rank-Nullity Theorem**
If $T:V \to W$ is a linear transformation and $V$ is finite-dimensional, then
$$
\begin{aligned}
\text{dim}[\text{Ker}(T)] + \text{dim}[\text{Rng}(T)] = \text{dim}(V)
\end{aligned}
$$

**One-To-One / Onto**
If $T:V \to W$ is a linear transformation.
+ $T$ is _one-to-one_ **iff** the preimage of every $w$ in the range consists of a single vector. That is whenever $v_1 \ne v_2, T(v_1) \ne T(v_2)$.
+ $T$ is _onto_ **iff** every element of $W$ has a preimage in $V$.
+ $T$ is one-to-one **iff** $\text{Ker}(T) = {0}$.
+ $T$ is onto **iff** $\text{Rng}(T) = W$. (This is one is immediate from the definition.)

If $T:V \to W$ is a linear transformation, and let $V$ and $W$ be finite-dimensional.
+ (1) $T$ is one-to-one, then $\text{dim}[V] \le \text{dim}[W]$.
+ (2) If $T$ is onto, then $\text{dim}[V] \ge \text{dim}[W]$.
+ (3) If $T$ is both one-to-one and onto, then $\text{dim}[V] = \text{dim}[W]$.
+ (4) If $\text{dim}[V] = \text{dim}[W]$, then $T$ is one-to-one **iff** $T$ is onto.

#### Homework
p.405 1-7 all, 13b, 14-20 all (see my answers)

1\. Consider $T:\R^2 \to \R^4$ defined by $T(x) = Ax$, where $A = \begin{bmatrix}
1 & 2\\
2 & 4\\
4 & 8\\
8 & 16
\end{bmatrix}$. For each $x$ below, find $T(x)$ and thereby determine whether $x$ is in $\text{Ker}(T)$.
>Solution
$$
\begin{aligned}
\begin{bmatrix}
1 & 2\\
2 & 4\\
4 & 8\\
8 & 16
\end{bmatrix}
\begin{bmatrix}
-10\\
5
\end{bmatrix} =
\begin{bmatrix}
0\\
0\\
0\\
0
\end{bmatrix}
\end{aligned}
$$
a. $x(-10, 5)$, $T(x) = (0, 0, 0, 0)$. Yes.
b. $x(-1, -1)$, $T(x) = (-1, -2, -4, -8)$. No.
c. $x(2, -1)$, $T(x) = (0, 0, 0, 0)$. Yes.

5\. Find $\text{Ker}(T)$ and $\text{Rng}(T)$, and give a geomatrical description of each. Also find $\text{dim}[\text{Ker}(T)]$ and $\text{dim}[\text{Rng}(T)]$, and verify Theorem 6.3.8.
$T:\R^3 \to \R^3$ defined by $T(x) = Ax$, where $A = \begin{bmatrix}
1 & -2 & 1\\
2 & -3 & -1\\
5 & -8 & -1
\end{bmatrix}$.
>Solution
$$
\begin{aligned}
&\begin{bmatrix}
1 & -2 & 1\\
2 & -3 & -1\\
5 & -8 & -1
\end{bmatrix}
\sim
\begin{bmatrix}
1 & -2 & 1\\
0 & 1 & -3\\
0 & 0 & 0
\end{bmatrix}\\
&\To x = t(5, 3, 1), t\ne 0
\end{aligned}
$$
$\text{Ker}(T) = \text{span}\{(5, 3, 1)\}$
$\text{dim}[\text{Ker}(T)] = 1$
$\text{Rng}(T) = \text{span}\{(1, 2, 5), (-2, -3, -8)\}$
$\text{dim}[\text{Rng}(T)] = 2$

13\. Consider the linear transformation $S: M_n(R) \to M_n(R)$ defined by $S(A) = A + A^T$, where $A$ is a fixed $2\times 2$ matrix. Determine a basis for $\text{Ker}(S)$, and hence, find its dimension.
>Solution
Let $A=\begin{bmatrix}a & b\\c & d\end{bmatrix}$, then
$$
\begin{aligned}
A^T &= \begin{bmatrix}a & c\\b & d\end{bmatrix}\\
S(A) &= A + A^T = \begin{bmatrix}2a & b+c\\b+c & 2d\end{bmatrix}\\
\end{aligned}
$$
Solve for nullspace
$$
\begin{aligned}
&\begin{cases}
2a = 0 \\
b+c = 0\\
b+c = 0\\
2d = 0
\end{cases}
\To \begin{cases}
a = 0\\
b = t\\
c = -t\\
d = 0
\end{cases}
\To A = t\begin{bmatrix}0 & 1\\-1 & 0\end{bmatrix}
\end{aligned}
$$
$\text{Ker}(S) = \text{span}\bigg\{\begin{bmatrix}0 & 1\\-1 & 0\end{bmatrix}\bigg\}$
$\text{dim}[\text{Ker}(T)] = 1$
$\text{Rng}(S) = \text{span}\bigg\{\begin{bmatrix}1 & 0\\0 & 0\end{bmatrix}, \begin{bmatrix}0 & 1\\1 & 0\end{bmatrix}, \begin{bmatrix}0 & 0\\0 & 1\end{bmatrix}\bigg\}$
$\text{dim}[\text{Rng}(T)] = 3$

14\. Consider the linear transformation $T:M_n(\R) \to M_2n\R)$ defined by
$$
\begin{aligned}
T(A) = AB - BA
\end{aligned}
$$
where $B$ is a fixed $n\times n$ matrix. Describe $\text{Ker}(T)$.
>Solution
$$
\begin{aligned}
T(A) &= AB - BA = 0\\
\To & AB = BA
\end{aligned}
$$
$\text{Ker}(T)$ is a set of matrix that commute with $B$.

15\. Consider the linear transformation $T:P_2(\R) \to P_2(\R)$ defined by
$$
\begin{aligned}
T(ax^2 + bx + c) = ax^2 + (a+2b+c)x +(3a-2b-c)
\end{aligned}
$$
where $a, b$, and $c$ are arbitrary constants.
a. Show that $\text{Ker}(T)$ consists of all polynomials of the form $b(x-2)$, and hence, find its dimension.
b. Find $\text{Rng}(T)$ and its dimension.
>Solution
$$
\begin{aligned}
T(p(x)) &= ax^2 + (a+2b+c)x +(3a-2b-c) = 0\\
&\To \begin{cases}
a & =0\\
a+2b+c & =0\\
3a-2b-c &= 0
\end{cases}\\
&\To \begin{bmatrix}
1 & 0 & 0\\
1 & 2 & 1\\
3 & -2 & -1
\end{bmatrix}
\sim
\begin{bmatrix}
1 & 0 & 0\\
0 & 2 & 1\\
0 & 0 & 0
\end{bmatrix}
\To \begin{cases}
a = 0\\
b = t\\
c = -2t
\end{cases}
\end{aligned}
$$
$\text{Ker}(T) = \text{span}\{x-2\}$
$\text{dim}[\text{Ker}(T)] = 1$
$\text{colspace} = \text{span}\{(1, 1, 3), (0, 1, -1)\}$
$\text{Rng}(T)= \text{span}\{x^2+ x + 3, x-1\}$
$\text{dim}[\text{Rng}(T)] = 2$

16\. Consider the linear transformation $T:P_2(\R) \to P_1(\R)$ defined by
$$
\begin{aligned}
T(ax^2 + bx + c) = (a+b) +(b-c)x
\end{aligned}
$$
where $a, b$, and $c$ are arbitrary constants. Determine $\text{Ker}(T)$, $\text{Rng}(T)$, and their dimension.
>Solution
$$
\begin{aligned}
T(p(x)) &= (a+b) +(b-c)x = 0\\
&\To \begin{cases}
a + b & =0\\
b - c &= 0
\end{cases}\\
&\To \begin{bmatrix}
1 & 1 & 0\\
0 & 1 & -1
\end{bmatrix}
\To \begin{cases}
a = -t\\
b = t\\
c = t
\end{cases}
\end{aligned}
$$
$\text{Ker}(T) = \text{span}\{-x^2-x-1\}$
$\text{dim}[\text{Ker}(T)] = 1$
$\text{colspace} = \text{span}\{(1, 0), (1, 1)\}$
$\text{Rng}(T)= \text{span}\{1, x+1\}$
$\text{dim}[\text{Rng}(T)] = 2$

17\. Consider the linear transformation $T:P_1(\R) \to P_2(\R)$ defined by
$$
\begin{aligned}
T(ax + b) = (b-a) +(2b-3a)x +bx^2
\end{aligned}
$$
Determine $\text{Ker}(T)$, $\text{Rng}(T)$, and their dimension.
>Solution
$$
\begin{aligned}
T(p(x)) &= (b-a) +(2b-3a)x +bx^2\\
&\To \begin{cases}
b - a &= 0\\
2b-3a &= 0\\
b &= 0
\end{cases}\\
&\To \begin{bmatrix}
-1 & 1 \\
-3 & 2 \\
0 & 1
\end{bmatrix}
\sim
\begin{bmatrix}
1 & 0 \\
0 & 1 \\
0 & 0
\end{bmatrix}
\To \begin{cases}
a = 0\\
b = 0\\
\end{cases}
\end{aligned}
$$
$\text{Ker}(T) = \{0\}$
$\text{dim}[\text{Ker}(T)] = 0$
$\text{colspace} = \text{span}\{(-1, -3, 0), (1, 2, 1)\}$
$\text{Rng}(T)= \text{span}\{-3x-1, x^2+2x+1\}$
$\text{dim}[\text{Rng}(T)] = 2$

18\. Consider the linear transformation $T:P_1(\R) \to P_2(\R)$ defined by
$$
\begin{aligned}
T\bigg(\begin{bmatrix} a & b\\c & d\end{bmatrix}\bigg) = (a-b+d) +(-a+b-d)x^2
\end{aligned}
$$
Determine $\text{Ker}(T)$, $\text{Rng}(T)$, and their dimension.
>Solution
$\text{Ker}(S) = \text{span}\bigg\{\begin{bmatrix}1 & 1\\0 & 0\end{bmatrix}, \begin{bmatrix}0 & 0\\1 & 0\end{bmatrix}, \begin{bmatrix}-1 & 0\\0 & 1\end{bmatrix}\bigg\}$
$\text{dim}[\text{Ker}(T)] = 3$
$\text{Rng}(S) = \text{span}\{1-x^2\}$
$\text{dim}[\text{Rng}(T)] = 1$

19\. Consider the linear transformation $T:{\R}^2 \to M_{23}(\R)$ defined by
$$
\begin{aligned}
T(x, y) = \begin{bmatrix}
-x-y & 0 & 2x+2y\\
0 & 3x+3y & -9x-9y
\end{bmatrix}
\end{aligned}
$$
Determine $\text{Ker}(T)$, $\text{Rng}(T)$, and their dimension.
>Solution
$\text{Ker}(S) = \text{span}\{(-1, 1)\}$
$\text{dim}[\text{Ker}(T)] = 1$
$\text{Rng}(S) = \text{span}\bigg\{\begin{bmatrix}-1 & 0 & 2\\ 0 & 3 & -9\end{bmatrix}\bigg\}$
$\text{dim}[\text{Rng}(T)] = 1$

20\. Consider the linear transformation $T:M_{24}(\R) \to M_{42}(\R)$ defined by
$$
T(A) = A^T
$$
Determine $\text{Ker}(T)$, $\text{Rng}(T)$, and their dimension.
>Solution
$\text{Ker}(S) = \{0_{2 \times 4}\}$
$\text{dim}[\text{Ker}(T)] = 0$
$\text{Rng}(S) = M_{42}(\R)$
$\text{dim}[\text{Rng}(T)] = 8$
