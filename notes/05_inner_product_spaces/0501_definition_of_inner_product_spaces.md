### 5.1 Definition of Inner Product Spaces

#### Standard Inner Product
Let $x = (x_1, x_2, \cdots x_n)$ and $y = (y_1, y_2, \cdots y_n)$ be vectors in $\R^n$. We define **the standard inner product** in $\R^n$, denoted $\la x, y\ra$ by
$$
\begin{aligned}
\la x, y\ra = x_1y_1 + x_2y_2 + \cdots + x_ny_n
\end{aligned}
$$
The **norm** of $x$ is
$$
\begin{aligned}
||x|| = \sqrt{\la x, x\ra} = \sqrt{x_1^2 + x_2^2 + \cdots + x_n^2}
\end{aligned}
$$

##### Properties
Let **u, v**, and **w** be vectors in **V**. Let $r$ be a scalar in **F**.
1\. $\la u, u\ra \ge 0$ and $\la u, u\ra = 0$ **iff** $u=0$
2\. $\la u, v \ra = \la v, u\ra$
3\. $r\la u, v \ra = \la ru, v\ra$
4\. $\la u+v, w \ra = \la u, w \ra + \la v, w\ra$

##### Example 5.1.2
If $x = (-2, 0, 4, 1, -2, 0)$ and $y = (5, -1, -1, 6, -3, 3)$ in $\R^6$, then
$$
\begin{aligned}
\la x, y\ra &= (-2)(5) + (0)(-1) + (4)(-1) + (1)(6) + (-2)(-3) + (-0)(3) = -2\\
||x|| &= \sqrt{(-2)^2 + 0^2 + 4^2 + 1^2 + (-2)^2 + 0^2} = 5\\
||y|| &= \sqrt{5^2 + (-1)^2 + (-1)^2 + 6^2 + (-3)^2 + 3^2} = 9
\end{aligned}
$$

#### Function Inner Product
In the vector space $C^0[a, b]$ of all real-valued functions that are continuous on the interval $[a, b]$, we define the mapping $\la f, g\ra$ by
$$
\begin{aligned}
\la f, g\ra &= \int_a^b f(x)g(x) dx
\end{aligned}
$$

#### Angle between two nonzero vectors
$$
\begin{aligned}
\cos\th &= \frac{\la v, w\ra}{||v|| ||w||}
\end{aligned}
$$

#### Homework
p.350 1-4, 12, 13, 19-21
1\. Use the standard inner product in $\R^5$ to determine the angle between the vectors $v = (0, -2, 1, 4, 1)$ and $w = (-3, 1, -1, 0, 3)$.
>Solution
$$
\begin{aligned}
\la v, w\ra &= 0(-3) + (-2)1 + 1(-1) + 4(0) + 1(3) = 0\\
||v|| &= \sqrt{0^2 + (-2)^2 + 1^2 + 4^2 + 1^2} = \sqrt{22}\\
||w|| &= \sqrt{(-3)^2 + 1^2 + (-1)^2 + 0^2 + 3^2} = 2\sqrt{5}\\
\cos\th &= \frac{\la v, w\ra}{||v|| ||w||}\\
&= 0\\
\To \th = \pi/2
\end{aligned}
$$

4\. If $f(x) = \sin x$ and $g(x) = 2\cos x + 4$ on $[0, \pi/2]$, use the function inner product (5.1.5) to determine the angle between $f$ and $g$.
>Solution
$$
\begin{aligned}
\la f, g\ra &= \int_a^b f(x)g(x) dx\\
&= \int_0^{\pi/2} \sin x(2\cos x + 4) dx\\
&= (\frac{-\cos 2x}{2}-4\cos x)|_0^{\pi/2} = 5\\
\la f, f\ra &= \int_a^b f(x)^2 dx\\
&= \int_0^{\pi/2} \sin^2 x dx\\
&= \int_0^{\pi/2} (\frac{1-\cos (2x)}{2})dx\\
&= (\frac{x}{2} - \frac{\sin (2x)}{4})_0^{\pi/2} = \frac{\pi}{4}\\
\la g, g\ra &= \int_a^b g(x)^2 dx\\
&= \int_0^{\pi/2} (2\cos x + 4)^2 dx\\
&= \int_0^{\pi/2} (2\cos(2x)+16\cos x + 18)dx\\
&= (\sin(2x) + 16\sin x + 18x)|_0^{\pi/2} = 9\pi + 16\\
\cos \th &= \frac{\la f, g\ra}{||f|| ||g||}\\
&=\frac{5}{\sqrt{\frac{\pi}{4}} \times \sqrt{(9\pi + 16)}} = 0.85\\
\To \th &= 32\degree
\end{aligned}
$$

20\. Consider the vector space $\R^2$. Define the mapping $\la , \ra$ by
$$
\begin{aligned}
\tag{5.1.14} \la v, w\ra = 2v_1w_1+v_1w_2+v_2w_1+2v_2w_2
\end{aligned}
$$
For $v = (2, -1)$ and $w = (3, 6)$, determine the inner product of given vectors using (a) the inner product (5.1.14) and (b) the standard inner product in $\R^2$.
>Solution
a. $\la v, w\ra = 2(2)(3) + 2(6) + (-1)3 + 2(-1)(6) = 9$
b. $\la v, w\ra = (2)(3) + (-1)6  = 0$
