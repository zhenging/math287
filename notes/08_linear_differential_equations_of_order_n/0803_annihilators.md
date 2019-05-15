### 0803 Annihilators
$D^2$ annihilates $12x + 1$.
$D^2 (12x + 1) = DD(12x + 1) = D(12) = 0$
$D^5$ also annihilates $12x + 1$.
$D^2$ is called the **annihilator** of $12x + 1$ because it's the lowest order operatpr that does the job.

**1\. What annihilates $p_2$, a polynomial of degree 2?**
$$
\begin{aligned}
y &= c_1 + c_2 x+ c_3 x^2\\
& = c_1 e^{0x} + c_2 xe^{0x} + c_3 x^2 e^{0x}\\
r &= 0, 0, 0\\
& \text{auxiliary equation:} r^3 = 0\\
& \text{DE: } D^3 y = 0
\end{aligned}
$$

$p_2$ is annihilated by $D^3$.
$p_n$ is annihilated by $D^{n+1}$.

**2\. What annihilates $e^{3x}$?**
$$
\begin{aligned}
y &= c e^{3x}\\
r &= 3\\
& \text{auxiliary equation:} r - 3 = 0\\
& \text{DE: } (D-3) y = 0
\end{aligned}
$$
$c e^{3x}$ is annihilated by $D-3$.
$c e^{ax}$ is annihilated by $D-a$.

**3\. What annihilates $p_2 e^{-5x}$?**
$$
\begin{aligned}
y &= (c_1 + c_2 x+ c_3 x^2) e^{-5x}\\
& = c_1 e^{-5x} + c_2 xe^{-5x} + c_3 x^2 e^{-5x}\\
r &= -5, -5, -5\\
& \text{auxiliary equation:} (r + 5)^3 = 0\\
& \text{DE: } (D+5)^3 y = 0
\end{aligned}
$$
$p_2 e^{-5x}$ is annihilated by $(D+5)^3$.
$p_n e^{ax}$ is annihilated by $(D-a)^{n+1}$.

**4\. What annihilates $c_1 e^{ax}\cos bx + c_2 e^{ax}\sin bx$**?
$$
\begin{aligned}
y &= c_1 e^{ax}\cos bx + c_2 e^{ax}\sin bx\\
&= e^{ax} (c_1 \cos bx + c_2 \sin bx)\\
r &= a \pm bi\\
& \text{auxiliary equation:} (r - (a+bi)) ((r - (a-bi))) = 0\\
& r^2 - 2ar + a^2 + b^2 = 0\\
& \text{DE: } (D^2 - 2aD + a^2 + b^2) y = 0
\end{aligned}
$$
$c_1 e^{ax}\cos bx + c_2 e^{ax}\sin bx$ is annihilated by $D^2 - 2aD + a^2 + b^2$.

Function | Annihilator
---------|-----------
1\. $p_n$ | $D^{n+1}$
2\. $c e^{ax}$  | $D-a$
3\. $p_n e^{ax}$ | $(D-a)^{n+1}$
4\. $c_1 e^{ax}\cos bx + c_2 e^{ax}\sin bx$ | $D^2 - 2aD + a^2 + b^2$
5\. $c_1 \cos bx + c_2 \sin bx$ | $D^2 + b^2$
6\. $p_n e^{ax} \cos bx + q_n e^{ax} \sin bx$ | $(D^2 - 2aD + a^2 + b^2)^{n+1}$
7\. sum | product of annihilators

##### Homework
8.3 p.525 1-45 odd

1-15\. Determine the annihilator of the given functions.
5\.$F(x) = 4 e^{-2x} \sin x$
>Solution
$$
\begin{aligned}
F(x) &= p_n e^{ax}\cos bx + q_n e^{ax}\sin bx\\
&= 0 \cdot e^{-2x} \cos (1x) + 4 \cdot e^{-2x} \sin (1x)\\
p_n &= 0, q_n = 4, n = 0, a = -2, b = 1\\
A(D) &= (D^2 - 2aD + a^2 + b^2)^{n+1}\\
&= D^2 - 2\times (- 2) D + (-2)^2 + 1^2\\
&= D^2 + 4D + 5
\end{aligned}
$$

7\. $F(x) = (1-3x)e^{4x} + 2x^2$
>Solution
$$
\begin{aligned}
F(x) &= p_n e^{ax} + q_m\\
p_n& = 1-3x, n = 1, a = 4, q_m = 2x^2, m=2\\
A(D) &= (D-4)^2 D^3
\end{aligned}
$$

17-31\. Determine the general solution to the given differential equation. Derive your trail solution to using the annihilator technique.
17\. $(D-1)(D + 2) y = 5e^{3x}$
>Solution
1\. The auxiliary polynomial is $P(r) = (r-1)(r+2)$, so the complementary solution
$$
\begin{aligned}
y_c = c_1 e^x + c_2 e^{-2x}
\end{aligned}
$$
2\. $F(x) = 5e^{3x}$. Its annihilator is $A(D) = D - 3$. Operating on the given differential equation with $A(D)$ yields the homogeneous differential equation
$$
\begin{aligned}
(D-3)(D-1)(D + 2) y = 0
\end{aligned}
$$
with general solution
$$
\begin{aligned}
y(x) = c_1 e^x + c_2 e^{-2x} + A_0 e^{3x}
\end{aligned}
$$
3\. An appropriate trail solution is $y_p(x) = A_0 e^{3x}$. Differentiating $y_p$ twice yields
$$
\begin{aligned}
y'_p = 3 A_0 e^{3x}, y''_p = 9 A_0 e^{3x}
\end{aligned}
$$
4\. Substitue $y_p$ back to the original equation
$$
\begin{aligned}
(D-1)(D + 2) y &= 5e^{3x}\\
D^2 + D - 2) y &= 5e^{3x}\\
9 A_0 e^{3x} + 3 A_0 e^{3x} -2 A_0 e^{3x} &= 5e^{3x}\\
10 A_0 e^{3x} & = 5 e^{3x}\\
\To A_0 &= \frac{1}{2}
\end{aligned}
$$
Consequently, a particular solution $y_p(x) = \frac{1}{2} e^{3x}$.
5\. The general solution is
$$
\begin{aligned}
y(x) = c_1 e^x + c_2 e^{-2x} + \frac{1}{2} e^{3x}
\end{aligned}
$$
