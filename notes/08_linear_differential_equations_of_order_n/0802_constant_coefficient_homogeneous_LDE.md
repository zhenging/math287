### 0802 Constant Coefficient Homogeneous Linear Differential Equation

Consider the differential equation
$$
\begin{aligned}
\tag{8.2.7} P(D)y = 0
\end{aligned}
$$
Let $r_1, r_2, \cdots r_k$ be the distinct roots of the auxiliary equation, so that
$$
\begin{aligned}
P(r) = (r-r_1)^{m_1}(r-r_2)^{m_2}\cdots (r-r_k)^{m_k}
\end{aligned}
$$
where $m_i$ denotes the multiplicity of the root $r=r_i$.
1. If $r_i$ is real, then the functions $e^{r_i x}, xe^{r_i x} \cdots, x^{m_i-1}e^{r_i x}$ are linearly independent solution to Equation (8.2.7) on any interval.
2. If $r_j$ is _complex_, say $r_j = a + ib$ ($a$ and $b$ are real, and $b \ne 0$), then the functions
$$
\begin{aligned}
e^{ax} \cos{bx}, x e^{ax} \cos{bx}, \cdots, x^{m_i-1} e^{ax} \cos{bx}\\
e^{ax} \sin{bx}, x e^{ax} \sin{bx}, \cdots, x^{m_i-1} e^{ax} \sin{bx}
\end{aligned}
$$
corresponding to the conjugate roots $r = a\pm ib$ are linearly independent solution to Equation (8.2.7) on any interval.
3. The $n$ real-valied solution $y_1, y_2, \cdots, y_n$ to Equation (8.2.7) that are obtained by considering the distinct roots $r_1, r_2, \cdots r_k$ are linearly independent on any interval. Consequently, the general solution to Equation (8.2.7) is
$$
\begin{aligned}
y(x) = c_1 y_1(x) + c_2 y_2(x) + \cdots + c_n y_n(x)
\end{aligned}
$$

#### Example
Solve $y'' - 6y' + 13y  = 0$
$$
\begin{aligned}
& r^2-6r + 13 = 0\\
\To & r_1 = 3 + 2i, r_2 = 3 - 2i\\
y &= c_1 e^{(3 + 2i)x} + c_2 e^{(3 2 2i)x} \\
&= c_1 e^{3x}e^{2ix} + c_1 e^{3x}e^{-2ix} \\
&= e^{3x} \big[ c_1 e^{i(2x)} + c_2 e^{i(-2x)} \big] \\
&= e^{3x} \big[ c_1\cos{2x} + c_1 i\sin{2x} + c_2\cos(-2x) + c_2 i\sin(-2x) \big]\\
&= e^{3x} \big[ c_1\cos{2x} + c_1 i\sin{2x} + c_2\cos{2x} - c_2 i\sin{2x}\big]\\
&= e^{3x} \big[ (c_1 + c_2)\cos{2x} + (c_1 i - c_2 i) \sin{2x} \big]\\
&\boxed{= e^{3x}(c_3\cos 2x + c_4 \sin 2x)}
\end{aligned}
$$

#### Euler Identity
$$
\begin{aligned}
e^{ix} &= \sum_{n=0}^\infty \frac{(ix)^n}{n!}\\
&= 1 + \frac{(ix^1}{1!} + \frac{(ix)^2}{2!} + \frac{(ix)^3}{3!} +\frac{(ix)^4}{4!} + \cdots\\
&= 1 + \frac{ix}{1!} + \frac{i^2 x^2}{2!} + \frac{i^3 x^3}{3!} +\frac{i^4 x^4}{4!} + \cdots\\
&= 1 + \frac{ix}{1!} - \frac{x^2}{2!} + \frac{i x^3}{3!} -\frac{x^4}{4!} + \cdots\\
\end{aligned}
$$

#### Homework
8.2 p.513 9-37 odd
