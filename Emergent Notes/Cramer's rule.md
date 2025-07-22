#theory 

A method to solve a system of $n$ linear equations with $n$ unknowns, given that the coefficient matrix is invertible ($\det \neq 0$).

### Geometric intuition

Write the columns of $A$ as vectors $a_1, a_2, \ldots, a_n \in \mathbb{R}^n$, so
$$
A = [\,a_1 \; a_2 \; \cdots \; a_n\,].
$$

The parallelepiped spanned by these column vectors has oriented $n$-dimensional volume $\det(A)$:
- In $n=2$, $\det(A)$ is the signed area of the parallelogram formed by $a_1$ and $a_2$.
- In $n=3$, it is the signed volume of the parallelepiped formed by $a_1,a_2,a_3$.
- Sign encodes orientation (whether the ordered set of columns preserves or reverses orientation relative to the standard basis).
- If $\det(A)=0$, the columns are linearly dependent: the "volume" collapses to a lower dimension, so they do **not** form a basis; the system need not have a unique solution.

Now suppose we want to express a vector $b$ in this column basis:
$$
b = x_1 a_1 + x_2 a_2 + \cdots + x_n a_n.
$$
Multilinearity of the determinant implies that if we replace the $i$-th column $a_i$ with $b$, the new determinant scales by $x_i$:
$$
\det(a_1,\ldots,b,\ldots,a_n) = x_i \det(a_1,\ldots,a_i,\ldots,a_n).
$$
Rearranging gives
$$
x_i = \frac{\det(a_1,\ldots,b,\ldots,a_n)}{\det(a_1,\ldots,a_i,\ldots,a_n)} = \frac{\det(A_i)}{\det(A)}.
$$
This geometric ratio view *is* Cramer's Rule: each coordinate $x_i$ measures how much of $a_i$ you need to reach $b$, read off as a volume (or area) ratio.

### System of equations

Consider the linear system:

$$
A \mathbf{x} = \mathbf{b}
$$

where:

- $A$ is an $n \times n$ matrix,
- $\mathbf{x} = (x_1, x_2, \ldots, x_n)^T$ is the vector of unknowns,
- $\mathbf{b} = (b_1, b_2, \ldots, b_n)^T$ is the vector of constants.

### Cramer's rule

If $\det(A) \neq 0$, the unique solution is given by:

$$
x_i = \frac{\det(A_i)}{\det(A)}, \quad i = 1, 2, \ldots, n
$$

where $A_i$ is the matrix $A$ with its $i$-th column replaced by the vector $\mathbf{b}$.

### Example

For a $2 \times 2$ system:

$$
\begin{cases}
a_{11} x_1 + a_{12} x_2 = b_1 \\
a_{21} x_1 + a_{22} x_2 = b_2
\end{cases}
$$

We have:

$$
A =
\begin{pmatrix}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{pmatrix},
\quad
\det(A) = a_{11}a_{22} - a_{12}a_{21}
$$

$$
x_1 = \frac{
\begin{vmatrix}
b_1 & a_{12} \\
b_2 & a_{22}
\end{vmatrix}
}{\det(A)}
= \frac{b_1 a_{22} - b_2 a_{12}}{a_{11}a_{22} - a_{12}a_{21}}
$$

$$
x_2 = \frac{
\begin{vmatrix}
a_{11} & b_1 \\
a_{21} & b_2
\end{vmatrix}
}{\det(A)}
= \frac{a_{11} b_2 - a_{21} b_1}{a_{11}a_{22} - a_{12}a_{21}}
$$
