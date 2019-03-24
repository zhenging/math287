### 7.2 Eigenspace and Nondefective Matrices

Let $A$ be $n\times n$ matrices.

**Eigenspace**
Let $\lm$ be an eigenvalue of $A$. The set of all eigenvectors of $\lm$, together with the zero vector, is a subspect of $\R^n$. We call this subspace the **eigenspace** of $\lm$.

**Algebraic Multiplicity and Geometric Multiplicity**
Let $\lm$ be an eigenvalue of $A$. The multiplicity of $\lm$ in the characteristic polynomial is called the **algebraic multiplicity** of $\lm$, The dimension of the eigenspace corresponding to $\lm$ is called the **geometric multiplicity** of $\lm$.

**Defective/Nondefective**
+ Let $A$ has $n$ linearly independent eigenvectors, then $A$ is called **nondefective**. Otherwise, $A$ is called **defective**.
+ If the algebraic multiplicity equals the geometric multiplicity for each eigenvalue of $A$, then $A$ is **nondefective**. Otherwise,$A$ is **defective**.

#### Homework
p.451 1-15 odd
1-15\. Determine the multiplicity of each eigenvalue and a basis for each eigenspace of the given matrix $A$. Hence determine the dimension of each eigenspace and state whether the matrix is defective of nondefective.
2\. $A = \begin{bmatrix}
-7 & 0\\
-3 & -7
\end{bmatrix}$
>Solution
$$
\begin{aligned}
A-\lm I &= \begin{bmatrix}
-7-\lm & 0\\
-3 & -7-\lm
\end{bmatrix}\\[1em]
det(A-\lm I) &= (\lm+7)(\lm+7) -0 = 0\\
\To \lm_1 &=  \lm_2 = -7
\end{aligned}
$$
**For eigenvalue $\lm = -7$** (with algebraic multiplicity 2), the eigenvectors are determined by solving the linear system $(A-\lm I) v = 0$. The agumented matrix for the system is
$$
\begin{aligned}
\begin{array}{cc|c}
-7-(-7) & 0 & 0\\
-3 & -7-(-7) & 0
\end{array}
\sim
\begin{array}{cc|c}
1 & 0 & 0\\
0 & 0 & 0
\end{array}
\end{aligned}
$$
1\. The general solution to this system is therefore
$$
\begin{aligned}
v= t(0, 1), t\ne 0
\end{aligned}
$$
2\. Eigenspace
$$
\begin{aligned}
E &= \{v\in \R^2: v=t(0, 1), t\ne 0\}\\
&=\text{span}\{(0, 1)\}
\end{aligned}
$$
3\. The basis of the eigenspace is $\{(0, 1)\}$, and the dimension is 1.
4\. The matrix is defective.

5\. $A = \begin{bmatrix}
5 & 5\\
-2 & -1
\end{bmatrix}$
>Solution
$$
\begin{aligned}
A-\lm I &= \begin{bmatrix}
5-\lm & 5\\
-2 & -1-\lm
\end{bmatrix}\\[1em]
det(A-\lm I) &= (\lm-5)(\lm+1) - (-10) = 0\\
&=\lm^2 - 4\lm + 5 = 0\\
\To \lm_1 &= 2+i, \lm_2 = 2-i
\end{aligned}
$$
**For egigenvalue $\lm_1 = 2+i$** (AM=1), the eigenvectors are determined by solving the lineary system, $(A-\lm_1 I) v_1 = 0$. The agumented matrix for the system is
$$
\begin{array}{cc|c}
5-(2+i) & 5 & 0\\
-2 & -1-(2+i) & 0
\end{array}
\sim
\begin{array}{cc|c}
2 & 3+i & 0\\
0 & 0 & 0
\end{array}
$$
1\. The general solution to this system is therefore
$$
v_1 = t(-3-i, 2), t\ne 0
$$
2\. Eigenspace
$$
\begin{aligned}
E_1 &= \{v\in \Complex^2: v= t(-3-i, 2), t\ne 0\}\\
&=\text{span}\{(-3-i, 2)\}
\end{aligned}
$$
3\. The basis of the eigenspace is $\{(-3-i, 2)\}$, and the dimension is 1.
For egigenvalue $\lm_2 = 2-i$ (AM=1), we have
1\. Eigenvectors $v_2 = t(-3+i, 2), t\ne 0$,
2\. Eigenspace $E_2=\text{span}\{(-3+i, 2)\}$.
3\. Basis of the eigenspace is $\{(-3+i, 2)\}$.
The matrix is **nondefective**.

9\. $A = \begin{bmatrix}
3 & 0 & 0\\
2 & 0 & -4\\
1 & 4 & 0
\end{bmatrix}$
>Solution
$$
\begin{aligned}
A-\lm I &= \begin{bmatrix}
3-\lm & 0 & 0\\
2 & -\lm & -4\\
1 & 4 & -\lm
\end{bmatrix}\\[1em]
det(A-\lm I) &= (\lm-3)(\lm^2+16) = 0\\
\To \lm_1 &= 3, \lm_2 = 4i, \lm_3 = -4i
\end{aligned}
$$
**For egigenvalue $\lm_1 = 3$** (AM=1), the eigenvectors are determined by solving the lineary system, $(A-\lm_1 I) v_1 = 0$. The agumented matrix for the system is
$$
\begin{array}{ccc|c}
0 & 0 & 0 & 0\\
2 & -3 & -4 & 0\\
1 & 4 & -3 & 0
\end{array}
\sim
\begin{array}{ccc|c}
1 & 4 & -3 & 0\\
0 & 11 & -2 & 0\\
0 & 0 & 0 & 0
\end{array}
$$
1\. The general solution to this system is therefore
$$
v_1 = t(25, 2, 11), t\ne 0
$$
2\. Eigenspace
$$
\begin{aligned}
E_1 &= \{v\in \R^2: v= t(25, 2, 11), t\ne 0\}\\
&=\text{span}\{(25, 2, 11)\}
\end{aligned}
$$
3\. The basis of the eigenspace is $\{(25, 2, 11)\}$, and the dimension is 1.
**For egigenvalue $\lm_2 = 4i$** (AM=1), we have
1\. Eigenvectors
$$
\begin{aligned}
&\begin{array}{ccc|c}
3-4i & 0 & 0 & 0\\
2 & -4i & -4 & 0\\
1 & 4 & -4i & 0
\end{array}
\sim
\begin{array}{ccc|c}
1 & 0 & 0 & 0\\
0 & 1 & -i & 0\\
0 & 0 & 0 & 0
\end{array}\\[1.0em]
&\To v_2 = t(0, i, 1), t\ne 0
\end{aligned}
$$
2\. Eigenspace $E_2=\text{span}\{(0, i, 1)\}$.
3\. Basis of the eigenspace is $\{(0, i, 1)\}$.
**For egigenvalue $\lm_3 = -4i$** (AM=1), we have
1\. Eigenvectors $v_3 = t(0, -i, 1), t\ne 0$.
2\. Eigenspace $E_3=\text{span}\{(0, -i, 1)\}$.
3\. Basis of the eigenspace is $\{(0, -i, 1)\}$.
The matrix is **nondefective**.
