### 1001  Definition of the Laplace Transform
Let $f$ be a function on the interval $[0, \infty]$. The **Laplace Transform** of $f$ isnthe function $F$ defined by
$$
\begin{aligned}
\tag{10.1.1} F(s) &= \int_0^{\infty} e^{-st}f(t)dt\\
&= \lim_{N\to \infty}\int_0^N e^{-st}f(t)dt\\
\end{aligned}
$$
This improper integral converges if and only if the limit on the right hand side exists and is finite. It follows that not all function definedd on $[0, \infty]$ have a **Laplace Transform**.

#### Example 10.1.2
Determine the Laplace transform for the following functions.
a. $f(t) = 1$
b. $f(t) = t$
c. $f(t) = e^{at}$
d. $f(t) = \cos {bt}$
>Solution
a. From the foregoing definition, we have
$$
\begin{aligned}
L[1] = \int_0^{\infty} (e^{-st} \cdot 1) dt &= \lim_{N \to \infty} \bigg[ -\frac{1}{s} e^{-st}\bigg]_0^N\\
&= \lim_{N \to \infty} \bigg[ -\frac{1}{s} e^{-sN} + \frac{1}{s} e^0\bigg]\\
&= \lim_{N \to \infty} \bigg[ -\frac{1}{s} e^{-sN}\bigg]+ \lim_{N \to \infty} \bigg[ \frac{1}{s} e^0\bigg]\\
&= 0 + \frac{1}{s} = \frac{1}{s}
\end{aligned}
$$
b. In this case, we use integration by parts to obtain
$$
\begin{aligned}
L[t] = \int_0^{\infty} (e^{-st} \cdot t) dt &= \lim_{N \to \infty} \bigg[ -\frac{t}{s}e^{-st} -\frac{1}{s^2} e^{-st}\bigg]_0^N\\
&= \lim_{N \to \infty} \bigg[ -\frac{t}{s}e^{-st}\bigg]_0^N + \lim_{N \to \infty} \bigg[-\frac{1}{s^2} e^{-st}\bigg]_0^N\\
&= \lim_{N \to \infty} \bigg[ -\frac{N}{s}e^{-sN} - 0\bigg] + \frac{1}{s^2}\\
&= 0 + \frac{1}{s^2}
\end{aligned}
$$
Note, $\dlim_{N \to \infty}Ne^{-st} = 0, s > 0$ (L'Hopital's Rule).
c\. In this case, we have
$$
\begin{aligned}
L[1] = \int_0^{\infty} (e^{-st} \cdot e^{at}) dt &= \int_0^{\infty} (e^{(a-s)t}dt\\
&= \lim_{N \to \infty} \bigg[ \frac{1}{a-s} e^{(a-s)t}\bigg]_0^N\\
&= 0-\frac{1}{a-s} = \frac{1}{s-a}, (s>a)
\end{aligned}
$$
d\. From the definition, we have
$$
\begin{aligned}
L[\cos {bt}] = \int_0^{\infty} (e^{-st} \cdot \cos {bt}) dt
\end{aligned}
$$
Use the standard integral
$$
\begin{aligned}
\int (e^{-st} \cos {bt}) dt &= \frac{e^{at}}{a^2 + b^2}(a\cos {bt} + b \sin {bt}) + c
\end{aligned}
$$
It follows that
$$
\begin{aligned}
L[\cos {bt}] &= \lim_{N \to \infty} \bigg[ \frac{e^{-st}}{(-s)^2 + b^2}(-s\cos {bt} + b \sin {bt})\bigg]_0^N\\
&= \frac{s}{s^2 + b^2}
\end{aligned}
$$
provided $s>0$. Thus
$$
\begin{aligned}
L[\cos {bt}] = &= \frac{s}{s^2 + b^2}, \qquad s>0
\end{aligned}
$$
Similarly, it can be show that
$$
\begin{aligned}
L[\sin {bt}] = &= \frac{b}{s^2 + b^2}, \qquad s>0
\end{aligned}
$$

#### Linearity of the Laplace Transform
The Lapace satifies the basic properties of a linear transformation.
$$
\begin{aligned}
L[f+g] &= L[f] +L[g]\\
L[cf] &= cL[f]
\end{aligned}
$$
Proof:
$$
\begin{aligned}
L[f+g] &= \int_0^{\infty} e^{-st}[f(t) + g(t)]dt\\
&= \int_0^{\infty} e^{-st}f(t)dt + \int_0^{\infty} e^{-st}g(t)dt\\
&= L[f] + L[g]
\end{aligned}
$$
Further, if $c$ is any real number, then
$$
\begin{aligned}
L[cf] &= \int_0^{\infty} e^{-st} cf(t) dt\\
&= c \int_0^{\infty} e^{-st} f(t) dt\\
&= cL[f]
\end{aligned}
$$

#### Piecewise Continuous Functions
A function $f$ is called **piecewise continuous** on the interval $[a, b]$ if we can divide $[a,b]$ into a finite number of subinterval in such a manner that
1\. $f$ is continuous on each subinterval, and
2\. $f$ approaches a finite limit as the endpoints of each subinterval are approached from within.
If $f$ is piecewise continuous on every interval of the form $[0, b]$, where $b$ is a constant, then we say that f is piecewise continuous on $[0, \infty]$


#### Homework
10.1A p.675 1, 3, 4, 7-11 odd, 31-34 all
10.1B p.675 13, 14, 17, 18, 20, 21
