### 7.1 The Eigenvalue/Eigenvector Problem

#### Definition
Let $A$ be $m\times n$ matrix. Any values of $\lm$ for which $Av = \lm v$ has _nontrival_ solutions $v$ are called **eigenvalues** of $A$. The corresponding vectors $v$ are called **eigenvectors** of $A$. (also refered as **characteristic** value and **characteristic** vectors).

#### Homework
p.443 1-7 all, 13-31 odd, 35

4\. Verity eigenvalue/eigenvector pair. $\lm=-2$ and $v = c_1(1, 0, -3) + c_2(4, -3, 0)$
$$
A = \begin{bmatrix}
1 & 4 & 1\\
3 & 2 & 1\\
3 & 4 & -1
\end{bmatrix}
$$
>Solution
$$
\begin{aligned}
Av = \begin{bmatrix}
1 & 4 & 1 \\
3 & 2 & 1 \\
3 & 4 & -1
\end{bmatrix}
\begin{bmatrix}
c_1+4c_2\\
-3c_2\\
-3c_1
\end{bmatrix}
=\begin{bmatrix}
-2c_1-8c_2\\
6c_2\\
6c_1
\end{bmatrix}
=\lm v
\end{aligned}
$$

6\. Given that $v_1=(-2,1)$ and $v_2=(1, 1)$ are eigenvectors of
$$
A = \begin{bmatrix}
-5 & 2\\
1 & -4
\end{bmatrix}
$$
>Solution
$$
\begin{aligned}
Av_1 &= \begin{bmatrix}
-5 & 2\\
1 & -4
\end{bmatrix}
\begin{bmatrix}
-2\\
1
\end{bmatrix}
= \begin{bmatrix}
12\\
-6
\end{bmatrix}
= -6v_1\\
\To \lm_1 &= -6\\
Av_2 &= \begin{bmatrix}
-5 & 2\\
1 & -4
\end{bmatrix}
\begin{bmatrix}
1\\
1
\end{bmatrix}
= \begin{bmatrix}
-3\\
-3
\end{bmatrix}
= -3v_2\\
\To \lm_2 &= -3
\end{aligned}
$$

13-31\. Determine all eigenvalues and corresponding eigenvectors
14\. $A = \begin{bmatrix}
7 & 4\\
-1 & 3
\end{bmatrix}$
>Solution
$$
\begin{aligned}
A-\lm I &= \begin{bmatrix}
7-\lm & 4\\
-1 & 3-\lm
\end{bmatrix}\\
det(A-\lm I) &= (\lm-7)(\lm-3) = 0\\[1.2em]
\To \lm_1 &= 7, \lm_2 = 3\\[1.2em]
\lm_1=7 \To &v_1 = \begin{bmatrix}
0 & 4\\
-1 & -4
\end{bmatrix}\\
\lm_2=3 \To &v_2 = \begin{bmatrix}
4 & 4\\
-1 & 0
\end{bmatrix}\\
\end{aligned}
$$

35\. Let $A = \begin{bmatrix}
1 & 2\\
2 & -2
\end{bmatrix}$.
a. Determine all eigenvalues of $A$.
b. Reduce A to row-echon form, and determine the eigenvalues of the resulting matrix. Are these the same as the eigenvalues of $A$?
>Solution
$$
\begin{aligned}
det(A-\lm I) &= (\lm-1)(\lm+2) - 4 = 0\\
&=(\lm+3)(\lm-2)\\
\To \lm_1 &= 3, \lm_2= 2\\[1.2em]
A = \begin{bmatrix}
1 & 2\\
2 & -2
\end{bmatrix}&
\sim
\begin{bmatrix}
1 & 2\\
0 & 1
\end{bmatrix}=B\\[1.2em]
det(B-\lm I) &= (\lm-1)(\lm-1) - 0 = 0\\
\To \lm_1 &= \lm_2= 1\\
\end{aligned}
$$
