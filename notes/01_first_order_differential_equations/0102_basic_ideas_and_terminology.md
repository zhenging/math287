### 1.2 Basic Ideas and  Terminology

**Linear Differential Equations**
A differntial equation that can be written in the form
$$
\begin{aligned}
a_0(x)y^{(n)} + a_1(x)y^{(n-1)} + \cdots + a_n(x)y = F(x)
\end{aligned}
$$
where $a_0, a_1, \cdots a_n$ and $F$ are functions of $x$ only, is called a **linear** differntial equation of order _n_. Such a differntial equation is **linear** in $y, y', y'', \cdots, y^{n}$.

**Examples**
The following equations are **linear** differntial equations of order 3 and order 1.
$$
\begin{aligned}
y''' +  e^{3x}y'' + x^3y' + (\cos x)y &= \ln x\\
xy' - \frac{2}{1+x^2}y &= 0
\end{aligned}
$$
The following equation sare nonlinear. In the first case, the nonlinearity arises from the $\cos(y')$ term, whereas in the second equations the nonlinearity is due to the $y^2$ term.
$$
\begin{aligned}
y'' +  x^4 \cos(y') - xy &= e^{x^2}\\
y'' + y^2 &= 0
\end{aligned}
$$

**General Solution**
A solution to an $n$th-order differntial equation on an interval $I$ is called the **general solution** on $I$ if it satisfies the following contions:
1. The solution contains $n$ constant $c_1, c_2 \cdots, c_n$.
2. All solutions to the differential equtions can be obtained by passing appropriate values to the constants.

#### Homework
1.2 p.21 1-6 all, 33-35 all, 37-40 all, 42, 43

1-6\. Determine whether the differntial equation is linear or nonlinear.
2\. $\d \frac{d^3 y}{dx^3} + 4 \frac{d^2 y}{dx^2} + \sin x \frac{dy}{dx} = xy^2 + \tan x$
>Solution
Nonlinear. ($xy^2$)

4\. $\sin x \cdot y'' + y' - \tan y = \cos x$
>Solution
Nonlinear. ($\tan y$)

6\. $\d\sqrt{x} y'' + \frac{1}{y'}\ln x = 3x^3$
>Solution
Nonlinear. ($\dfrac{1}{y'}$)

37-40\. Solve the given _initial-value problem_.
37\. $y' = x^2 \ln x$, $y(1) = 2$
>Solution
$$
\begin{aligned}
y &= \int x^2 \ln x dx\\
u &= \ln x, du = \frac{1}{x} dx, dv = x^2 dx, v = \frac{1}{3}x^3\\
y &= uv - \int vdu\\
&= \frac{1}{3}x^3 \ln x - \int \frac{1}{3}x^3 \cdot \frac{1}{x} dx\\
&= \frac{1}{3}x^3 \ln x - \frac{1}{9}x^3 + C\\
y(1) &= 2 \To C = \frac{19}{9}\\
y &= \frac{1}{3}x^3 \ln x - \frac{1}{9}x^3 + \frac{19}{9}\\
\end{aligned}
$$

42-43\. Solve the given _boundary-value problem_.
43\. $y'' = -2(3 + 2\ln x)$, $y(1) = y(e) = 0$
>Solution
$$
\begin{aligned}
y' &= \int -2(3 + 2\ln x) dx\\
&= -2x - 4x\ln x + c_1\\
y &= \int (-2x - 4x\ln x + c_1) dx\\
&= -2x^2\ln x + c_1 x + c_2\\
y(1) &= y(e) = 0\\
\To c_1 &= \frac{2e^2}{e-1}, c_2 = \frac{-2e^2}{e-1}\\
y &= -2x^2\ln x + \frac{2e^2}{e-1} x - \frac{2e^2}{e-1}
\end{aligned}
$$
