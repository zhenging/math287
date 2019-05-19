### 4.9 The Rank-nullity Theorem

#### Rank-Nullity Theorem

**Nullity**
The dimension of _nullspace(A_) is called **nullity** of $A$.

**Rank-Nullity Theorem**
$\text{rank}(A) + \text{nullity}(A) = \# \text{ of } \text{columns of } A = n$

#### Particular Solution
+ If $x_p$ is a particular solutuion to $A\bold{x} = b$, then every solution can be written $\bold{x} = \bold{x_h} + \bold{x_p}$, where $\bold{x_h}$ is a solution to $A\bold{x} = 0$
+ The dimension of $\bold{x_h}$ is $\text{nullity}(A)$.
+ Furthermore, $\bold{b}$ must be in colspace(A)

Let $A$ be an $n\times n$ matrix with real elements. The following conditions on $A$ are equivalent.
+ A is invertible.
+ $A\bold{x} = b$ has a unique solution for every $\bold{b}$ in $\R^n$.
+ $A\bold{x} = 0$ has only trivial solutio $\bold{b}$ in $\bold{x}=0$.
+ $\text{rank}(A) = n$
+ $A$ is row-equivalent to $I_n$.
+ $\text{det}(A) \neq 0$
+ $A^T$ is invertible.
+ $\text{nullity}(A) = 0$
+ $\text{colspace}(A) = \R^N$ (that is, the columns of $A$ form a basis for $\R^n$).
+ $\text{rowspace}(A) = \R^N$ (that is, the rows of $A$ form a basis for $\R^n$).


#### Homework
p.330 1-13 all
