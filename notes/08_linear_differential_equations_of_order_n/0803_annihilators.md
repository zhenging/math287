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
& \text{DE:} D^3 y = 0
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
& \text{DE:} (D-3) y = 0
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
& \text{DE:} (D+5)^3 y = 0
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
& \text{DE:} (D^2 - 2aD + a^2 + b^2) y = 0
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
