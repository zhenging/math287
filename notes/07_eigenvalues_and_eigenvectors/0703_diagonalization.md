### 7.3 Diagonalization

Let $A$ and $B$ be $n\times n$ matrices.

If $A$ is **triangular**, then its eigenvalues are the entries on its main diagonal.

**Similar**
+ $A$ is **similar** to $B$ if there exist an invertible matrix $S$ such that $B=S^{-1}AS$.
+ If $A$ and $B$ are similar, then they have the same eigenvalues (including multiplicity).

**Proof** if $A$ is **similar** to $B$, then $B = S^{-1}AS$ for some invertible matrix $S$. Thus
$$
\begin{aligned}
det(B-\lm I) &= det(S^{-1}AS -\lm I)\\
&= det(S^{-1}AS -\lm S^{-1} S)\\
&= det[S^{-1}(A -\lm I) S]\\
&= det(S^{-1})det(A -\lm I) det(S)\\
&= det(A -\lm I)
\end{aligned}
$$
where we have used the face that $det(S^{-1}) = \dfrac{1}{det(S)}$ in the final step. Consequently $A$ and $B$ have the same characteristic polynomial and hence the same eigenvalues (and multiplicities).

**Diagonalizable**
+ If $A$ is similar to a diagonal matrix, then $A$ is **diagonalizable**.
+ A is diagonalizable **iff** $A$ is nondefective.

#### Examples
Let $A$ be a $2\times 2$ nondefective matrix. $A$ has one eigenvalue $\lm_1 = 1$ with corresponding eigenvectors $v_1 = t(1, 5)$, and another eigenvalue $\lm_2=7$ with corresponding eigenvectors $v_2 = t(-1, 1)$. Find $A$.
>Solution
$A$ is nondefective. Thus, there exists a diagonal matrix $D$ and a matrix $S$ such that $D = S^{-1} A S$
$$
\begin{aligned}
D &= \begin{bmatrix}
1 & 0\\
0 & 7
\end{bmatrix}\\
S &= \begin{bmatrix}
1 & -1\\
5 & 1
\end{bmatrix}\\
S^{-1} &= \frac{1}{6}\begin{bmatrix}
1 & 1\\
-5 & 1
\end{bmatrix}\\
D &= S^{-1} A S\\
\To A&= S D S^{-1}\\
&= \begin{bmatrix}
1 & -1\\
5 & 1
\end{bmatrix}
\begin{bmatrix}
1 & 0\\
0 & 7
\end{bmatrix}
\frac{1}{6}\begin{bmatrix}
1 & 1\\
-5 & 1
\end{bmatrix}\\
&= \begin{bmatrix}
6 & -1\\
-5 & 2
\end{bmatrix}
\end{aligned}
$$

#### Homework
p.459 1-13 odd

1-13\. Determine whether the given matrix $A$ is diagonalizable. When possible, find a matrix $S$ such that
$$
\begin{aligned}
S^{-1} A S = diag(\lm_1, \lm_2, \cdots \lm_n)
\end{aligned}
$$
1\. $A = \begin{bmatrix}
-9 & 0\\
4 & -9
\end{bmatrix}$
>Solution
$$
\begin{aligned}
A-\lm I &= \begin{bmatrix}
-9-\lm & 0\\
4 & -9-\lm
\end{bmatrix}\\[1em]
det(A-\lm I) &= (\lm+9)(\lm+9) - 0 = 0\\
\To \lm_1 &= \lm_2 = -9
\end{aligned}
$$
**For eigenvalue $\lm = -9$**(**Algebraic multiplicity is 2**), the eigenvectors are determined by solving the linear system $(A-\lm I) v = 0$. The agumented matrix for the system is
$$
\begin{aligned}
&\begin{array}{cc|c}
-9-(-9) & 0 & 0\\
4 & -9-(-9) & 0
\end{array}
\sim
\begin{array}{cc|c}
1 & 0 & 0\\
0 & 0 & 0
\end{array}\\
&\To v= t(0, 1), t\ne 0
\end{aligned}
$$
The eigenspace is $E = \text{span}\{(0, 1)\}$. The basis of the eigenspace is $\{(0, 1)\}$. (**Geometric multiplicity is 1**).
Algebraic multiplicity $\ne$ Geometric multiplicity. Thus the matrix is **defective** and **not diagonalizable**.

5\. $A = \begin{bmatrix}
0 & 4\\
-4 & 0
\end{bmatrix}$
>Solution
$$
\begin{aligned}
A-\lm I &= \begin{bmatrix}
-\lm & 4\\
-4 & -\lm
\end{bmatrix}\\[1em]
det(A-\lm I) &= \lm^2 + 16= 0\\
\To \lm_1 &= 4i, \lm_2 = -4i
\end{aligned}
$$
**For eigenvalue $\lm_1 = 4i$**, the eigenvectors
$$
\begin{aligned}
&\begin{array}{cc|c}
-4i & 4 & 0\\
-4 & -4i & 0
\end{array}
\sim
\begin{array}{cc|c}
1 & i & 0\\
0 & 0 & 0
\end{array}\\
&\To v_1= t(-i, 1), t\ne 0
\end{aligned}
$$
**For eigenvalue $\lm_2 = -4i$**, the eigenvectors
$$
\begin{aligned}
&\begin{array}{cc|c}
4i & 4 & 0\\
-4 & 4i & 0
\end{array}
\sim
\begin{array}{cc|c}
1 & -i & 0\\
0 & 0 & 0
\end{array}\\
&\To v_2= t(i, 1), t\ne 0
\end{aligned}
$$
$v_1$ and $v_2$ are linearly independent eigenvectors of $A$. Let $S = [v_1, v_2]$,
$$
\begin{aligned}
S &= \begin{bmatrix}
-i & i\\
1 & 1
\end{bmatrix}\\[1.0em]
S^{-1} A S &= \text{diag}(\lm_1, \lm_2)\\
&= \text{diag}(4i, -4i)\\
\end{aligned}
$$

11\. $A = \begin{bmatrix}
4 & 0 & 0\\
3 & -1 & -1\\
4 & 2 & 1
\end{bmatrix}$
>Solution
$$
\begin{aligned}
A-\lm I &= \begin{bmatrix}
4-\lm & 0 & 0\\
3 & -1-\lm & -1\\
4 & 2 & 1-\lm
\end{bmatrix}\\[1em]
det(A-\lm I) &= (4-\lm)[\lm^2+1]= 0\\
\To \lm_1 &= 4, \lm_2 = i, \lm_3=-i
\end{aligned}
$$
**For eigenvalue $\lm_1 = 4$**, the eigenvectors
$$
\begin{aligned}
&\begin{array}{ccc|c}
0 & 0 & 0 & 0\\
3 & -5 & -1 & 0\\
0 & 2 & -3 & 0
\end{array}
\sim
\begin{array}{ccc|c}
3 & -5 & -1 & 0\\
0 & 2 & -3 & 0\\
0 & 0 & 0 & 0
\end{array}\\
&\To v_1= t(17, 9, 6), t\ne 0
\end{aligned}
$$
**For eigenvalue $\lm_2 = i$**, the eigenvectors
$$
\begin{aligned}
&\begin{array}{ccc|c}
4-i & 0 & 0 & 0\\
3 & -1-i & -1 & 0\\
4 & 2 & 1-i & 0
\end{array}
\sim
\begin{array}{ccc|c}
1 & 0 & 0 & 0\\
0 & 2 & 1-i & 0\\
0 & 0 & 0 & 0
\end{array}\\
&\To v_2= t(0, i-1, 2), t\ne 0
\end{aligned}
$$
**For eigenvalue $\lm_3 = -i$**, the eigenvectors
$$
\begin{aligned}
&\begin{array}{ccc|c}
4+i & 0 & 0 & 0\\
3 & -1+i & -1 & 0\\
4 & 2 & 1+i & 0
\end{array}
\sim
\begin{array}{ccc|c}
1 & 0 & 0 & 0\\
0 & 2 & 1+i & 0\\
0 & 0 & 0 & 0
\end{array}\\
&\To v_3= t(0, -i-1, 2), t\ne 0
\end{aligned}
$$
$v_1, v_2$ and $v_3$ are linearly independent eigenvectors of $A$. Let $S = [v_1, v_2, v_3]$,
$$
\begin{aligned}
S &= \begin{bmatrix}
17 & 0 & 0\\
9 & i-1 & -i-1\\
6 & 2 & 2
\end{bmatrix}\\[1.0em]
S^{-1} A S &= \text{diag}(\lm_1, \lm_2, \lm_3)\\
&= \text{diag}(4, i, -i)\\
\end{aligned}
$$
