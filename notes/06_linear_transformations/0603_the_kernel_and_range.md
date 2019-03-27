### 6.3 The kernel and range of a linear transformation

**Kernel**
Let $T:V \to W$ be a linear transformation. The set of all vectors $v$ in $V$ such that $T(v) = 0$ is called the kernel of the $T$ and is denoted by $\text{Ker}(T)$.

**Range**
The **range** of $T:V \to W$ is the subset of $W$ consisting of all transformed vectors from $V$. The range of T is denoted by $\text{Rng}(T)$.

If $T: V \to W$ is a linear transformation, then
+ $\text{Ker}(T)$ is a subspace of $V$.
+ $\text{Rng}(T)$ is a subspace of $W$.

If $T:\R^n \to \R^m$ is a linear transformation, then
+ $\text{Ker}(T) = \text{nullspace}(A)$, which is a subspace of $\R^n$
+ $\text{Rng}(T) = \text{colspace}(A)$, which is a subspace of $\R^m$

**General Rank-Nullity Theorem**
If $T: V \to W$ is a linear transformation and $V$ is finite-dimensional, then
$$
\begin{aligned}
\text{dim}[\text{Ker}(T)] + \text{dim}[\text{Rng}(T)] = \text{dim}(V)
\end{aligned}
$$

**One-To-One / Onto**
If $T: V \to W$ is a linear transformation.
+ $T$ is _one-to-one_ **iff** the preimage of every $w$ in the range consists of a single vector. That is whenever $v_1 \ne v_2, T(v_1) \ne T(v_2)$.
+ $T$ is _onto_ **iff** every element of $W$ has a preimage in $V$.
+ $T$ is one-to-one **iff** $\text{Ker}(T) = {0}$.
+ $T$ is onto **iff** $\text{Rng}(T) = W$. (This is one is immediate from the definition.)

If $T: V \to W$ is a linear transformation, and let $V$ and $W$ be finite-dimensional.
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
$T: \R^3 \to \R^3$ defined by $T(x) = Ax$, where $A = \begin{bmatrix}
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

13\, Consider the linear transformation $S: M_n(R) \to M_n(R)$ defined by $S(A) = A + A^T$, where A is a fixed $2\times 2$ matrix. Determine a basis for $\text{Ker}(T)$, and hence, find its dimension.
>Solution
