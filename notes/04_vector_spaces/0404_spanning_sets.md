### 4.4 Spanning Sets

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
 &x_1 = 2s-t, x_2 = -s+3t, x_3 = s, x_4 = t\\
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
