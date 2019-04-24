### 0801 General Theory for Linear Transformation

**Derivative Operator**
The mapping $D: C^1(I) \to C^0(I)$ defined by $D(f) = f'$ is a _linear transformation._. We call $D$ the **derivative operator**. Higher-order derivative operators can be defined by composition. Thus $D^k: C^k(I) \to C^0(I)$ is defined by
$$
\begin{aligned}
D^k = D(D^k-1), k = 2, 3, \cdots
\end{aligned}
$$
so that
$$
\begin{aligned}
D^k(f) = \frac{d^k f}{dx^k}
\end{aligned}
$$
By taking a linear combination of the basic derivative operators, we obtain the general **linear differential operator of order** $n$.
$$
\begin{aligned}
\tag{8.1.1} L = D^n + a_1 D^{n-1} + \cdots + a_{n-1} D + a_n
\end{aligned}
$$
defined by
$$
\begin{aligned}
Ly = y^{(n)} + a_1 y^{(n-1)} + \cdots + a_{n-1} y' + a_n y
\end{aligned}
$$
where the $a_i$ are functions of $x$.

##### Example 8.1.1
If $L = D^2 + 4xD - 3x$, then
$$
\begin{aligned}
Ly = y'' + 4xy' - 3xy
\end{aligned}
$$
so that, for example
$$
\begin{aligned}
L(\sin x) &= -\sin x + 4x \cos x - 3x\sin x\\
L(x^2) &= 2 + 8x - 3x^3
\end{aligned}
$$

##### Example 8.1.2
Determine the kernel of the linear differential operatpr $L = D-2x$
>Solution
The kernel of $L$ consists of all function that satisfy $Ly = 0$; that is all solution to the differential equation
$$
\begin{aligned}
y' - 2xy = 0
\end{aligned}
$$


**Homogeneous Linear Differential Equation**
Now consider the general n-th order linear differential equation
$$
\begin{aligned}
\tag{8.1.2} a_0(x)y^{(n)} + a_1 y^{(n-1)} + \cdots + a_{n-1} y' + a_n y = F(x)
\end{aligned}
$$
where $a_0 \ne 0, a_1, \cdots , a_n$ and $F$ are functions specified on the interval $I$. If $F(x)$ is identically zero on $I$, then the differential equation $(8.1.2)$ is called **homogeneous**. Otherwise, it is called **nonhomogeneous**.

#### Homework
8.1 p.503 1-5 odd, 6, 7, 10, 13, 17, 18, 23, 25, 28, 30
