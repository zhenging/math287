### 4.6 Base and Dimension

**Basis**
A minimal spanning set of a vector space is called a **basis** of that vector space. The plural of basis is **bases**.

Let $V$ be a vector space, and let $S = \{v_1, v_2, v_3, v_4, v_5\}$ be a basis of $V$
1. All bases of V have exactly 5 vectors.
2. The dimension of $V$ is 5.
3. $S$ has no "deadweight".
4. _minimal spanning set_
  + If you add any vectors to $S$, then the bigger set is still a spanning sef $V$.
  + If you take away vectors from $S$, then the samller set is not a spanninet of $V$.
5. _maximumal independent set_
  + If you add any vectors to $S$, then the bigger set is not an independenet.
  + If you take away vectors from $S$ (provided you don't take the last one)hen the samller set is still an independent set.
6. Any set of 5 independent vectors is a basis.
7. Any set of 5 vectors that spans $V$ is a basis.
8. Any spanning set of $V$ must contain 5 vectors or more.
9. Any independent set must contain 5 vectors of less.
10. If $T$ is a subspace of $V$, then $\text{dim}(T) \le 5$.
11. If $T$ is a subspace of $V$, then any basis for $T$ is part of a basis  $V$.

**Finite/Infinite-dimensional vector space**
If a vector space $V$ has a basis consisting of a finite number of vectors, then $V$ is called a **finite-dimensional vector space**. Otherwise V is called an **infinite-dimensional vector space**.

If $\text{dim}[V] = n$, and $S$ is a set of vectors, then the following statements are equivalent.
+ $S$ is a basis.
+ $S$ is linearly independent.
+ $S$ spans $V$.

If $V$ is a vector space with basis $B$, then every vector in $V$ can be written uniquely as a linear combination of the vectors in $B$.

#### Homework
p.308 1-7 all, 9-30 all, 32-35 all, 37, 39, 41a, 42a, 45-47 all

20-23\. Find the dimension of the null space of the givern matrix $A$.
20\. $A = \begin{bmatrix}
1 & 3\\
-2 & -6
\end{bmatrix}$
>Solution
$$
\begin{aligned}
&\begin{bmatrix}
1 & 3\\
-2 & -6
\end{bmatrix}
\sim
\begin{bmatrix}
1 & 3\\
0 & 0
\end{bmatrix}\\[1.0em]
&\To c_1 = -3t, c_2 = t
\end{aligned}
$$
nullspace(A) = $\{t(-3, 1), t\in \R\}$, dimension  = 1

22\. $A = \begin{bmatrix}
1 & -1 & 4\\
2 & 3 & -2\\
1 & 2 & -2
\end{bmatrix}$
>Solution
$$
\begin{aligned}
&\begin{bmatrix}
1 & -1 & 4\\
2 & 3 & -2\\
1 & 2 & -2
\end{bmatrix}
\sim
\begin{bmatrix}
1 & -1 & 4\\
0 & 1 & -2\\
0 & 0 & 0
\end{bmatrix}\\[1.0em]
&\To c_1 = -2t, c_2 = 2t, c_3 = t
\end{aligned}
$$
nullspace(A) = $\{t(-2, 2, 1), t\in \R\}$, dimension  = 1
