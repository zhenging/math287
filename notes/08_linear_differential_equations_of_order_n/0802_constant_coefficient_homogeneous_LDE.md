### 0802 Constant Coefficient Homogeneous Linear Differential Equation

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
