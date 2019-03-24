### 4.7 Change of Basis

**Ordered Basis**
An **ordered basis** is a basis in which we are keeping track of the order in which the basis vectors are written.

**Component Vector**
Let $V$ be a vector space with ordered basis $B = \{v_1, v_2, v_3\}$, and let $v$ be a vector in $V$, then $v = c_1v_1 + c_2v_2 + c_3v_3$ is the unique representation of $v$ as a linear combination of $B$.
The **component vector of $v$ relative to $B$** is written $\begin{bmatrix}c_1 \\ c_2 \\ c_2 \end{bmatrix}$ or $(c_1, c_2, c_3)$.
We use the notation $[v]_B = (c_1, c_2, c_3)$.

**Change of basis matrix from $B$ to $C$**
Let V be a vector space with ordered bases $B = \{v_1, v_2, v_3\}$ and $C=\{w_1, w_2, \cdots w_n\}$. The matrix
$$
P_{C \leftarrow B} = [[v_1]_C, [v_2]_C, [v_3]_C]
$$
is called the **change of basis matrix from $B$ to $C$**.
The matrix changed vectors writtern in terms of B to vectors written in terms of $C$.
+ $[v]_C = P_{C \leftarrow B} [v]_B$
+ $P_{B \leftarrow C}$ is the inverse of $P_{C \leftarrow B}$.

#### Homework
p.318 1-11 odd, 12, 13, 17-20 all, 27, 28, 33, 34

1-14\. Determine the component of vector of the givern vector in the vector space $V$ relative to the given ordered basis $B$.

1\. $V = \R^2; B=\{(7, -1), (-9, -2)\}; v=(27, 6)$
>Solution
Let $v_1 = (7, -1)$, and $v_2 = (-9, -2)$
$$
\begin{aligned}
&c_1v_1 + c_2 v_2 = v\\
&\begin{bmatrix}
v_1 & v_2\\
\end{bmatrix}
\begin{bmatrix}
c_1\\
c_2
\end{bmatrix} = v\\[1.0em]
&\begin{bmatrix}
7 & -9\\
-1 & -2
\end{bmatrix}
\begin{bmatrix}
c_1\\
c_2
\end{bmatrix} = \begin{bmatrix}
27\\
6
\end{bmatrix}\\[1.0em]
&\begin{array}{cc|c}
7 & -9 & 27\\
-1 & -2 & 6
\end{array}
\sim
\begin{array}{cc|c}
1 & 0 & 0\\
0 & 1 & -3
\end{array}\\[1.0em]
&[v]_B = (0, -3)
\end{aligned}
$$

5\. $V = \R^3; B=\{(1, -6, 3), (0, 5, -1), (3, -1, -1)\}; v=(1, 7, 7)$
>Solution
Let $v_1 = (1, -6, 3)$, $v_2 = (0, 5, -1)$ and $v_3=(3, -1, -1)$
$$
\begin{aligned}
&c_1v_1 + c_2 v_2 +c_3 v_3 = v\\
&\begin{bmatrix}
v_1 & v_2 & v_3\\
\end{bmatrix}
\begin{bmatrix}
c_1\\ c_2\\ c_3
\end{bmatrix} = v\\[1.5em]
&\begin{bmatrix}
1 & 0 & 3\\
-6 & 5 & -1\\
3 & -1 & -1
\end{bmatrix}
\begin{bmatrix}
c_1\\ c_2\\ c_3
\end{bmatrix} =
\begin{bmatrix}
1 \\ 7 \\ 7
\end{bmatrix}\\[1.5em]
&\begin{array}{ccc|c}
1 & 0 & 3 & 1\\
-6 & 5 & -1 & 7\\
3 & -1 & -1 & 7
\end{array}
\sim
\begin{array}{ccc|c}
1 & 0 & 0 & 4\\
0 & 1 & 0 & 6\\
0 & 0 & 1 & -1
\end{array}\\[1.0em]
&[v]_B = (4, 6, -1)
\end{aligned}
$$

12\. $V=M_2(R)$; $B=\bigg\{
\begin{bmatrix}
1 & 1\\
1 & 1
\end{bmatrix},
\begin{bmatrix}
1 & 1\\
1 & 0
\end{bmatrix},
\begin{bmatrix}
1 & 1\\
0 & 0
\end{bmatrix},
\begin{bmatrix}
1 & 0\\
0 & 0
\end{bmatrix}
\bigg\}$; $A=\begin{bmatrix}
-3 & -2\\
-1 & 2
\end{bmatrix}$
>Solution
$$
\begin{aligned}
&\begin{bmatrix}
1 & 1 & 1 & 1\\
1 & 1 & 1 & 0\\
1 & 1 & 1 & 1\\
1 & 1 & 1 & 1
\end{bmatrix}
\begin{bmatrix}
c_1\\ c_2\\ c_3\\ c_4
\end{bmatrix} =
\begin{bmatrix}
-3\\ -2\\ -1\\ 2
\end{bmatrix}\\[1.5em]
&\begin{array}{cccc|c}
1 & 1 & 1 & 1 & -3\\
1 & 1 & 1 & 0 & -2\\
1 & 1 & 1 & 1 & -1\\
1 & 1 & 1 & 1 & 2
\end{array}
\sim
\begin{array}{cccc|c}
1 & 0 & 0 & 0 & 2\\
0 & 1 & 0 & 0 & -3\\
0 & 0 & 1 & 0 & -1\\
0 & 0 & 0 & 1 & -1
\end{array}\\[1.0em]
&[A]_B = (2, -3, -1, -1)
\end{aligned}
$$

17-20\. Find the change of basis matrix $P_{C \leftarrow B}$ from the given ordered basis $B$ to the given ordered basis $C$ of the vector space $V$.
17\. $V = \R^2$; $B=\{(9, 2), (4, -3)\}$; $C=\{(2, 1), (-3, 1)\}$
>Solution
$$
\begin{aligned}
&\begin{array}{cc|cc}
2 & -3 & 9 & 4\\
1 & 1 & 2 & -3
\end{array}
\sim
\begin{array}{cc|cc}
1 & 0 & 3 & -1\\
0 & 1 & -1 & -2
\end{array}\\[1.0em]
&P_{C \leftarrow B} = \begin{bmatrix}
3 & -1\\
-1 & -2
\end{bmatrix}
\end{aligned}
$$
