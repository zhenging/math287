### 6.4 Additional Properties of Linear Transformation

**Inverse Transformation**
If $T$ is both one-to-one and onto, then the **inverse transformation** $T^{-1}: W \to V$ is defined by $T^{-1}(w) = v$ **iff** $w = T(v)$

Let $T:\R^n \to \R^n$ be a linear transformation with matrix $A$.
+ $T^{-1}$ exists **iff** $det(A) \ne 0$.
+ $T^{-1}$ is a lnear transformation with matrix $A^{-1}$.

**Isomorphism and Isomorphic**
If $T: V \to W$ is a linear transformation that is both one-to-one and ont, then $T$ is called an **isomorphism**, and we say that $V$ and $W$ are **isomorphic**.
+ All $n$-dimensional (real) vector spaces are isomorphic to $\R^n$.

**Theorem**
Let $A$ be an $n\times n$ matrix with real elements.
Let $T:\R^n \to \R^n$ be the matrix transformation defined by $T(x) = Ax$ .
The following conditions on $A$ are equivalent.
1. $A$ is invertible.
2. $Ax = b$ has a unique solution for every $b$ in $\R^n$.
3. $Ax = 0$ has the only trivial solution for $x=0$.
4. $\text{rank}(A) = n$.
5. $A$ is row-equivalent to $I_n$.
6. $\text{det}(A) \ne 0$.
7. $A^T$ is invertible.
8. $\text{nullity}(A) = 0$
9. $\text{colspace}(A) = \R^n$ (that is, the columns of $A$ form a basis for $\R^n$).
10. $\text{rowspace}(A) = \R^n$ (that is, the rows of $A$ form a basis for $\R^n$).
11. $T$ is an isomorphism.

#### Homework
p.417 10-14 all, 18-22 all, 25-35 all (#19-book answer wrong)

19\. Define $T: P_2(\R^2) \to \R^2$ by
$$
\begin{aligned}
T(ax^2 + bx + c) = (a-3b+2c, b-c)
\end{aligned}
$$
Determine whether $T$ is one-to-one, onto,both, or neither. Find $T^{-1}$ or explain why it does not exist.
>Solution
$T$ is onto but not one-to-one, $T^{-1}$ DNE.

20\. Let $V$ denote the vector space of $2\times 2$ symetrix matrices and define $T: V \to P_2(\R)$ by
$$
\begin{aligned}
T\bigg(\begin{bmatrix}a & b\\ b & c\end{bmatrix}\bigg) = ax^2 + bx + c
\end{aligned}
$$
Determine whether $T$ is one-to-one, onto,both, or neither. Find $T^{-1}$ or explain why it does not exist.
>Solution
$T$ is both onto and one-to-one. $T^{-1}(ax^2 + bx + c) = \begin{bmatrix}a & b\\ b & c\end{bmatrix}$
