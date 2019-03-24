### 5.2 Orthogonal Sets of Vectors and Orthogonal Projections

**Unit Vector**
If a vector has norm of 1, then it is called a **unit vector**.

**Normalization**
If v is any nonzero vector in an inner product space **V**, then the vector $u=\dfrac{v}{||v||}$ is a unit vector in the direction of $v$. The process of replacing $v$ with $u$ is called **normalization**.

**Orthogonal**
A set $S$ of nonzero vectors in an inner product space $V$ is called orthogonal if every pair of vectors in $S$ is **orthogonal**. If, in addition each vector in the set is a unit vector, then S is called **orthonormal**.

**Theorems**
+ If $S$ is an orthogonal set of nonzero vectors in an inner product space $V$, then $S$, is linearly independent.
+ If $V$ is an inner product space of dimension $n$, then any orthogonal set of $n$ vector is a basis of $V$.
+ Let $V$ be an inner product space with orthogonal basis $B= \{v_1, v_2, v_3\}$. Let $u$ be a vector in $V$, then the component vector of $u$ relative to $B$ is $[u]_B = \begin{bmatrix} \la u, v_1\ra \\ \la u, v_2\ra \\\la u, v_3\ra\end{bmatrix}$.

#### Homework
p.359 1-6 all, 8, 15, 19, 20

8\. Let $v_1=(1, 2, 3)$ and $v_2=(1, 1, -1)$. Determine all nonzero vectors $w$ in $\R^3$ such that $[v_1, v_2, w]$ is an orthogonal set.
>Solution
Let $w = (x, y, z)$, then
$$
\begin{aligned}
x + 2y + 3z &= 0\\
x + y - z &= 0
\end{aligned}
$$
Solve the equation using matrix
$$
\begin{aligned}
&\begin{bmatrix}
1 & 2 & 3\\
1 & 1 & -1
\end{bmatrix}
\sim
\begin{bmatrix}
1 & 2 & 3\\
0 & 1 & 4
\end{bmatrix}\\[1em]
\To &(x, y, z) = (5t, -4t, t)\\
w &= t(5, -4, 1)
\end{aligned}
$$

15\. Show that given functions in $C^0[-1, 1]$ are orthogonal, and use them to construct an orthonormal set of functions in $C^0[-1, 1]$.
$f_1(x) = 1, f_2(x) = x, f_3(x) = \dfrac{1}{2}(3x^2 -1)$
>Solution
$$
\begin{aligned}
\la f_1(x), f_2(x) \ra &= \int_{-1}^1 x dx \\
&= \frac{1}{2} x^2 |_{-1}^1 = 0\\
\la f_2(x), f_3(x) \ra &= \int_{-1}^1 \frac{1}{2}x(3x^2 -1) dx \\
&= (\frac{3}{8}x^4 - \frac{1}{4}x^2)|_{-1}^1 = 0\\
\la f_1(x), f_3(x) \ra &= \int_{-1}^1 \frac{1}{2}(3x^2 -1) dx \\
&= (\frac{1}{2}x^3 - \frac{1}{2}x^)|_{-1}^1 = 0\\
||f_1(x)||^2 &= \la f_1(x), f_1(x) \ra = \int_{-1}^1  dx\\
&= x|_{-1}^1 = 2\\
\To ||f_1(x)|| &= \sqrt 2\\
||f_2(x)||^2 &= \la f_2(x), f_2(x) \ra = \int_{-1}^1 x^2 dx \\
&= (\frac{1}{3}x^3)|_{-1}^1 = \frac{2}{3}\\
\To ||f_2(x)||  &= \frac{\sqrt 6}{3}\\
||f_3(x)||^2 &= \la f_3(x), f_3(x) \ra = \int_{-1}^1 \frac{1}{4}(3x^2 -1)^2 dx \\
&= (\frac{9}{20}x^5 - \frac{1}{2}x^3 + \frac{1}{4}x)|_{-1}^1 = \frac{2}{5}\\
\To ||f_3(x)||  &= \frac{\sqrt {10}}{5}\\
\end{aligned}
$$
Orthonormal set is $\{\dfrac{\sqrt 2}{2}, \dfrac{3}{\sqrt 6} x, \dfrac{5}{2\sqrt {10}}(3x^2 - 1)\}$.

20\. Let $A_1 = \begin{bmatrix} 1 & 1 \\-1 & 2 \end{bmatrix}$, $A_2 = \begin{bmatrix} -1 & 1 \\2 & 1 \end{bmatrix}$, and $A_3 = \begin{bmatrix} -1 & -3 \\0 & 2 \end{bmatrix}$. Use the inner product
$$
\la A, B\ra = a_{11}b_{11} + a_{12}b_{12} +a_{21}b_{21} +a_{22}b_{22}
$$
to find all matrices $A_4 = \begin{bmatrix} a & b \\c & d \end{bmatrix}$ such that $\{A_1, A_2, A_3, A_4\}$ is an orthogonal set of matrices in $M_2(\R)$.
>Solution
$$
\begin{aligned}
&\begin{bmatrix}
1 & 1 & -1 & 2 \\
-1 & 1 & 2 & 1 \\
-1 & -3 & 0 & 2
\end{bmatrix}
\sim
\begin{bmatrix}
1 & 1 & -1 & 0 \\
0 & 1 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}\\[2em]
\To &(a, b, c, d) = (\frac{3}{2}t, \frac{-1}{2}t, t, 0), t \ne 0\\[1em]
A_4 &= 2t\begin{bmatrix} 3 & -1 \\ 2 & 0 \end{bmatrix}
\end{aligned}
$$
