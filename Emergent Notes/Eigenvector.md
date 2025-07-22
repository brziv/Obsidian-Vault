#theory 

For a linear transformation $T: V \to V$ (or a square matrix $A \in \mathbb{R}^{n \times n}$), a **nonzero vector** $\mathbf{v}$ is called an **eigenvector** if there exists a scalar $\lambda \in \mathbb{R}$ such that:
$$
T(\mathbf{v}) = \lambda \mathbf{v},
$$
or equivalently (for matrices):
$$
A \mathbf{v} = \lambda \mathbf{v}.
$$

The scalar $\lambda$ is called an **eigenvalue** of $A$ corresponding to $\mathbf{v}$.

---
### Geometric intuition

 An eigenvector marks a direction in which the transformation acts by simple scaling.
 
#### 1. Invariant lines (or subspaces)

Pick any nonzero $\mathbf{v}$. Under $A$, most directions get sent to some new direction. But if $\mathbf{v}$ is an eigenvector, then $A\mathbf{v}$ lies on the **same line** $\text{span}{\mathbf{v}}$. That line is _invariant_ under $A$.

- If $\lambda > 1$: vectors on that line are **stretched**.

- If $0 < \lambda < 1$: vectors are **compressed** toward the origin.

- If $\lambda = 1$: vectors on that line are **unchanged in direction and length** (a fixed direction, isometric along that line).
    
- If $\lambda = -1$: vectors **flip direction** (180°) but keep length.

- If $\lambda < 0$ in general: scale and **flip**.

- If $\lambda = 0$: the whole invariant line **collapses to the origin**.

#### 2. Grid deformation picture

Imagine a square grid drawn in the plane (for $\mathbb{R}^2$). Apply $A$ to every grid point.

- The grid usually shears, rotates, and stretches.

- Eigenvector directions show up as straight grid axes that don’t turn - they may stretch, shrink, or flip, but they stay _colinear_.

---
### Eigenvalue equation

To find eigenvalues, we look for $\lambda$ such that:
$$
(A - \lambda I)\mathbf{v} = \mathbf{0},
$$
where $I$ is the identity matrix.

For a nontrivial solution $\mathbf{v} \neq \mathbf{0}$, we require:
$$
\det(A - \lambda I) = 0.
$$
This determinant expands to a polynomial of degree $n$ (the **characteristic polynomial**), whose roots are the eigenvalues.

---
### Eigenspaces

For a given eigenvalue $\lambda$, the set of all eigenvectors (plus the zero vector) forms a subspace:
$$
E_\lambda = \{ \mathbf{v} \in \mathbb{R}^n : (A - \lambda I) \mathbf{v} = 0 \} = \ker(A - \lambda I).
$$
The **geometric multiplicity** of $\lambda$ is $\dim E_\lambda$.

---
### Example (2x2)

Consider:
$$
A = 
\begin{pmatrix}
2 & 1 \\
1 & 2
\end{pmatrix}.
$$

**Step 1:** Find eigenvalues  
Solve:
$$
\det(A - \lambda I) = \det 
\begin{pmatrix}
2-\lambda & 1 \\
1 & 2-\lambda
\end{pmatrix}
= (2-\lambda)^2 - 1 = 0.
$$
This simplifies to:
$$
(2-\lambda)^2 = 1 \implies 2 - \lambda = \pm 1 \implies \lambda = 1, 3.
$$

**Step 2:** Find eigenvectors  
For $\lambda = 1$:
$$
(A - I) = 
\begin{pmatrix}
1 & 1 \\
1 & 1
\end{pmatrix},
\quad
\begin{pmatrix}
1 & 1 \\
1 & 1
\end{pmatrix} 
\begin{pmatrix}
x \\
y
\end{pmatrix} = 
\begin{pmatrix}
0 \\
0
\end{pmatrix}
\implies x = -y.
$$
Eigenvectors: $\mathbf{v} = t \begin{pmatrix} 1 \\ -1 \end{pmatrix}$.

For $\lambda = 3$:
$$
(A - 3I) = 
\begin{pmatrix}
-1 & 1 \\
1 & -1
\end{pmatrix},
\quad x = y.
$$
Eigenvectors: $\mathbf{v} = t \begin{pmatrix} 1 \\ 1 \end{pmatrix}$.

[[Diagonalization]]
