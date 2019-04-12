### 6.5 The Matrix of a Linear Transformation

Let $V$ and $W$ be vector spaces, with ordered bases $B=\{v_1, v_2, \cdots v_n\}$ and $C=\{w_1, w_2, \cdots w_n\}$, respectively.

Let $T:V \to W$ be a linear transformation
The $m\times n$ matrix
$$
\begin{aligned}
[T]_B^C = \big[ [T(v_1)]_c, [T(v_2)]_c, \cdots [T(v_n)]_c,\big]
\end{aligned}
$$
is called the **matrix representation of $T$ relative to the base $B$ and $C$**.

If $T:V = \R^n$ and $W = \R^m$ are each equipped with the standard bases, then $[T]_B^C$ is just the matrix of $T$ defined earlier.

If $V=W$ and $T(v) = v$ for all $v$ in $V$, then $[T]_B^C$ is just the change of basis matrix from $B$ to $C$ defined earlier.

$[T(v)]_C = [T]_B^C[v]_B$

#### Homework
p.426 1a, 2a, 3a, 4a

1-4\. Determine the matrix representation $[T]_B^C$ for the given linear transformation $T$ and ordered bases $B$ and $C$.

1\. $T:M_2(\R) \to P_3(\R)$ given by
$$
\begin{aligned}
T\bigg(\begin{bmatrix} a & b\\c & d\end{bmatrix}\bigg) = (a-d) + 3bx^2 + (c-a)x^3
\end{aligned}
$$
$B=\{E_{11}, E_{12}, E_{21}, E_{22}\}$ and $C=\{1, x, x^2, x^3\}$
>Solution
$$
\begin{aligned}
[T(E_{11})]_C &= [1-x^3]_C = \begin{bmatrix} 1\\0 \\ 0\\-1\end{bmatrix}\\[2.5em]
[T(E_{12})]_C &= [3x^2]_C = \begin{bmatrix} 0\\0 \\ 3\\0\end{bmatrix}\\[2.5em]
[T(E_{21})]_C &= [x^3]_C = \begin{bmatrix} 0\\0 \\ 0\\1\end{bmatrix}\\[2.5em]
[T(E_{22})]_C &= [3x^3]_C = \begin{bmatrix} -1\\0 \\ 0\\0\end{bmatrix}\\[2.5em]
[T]_B^C &= \begin{bmatrix}
1 & 0 & 0 & -1\\
0 & 0 & 0 & 0\\
0 & 3 & 0 & 0\\
-1 & 0 & 1 & 0
\end{bmatrix}
\end{aligned}
$$

3\. $T:P_2(\R) \to P_3(\R)$ given by
$$
\begin{aligned}
T(p(x)) = (x+1)p(x)
\end{aligned}
$$
$B=\{1, x, x^2\}$ and $C=\{1, x, x^2, x^4\}$
>Solution
Let $p(x) = a+bx+cx^2$
$$
\begin{aligned}
T(p(x)) &= (x+1)p(x)\\
T(a+bx+cx^2) &= a + (a+b)x + (b+c)x^2 + cx^3\\
v_1 &= 1\\
\To &a = 1, b = 0, c = 0\\
T(v_1) &= 1 + x \\
1 + x  &= 1 \times 1 + 1 \times x + 0 \times x^2 + 0 \times x^3\\
[T(1)]_C &= [1 + x ]_C = \begin{bmatrix} 1\\ 1\\ 0\\ 0 \end{bmatrix}\\[2.5em]
[T(x)]_C &= [x + x^2 ]_C = \begin{bmatrix} 0\\ 1\\ 1\\ 0 \end{bmatrix}\\[2.5em]
[T(x^2)]_C &= [x^2 + x^3 ]_C = \begin{bmatrix} 0\\ 0\\ 1\\ 1 \end{bmatrix}\\[1.5em]
[T]_B^C &= \begin{bmatrix}
1 & 0 & 0\\
1 & 1 & 0\\
0 & 1 & 1\\
0 & 0 & 1
\end{bmatrix}
\end{aligned}
$$

2\. $T:P_2(\R) \to \R^2$ given by
$$
\begin{aligned}
T(a+bx+cx^2) = (a-3c, 2a + b-2c)
\end{aligned}
$$
$B=\{1, x, x^2\}$ and $C=\{(1, 0), (0, 1)\}$
>Solution
$$
\begin{aligned}
v_1 &= 1\\
\To &a = 1, b = 0, c = 0\\
T(v_1) &= (1 - 3 \times 0, 2 \times 1 + 0 - 2\times 0) \\
&= (1, 2)\\
(1, 2) &= 1 \times (1, 0) + 2 \times (0, 1)\\[1.5em]
[T(1)]_C &= [(1, 2)]_C = \begin{bmatrix} 1\\2 \end{bmatrix}\\[1.5em]
[T(x)]_C &= [(0, 1)]_C = \begin{bmatrix} 0\\1 \end{bmatrix}\\[1.5em]
[T(x^2)]_C &= [(-3, -2)]_C = \begin{bmatrix} -3\\-2 \end{bmatrix}\\[1.5em]
[T]_B^C &= \begin{bmatrix}
1 & 0 & -3\\
2 & 1 & -2
\end{bmatrix}
\end{aligned}
$$

4\. $T:\R^3 \to \text{span}\{\cos x, \sin x \}$ given by
$$
\begin{aligned}
T(a, b, c) = (a-2c)\cos x + (3b + c) \sin x
\end{aligned}
$$
$B=\{(1, 0, 0), (0, 1, 0), (0, 0, 1)\}$ and $C=\{\cos x, \sin x\}$
>Solution
$$
\begin{aligned}
v_1 &= (1, 0, 0)\\
\To &a = 1, b = 0, c = 0\\
T(v_1) &= (a-2c)\cos x + (3b + c) \sin x \\
&= \cos x\\
\cos x &= 1 \times \cos x + 0 \times \sin x\\[1.5em]
[T((1, 0, 0))]_C &= [\cos x]_C = \begin{bmatrix} 1\\0 \end{bmatrix}\\[1.5em]
[T((0, 1, 0))]_C &= [3\sin x]_C = \begin{bmatrix} 0\\3 \end{bmatrix}\\[1.5em]
[T((0, 0, 1))]_C &= [-2\cos x + \sin x]_C = \begin{bmatrix} -2\\1 \end{bmatrix}\\[1.5em]
[T]_B^C &= \begin{bmatrix}
1 & 0 & -3\\
2 & 1 & -2
\end{bmatrix}
\end{aligned}
$$
