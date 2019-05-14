### 0901 First-Order Linear System

A system of differential equations of the form
$$
\begin{aligned}
\frac{dx_1}{dt} &= a_{11}(t)x_1(t)+a_{12}(t)x_2(t)+\cdots + a_{1n}(t)x_n(t)+ b_1(t)\\
\frac{dx_2}{dt} &= a_{21}(t)x_1(t)+a_{22}(t)x_2(t)+\cdots + a_{2n}(t)x_n(t)+ b_1(t)\\
\cdots\\
\frac{dx_n}{dt} &= a_{n1}(t)x_1(t)+a_{n2}(t)x_2(t)+\cdots + a_{nn}(t)x_n(t)+ b_n(t)\\
\end{aligned}
$$
where the $a_{ij}(t)$ and $b_i(t)$ are specified functions on the interval $I$, is called first-order\ linear system. If $b_1 = b_2 \cdots = b_n = 0$, then the system is called **homogeneous**. Otherwise it is called **none homogeneous.**
+ The highest derivative is a first derivative.\
+ There is precisely one equation involving the derivative of each seperate unknown functions.
+ The terms that appear on the right-hand side of the equation do not involve any derivatives and are linear in unknown functions $x_1, x_2, \cdots, x_n$


#### Homework
9.1 p.587 1-6 all, 9, 10, 12, 13, 15-19 all

12-13\. Solve the given nonehomogeneous system
12\. $x_1' = x_1 + 2x_2 + 5e^{4t}$, $x_2' = 2x_1 + x_2$
>Solution
$$
\begin{aligned}
&\begin{alignedat}{1}
&x_1' = x_1 + 2x_2 + 5e^{4t}\\
&x_2' = 2x_1 + x_2
\end{alignedat}\\
&\To \begin{cases}
(D-1) x_1 &- 2x_2 &= 5e^{4t}\\
(D-1) x_2 &- 2x_1 &= 0
\end{cases}\\[1.25em]
&\To \begin{cases}
2(D-1) x_1 &- 4x_2 &= 10e^{4t}\\
(D-1)^2 x_2 &- 2(D-1)x_1 &= 0
\end{cases}\\[1.25em]
&\To (D-1)^2 x_2 - 4x_2 = 10e^{4t}\\
&\To (D^2-2D - 3) x_2 = 10e^{4t}\\
&\To (D-3)(D+1) x_2 = 10e^{4t}
\end{aligned}
$$
The auxiliary polynomial is $P(r) = (r-3)(r+1)$, so that the complentary function for $x_2$ is
$$
\begin{aligned}
x_{2c} = c_1 e^{3t} + c_2 e^{-t}
\end{aligned}
$$
Let $F(x) = 10e^{4t}$, the annihilator is $A(D) = D-4$. Operating on the differential equation yields the homogeneous differential equation.
$$
\begin{aligned}
&(D-4)(D-3)(D+1) x_2 = 0\\
&\To \text{general solution for } x_2\\
& x_2 = A e^{4t} + c_1 e^{3t} + c_2 e^{-t}
\end{aligned}
$$
An appropriate trail solution for $x_2$ is $x_{2p} = A e^{4t}$.
$$
\begin{aligned}
& x_{2p}' = 4A e^{4t}\\
& x_{2p}''= 16A e^{4t}\\
& 16A e^{4t} - 2 \times 4A e^{4t} - 3 A e^{4t} =  10 e^{4t}\\
&\To A = 2
\end{aligned}
$$
Hence,
$$
\begin{aligned}
x_1 &= c_1 e^{3t} - c_2 e^{-t} + 3 e^{4t}\\
x_2 &= c_1 e^{3t} + c_2 e^{-t} + 2 e^{4t}
\end{aligned}
$$

15-19\. Convert the given system of differential equations to a first-order linear system.
16\. $\d \frac{d^2 x}{d t^2} - 3 \frac{d x}{d t} + x = \sin t$, $\d \frac{d^2 y}{d t^2} - t \frac{d x}{d t} - e^ty = t^2$
>Solution
Let $x_1 = x, x_2 = x_1', x_3 = y, x_4 = y'$
$$
\begin{aligned}
x_1' &= x_2\\
x_2' & =  - x_1 + 3x_2 + \sin t\\
x_3' &= x_4\\
x_4' &= tx_2 + e^t x_3 + t^2
\end{aligned}
$$

18\. $y'' + ay' + by = F(t)$, $a, b$ are constants.
>Solution
Let $x_1 = y, x_2 = y''$
$$
\begin{aligned}
x_1' &= x_2\\
x_2' &= - bx_1 - ax_2 + F(t)
\end{aligned}
$$
