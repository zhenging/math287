### 0902 Vector Formulation
The scalar system of equations
$$
\begin{aligned}
x_1' &= a_{11}(t)x_1 t + a_{12}(t)x_2 t + \cdots + a_{1n}(t)x_n t\\[0.5em]
x_2' &= a_{21}(t)x_1 t + a_{22}(t)x_2 t + \cdots + a_{2n}(t)x_n t\\[0.5em]
\cdots\\
x_n' &= a_{n1}(t)x_1 t + a_{n2}(t)x_2 t + \cdots + a_{nn}(t)x_n t
\end{aligned}
$$
can be written as the equivalent vector equation
$$
\begin{aligned}
\boxed{x'(t) = A(t) x_{t} + b(t)}
\end{aligned}
$$
where
$$
\begin{aligned}
x(t) = \begin{bmatrix}
  x_1(t)\\
  x_2(t)\\
  \vdots\\
  x_n(t)
\end{bmatrix} ,\qquad
x'(t) = \begin{bmatrix}
  x_1'(t)\\
  x_2'(t)\\
  \vdots\\
  x_n'(t)
\end{bmatrix}
\end{aligned}
$$
and
$$
\begin{aligned}
A_(t) = \begin{bmatrix}
  a_{11}(t) & a_{12}(t) & \cdots & a_{n1}(t)\\
  a_{21}(t) & a_{22}(t) & \cdots & a_{n2}(t)\\
  \vdots & \vdots &  & \vdots\\
  a_{n1}(t) & a_{n2}(t) & \cdots & a_{nn}(t)
\end{bmatrix}, \quad
b(t) = \begin{bmatrix}
  b_1(t)\\
  b_2(t)\\
  \vdots\\
  b_n(t)
\end{bmatrix}
\end{aligned}
$$

**Wronskian**
Let $x_1(t), x_2(t), \cdots x_n(t)$ be vectors in $V_n(I)$. If $W[x_1, x_2, \cdots , x_n](t_0)$ is _nonzero_ at some point $t_0$ in $I$, then $\{x_1(t), x_2(t), \cdots x_n(t)\}$  is linearly independent on $I$.

**Vector Differential Equation**
A system of linear differential equations written in the vector form
$$
\begin{aligned}
\bold{x'}(t) = A(t)\bold{x}(t) + \bold{b}(t)
\end{aligned}
$$

#### Homework
9.2 p.592 1-4 all, 6, 8, 9
