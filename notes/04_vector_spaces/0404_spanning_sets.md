### 4.4 Spanning Sets
Let $V$ be a vector space.
Let $S = \{v_1, v_2, \cdots v_3 \}$ be a subset of $V$.
Let $c_1, c_2, \cdots c_n$ be scalars.

+ $u$ is a linear combination of $v_1, v_2, \cdots v_k$, **iff** $u= c_1v_1 + c_2v_2 + \cdots + c_kv_k$
+ Forming all poosible linear combination of $v_1, v_2, \cdots v_k$ generates a subset of $V$ called the **linear span** of $v_1, v_2, \cdots v_k$, denoted by $\text{Span}\{v_1, v_2, \cdots v_k\}$ or $\text{Span} (S)$.
+ $\text{Span} (S)$ is a subspace of $V$.
+ If $\text{Span} (S) = T$, then $S$ is a spanning set of $T$. We can say "$S$ spans $T$" or "$T$ is spanned by $S$".
+ Any 3 nonzero, noncoplanear vector in $\R^3$ span $\R^3$.
+ Any 2 nonzero, nonlinear vector in $\R^2$ span $\R^2$.

#### Example
**Ex.2** Finding a Spanning Set for the nullspace of A.
>Solution
$$
\begin{aligned}
&A = \begin{bmatrix}
1 & 0 & -2 & 1\\
3 & 1 & -5 & 0\\
1 & 2 & 0 & -5
 \end{bmatrix}
\sim
\begin{bmatrix}
1 & 0 & -2 & 1\\
0 & 1 & 1 & -3\\
0 & 0 & 0 & 0
 \end{bmatrix}\\
&\To \begin{cases}
x_1 &= 2s-t \\
x_2 &= -s+3t \\
x_3 &= s \\
x_4 &= t
\end{cases}\\
  &\text{Solution Set }  S = \{(2s-t,-s+3t, s, t)\}\\
 &\text{nullspace}(A) = S\\
 &{(2s-t,-s+3t, s, t)} = s(2, -1, 1, 0) + t(-1, 3, 0, 1)\\
 &\text{One spanning set is span } \{(2, -1, 1, 0), (-1, 3, 0, 1)\}
\end{aligned}
$$

**EX.3** Does $S= \{(1, 2, 3), (0, 1, 2), (-2, 0, 1)\}$ span $\R^3$?
>Solution
Let $A = \begin{bmatrix}
1 & 0 & -2 \\
2 & 1 & 0 \\
3 & 2 & 1
 \end{bmatrix}$,
 $$
 det(A) = 1(1) + (-2)(1) = -1 \ne 0
 $$
 Thus $S$ spans $\R^3$.
