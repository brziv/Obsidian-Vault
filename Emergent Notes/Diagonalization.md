#theory 

A matrix $A \in \mathbb{R}^{n \times n}$ is **diagonalizable** if there exists an invertible matrix $P$ and a diagonal matrix $D$ such that:
$$
A = P D P^{-1},
$$
or equivalently:
$$
P^{-1} A P = D.
$$
The columns of $P$ are **eigenvectors** of $A$, and the diagonal entries of $D$ are the corresponding **eigenvalues**.

---
### Why does this work?

If $A$ has $n$ linearly independent eigenvectors $\mathbf{v}_1, \ldots, \mathbf{v}_n$, we can form:
$$
P = [ \mathbf{v}_1 \; \mathbf{v}_2 \; \cdots \; \mathbf{v}_n ].
$$
Then:
$$
A P = A [\mathbf{v}_1 \; \cdots \; \mathbf{v}_n]
= [A \mathbf{v}_1 \; \cdots \; A \mathbf{v}_n]
= [\lambda_1 \mathbf{v}_1 \; \cdots \; \lambda_n \mathbf{v}_n]
= P D,
$$
where:
$$
D = \text{diag}(\lambda_1, \lambda_2, \ldots, \lambda_n).
$$
Multiplying by $P^{-1}$ yields $P^{-1} A P = D$.

---

### Geometric intuition

1. Eigenvectors as "natural directions":  
   A general linear transformation $A$ might rotate, shear, and stretch space. Eigenvectors identify the "fixed directions" where $A$ acts as pure scaling.  
   - For $\mathbf{v}$ an eigenvector, $A \mathbf{v}$ is **collinear** with $\mathbf{v}$.

2. Diagonalization as [[Change of basis]]: 
   In the standard basis, $A$ might look complicated. But if we **choose the eigenvectors as a new basis**, $A$ becomes diagonal:
   - Diagonal matrices just scale each axis independently.
   - So diagonalization is about finding a coordinate system where $A$ acts as a simple stretch along coordinate axes.

3. Visualizing in 2D:  
   - Think of a $2 \times 2$ matrix $A$ as transforming the plane.
   - Eigenvectors show the two "special" lines that $A$ does not rotate—only stretches (or compresses).
   - If $A$ can be diagonalized, we can "rotate" our viewpoint (via $P$) so that $A$ appears as a simple rescaling along the new x- and y-axes.

---
### When is a Matrix Diagonalizable?

- $A$ is diagonalizable if and only if it has **$n$ linearly independent eigenvectors**.
- A sufficient condition: $A$ has $n$ distinct eigenvalues.
- Symmetric matrices are always diagonalizable (by the Spectral Theorem).

---
### Example (2×2 Matrix)

Take:
$$
A = \begin{pmatrix}
2 & 1 \\
1 & 2
\end{pmatrix}.
$$
We have eigenvalues $\lambda_1 = 1, \lambda_2 = 3$, with eigenvectors:
$$
\mathbf{v}_1 = \begin{pmatrix} 1 \\ -1 \end{pmatrix}, \quad
\mathbf{v}_2 = \begin{pmatrix} 1 \\ 1 \end{pmatrix}.
$$
Form:
$$
P = \begin{pmatrix}
1 & 1 \\
-1 & 1
\end{pmatrix}, \quad
D = \begin{pmatrix}
1 & 0 \\
0 & 3
\end{pmatrix}.
$$
Check:
$$
P^{-1} A P = D.
$$
Thus, in the eigenbasis, $A$ just stretches one axis by $1$ and the other by $3$.