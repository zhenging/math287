### 6.1 Definition of a Linear Transformation

**Mapping**
Let $V$ and $W$ be vector spaces. A **mapping** $T$ from $V$ into $W$ is a rule that assigns to each vector $v$ in $V$ precisely on vector $w=T(v)$ in $W$. We denote such a mapping by $T:V \to W$.
$w$ is called the **image** of $v$.
$v$ is called the **preimage** of $w$.

**Examples**
1\. $T: \R^3 \to \R^2$, defined by $T(x, y, z) = (x-y, x-2z)$
2\. $T: \R^2 \to \R^2$, defined by $T(x, y) = (x+3, y)$
3\. $T: \R \to \R$, defined by $T(x) = x+1$

**Linear Transformation**
A mapping $V \to W$ is called a linear transformation from V to W if it satisfies the following properties
(1) $T(u+v) = T(u) + T(v)$ for all $u, v$ in $V$.
(2) $T(cv) = cT(v)$ for all $v$ in $V$ and all scalars $c$.
These properties are called the linearly properties.
$V$ is called the **domain** of $T$.
$W$ is called the **codomain** of $T$.
+  $T(c_1v_1 + c_2v_2) = c_1T(v_1) + c_2T(v_2)$ for all $v_1, v_2$ in $V$ and scalars $c_1, c_2$
+  $T(0v) = 0w$
+  $T(-v) = -T(v)$ for all $v$ in $V$.

**Matrix of $T$**
If $T: \R^n \to \R^m$ is a linear transformation, then the matrix of $T$ is $A = [T(e_1), T(e_2), \cdots T(e_n)]$.
+ Every $m\times n$ matrix represents a linear transformation from $\R^n$ to $\R^m$.
+ Eveyr linear transformation from $\R^n$ to $\R^m$ can be represented by an $m\times n$ matrix.

#### Homework
p.389 14-23 all

14-18\. Determine the matrix of the given transformation. $T: \R^n \to \R^m$
14\. $T(x_1, x_2) = (3x_1-2x_2, x_1 + 5x_2)$
>Solution
Let the matrix of the given transformation be $A$.
$$
\begin{aligned}
e_1 &= (1, 0), T(e_1) = (3, 1)\\
e_2 &= (0, 1), T(e_2) = (-2, 5)\\
A &= [T(e_1), T(e_2)]\\
&= \begin{bmatrix}
3 & -2\\
1 & 5
\end{bmatrix}
\end{aligned}
$$

15\. $T(x_1, x_2) = (x_1+3x_2, 2x_1 - 7x_2, x_1)$
>Solution
Let the matrix of the given transformation be $A$.
$$
\begin{aligned}
e_1 &= (1, 0), T(e_1) = (1, 2, 1)\\
e_2 &= (0, 1), T(e_2) = (3, -7, 0)\\
A &= [T(e_1), T(e_2)]\\
&= \begin{bmatrix}
1 & 3\\
2 & -7\\
1 & 0
\end{bmatrix}
\end{aligned}
$$

19-23\. Determine the linear transformation  $T: \R^n \to \R^m$ that has the given matrix.
19\. $A= \begin{bmatrix}
1 & 3\\
-4 & 7
\end{bmatrix}$
>Solution
$$
\begin{aligned}
&\begin{bmatrix}
1 & 3\\
-4 & 7
\end{bmatrix}
\begin{bmatrix}
x_1 \\
x_2
\end{bmatrix} =
\begin{bmatrix}
x_1 + 3x_2\\
-4x_1+7x_2
\end{bmatrix}\\[1.0em]
&T(x_1, x_2) = (x_1 + 3x_2, -4x_1+7x_2)
\end{aligned}
$$

21\. $A= \begin{bmatrix}
2 & 2 & -3\\
4 & -1 & 2\\
5 & 7 & -8
\end{bmatrix}$
>Solution
$$
\begin{aligned}
&\begin{bmatrix}
2 & 2 & -3\\
4 & -1 & 2\\
5 & 7 & -8
\end{bmatrix}
\begin{bmatrix}
x_1 \\
x_2 \\
x_3
\end{bmatrix} =
\begin{bmatrix}
2x_1 + 2x_2 - 3x_3\\
4x_1 - x_2 - 2x_3\\
5x_1+7x_2 -8x_3
\end{bmatrix}\\[1.0em]
&T(x_1, x_2) = (2x_1 + 2x_2 - 3x_3, 4x_1 - x_2 - 2x_3, 5x_1+7x_2 -8x_3)
\end{aligned}
$$
