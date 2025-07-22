#theory 

A vector $\mathbf{v} \in \mathbb{R}^n$ can be represented in different coordinate systems (bases). A **change of basis** translates the coordinates of $\mathbf{v}$ from one basis to another.

---
### Geometric intuition

Two interpretations of the _**same**_ matrix-vector multiplication.

- Transformation view: Interpret the result as a **new vector** in the same grid (space moved).

<div align="center">
  <strong>Vector moves, grid follows</strong>
</div>

- Change-of-basis view: Interpret the result as **new coordinates** of the same geometric vector (grid redrawn).
<div align="center">
  <strong>Grid moves, vector stays</strong>
</div>

Keep the interpretation straight: _Are we moving points, or just relabeling them?_

---
### Basis and coordinates

Let $\mathcal{B} = \{ \mathbf{b}_1, \mathbf{b}_2, \ldots, \mathbf{b}_n \}$ be a basis for $\mathbb{R}^n$.  
Any vector $\mathbf{v}$ can be written uniquely as:
$$
\mathbf{v} = x_1 \mathbf{b}_1 + x_2 \mathbf{b}_2 + \cdots + x_n \mathbf{b}_n.
$$

The **coordinate vector** of $\mathbf{v}$ with respect to $\mathcal{B}$ is:
$$
[\mathbf{v}]_{\mathcal{B}} = 
\begin{pmatrix}
x_1 \\
x_2 \\
\vdots \\
x_n
\end{pmatrix}.
$$

If we arrange the basis vectors as columns of a matrix:
$$
P_{\mathcal{B}} = [ \mathbf{b}_1 \; \mathbf{b}_2 \; \cdots \; \mathbf{b}_n ],
$$
then:
$$
\mathbf{v} = P_{\mathcal{B}} [\mathbf{v}]_{\mathcal{B}}.
$$

---
### Change of basis matrix

Let $\mathcal{B} = \{\mathbf{b}_1,\ldots,\mathbf{b}_n\}$ and $\mathcal{C} = \{\mathbf{c}_1,\ldots,\mathbf{c}_n\}$ be two bases of $\mathbb{R}^n$.  
We want to find a matrix $P_{\mathcal{C}\leftarrow \mathcal{B}}$ such that:
$$
[\mathbf{v}]_{\mathcal{C}} = P_{\mathcal{C}\leftarrow \mathcal{B}} [\mathbf{v}]_{\mathcal{B}}.
$$

### Construction of $P_{\mathcal{C}\leftarrow \mathcal{B}}$

1. Express each vector $\mathbf{b}_i$ in terms of the $\mathcal{C}$ basis:
   $$
   \mathbf{b}_i = \alpha_{1i} \mathbf{c}_1 + \alpha_{2i} \mathbf{c}_2 + \cdots + \alpha_{ni} \mathbf{c}_n.
   $$
2. The columns of $P_{\mathcal{C}\leftarrow \mathcal{B}}$ are the coordinate vectors $[\mathbf{b}_i]_{\mathcal{C}}$:
   $$
   P_{\mathcal{C}\leftarrow \mathcal{B}} = \big[ [\mathbf{b}_1]_{\mathcal{C}} \; [\mathbf{b}_2]_{\mathcal{C}} \; \cdots \; [\mathbf{b}_n]_{\mathcal{C}} \big].
   $$

If we have the matrices $P_{\mathcal{B}}$ and $P_{\mathcal{C}}$ (from each basis to the standard basis), then:
$$
P_{\mathcal{C}\leftarrow \mathcal{B}} = P_{\mathcal{C}}^{-1} P_{\mathcal{B}}.
$$

---
### Example

Consider $\mathbb{R}^2$ with:
$$
\mathcal{B} = \left\{ \begin{pmatrix} 1 \\ 1 \end{pmatrix}, \begin{pmatrix} 1 \\ -1 \end{pmatrix} \right\},
\quad
\mathcal{C} = \left\{ \begin{pmatrix} 1 \\ 0 \end{pmatrix}, \begin{pmatrix} 0 \\ 1 \end{pmatrix} \right\}.
$$

We have:
$$
P_{\mathcal{B}} = 
\begin{pmatrix}
1 & 1 \\
1 & -1
\end{pmatrix}, \quad
P_{\mathcal{C}} = I_2.
$$

Thus:
$$
P_{\mathcal{C}\leftarrow \mathcal{B}} = P_{\mathcal{C}}^{-1} P_{\mathcal{B}} = 
\begin{pmatrix}
1 & 1 \\
1 & -1
\end{pmatrix}.
$$

If $\mathbf{v} = \begin{pmatrix} 3 \\ 1 \end{pmatrix}$ in the standard basis, then:
$$
[\mathbf{v}]_{\mathcal{B}} = P_{\mathcal{B}}^{-1} \mathbf{v}
= \frac{1}{2}
\begin{pmatrix}
1 & 1 \\
1 & -1
\end{pmatrix}
\begin{pmatrix}
3 \\
1
\end{pmatrix}
= \frac{1}{2}
\begin{pmatrix}
4 \\
2
\end{pmatrix}
= \begin{pmatrix}
2 \\
1
\end{pmatrix}.
$$

---
### Key Points

- $P_{\mathcal{B}}$ maps $\mathcal{B}$-coordinates to standard coordinates.
- $P_{\mathcal{B}}^{-1}$ maps standard coordinates to $\mathcal{B}$-coordinates.
- Changing from basis $\mathcal{B}$ to basis $\mathcal{C}$ is done via:
  $$
  [\mathbf{v}]_{\mathcal{C}} = P_{\mathcal{C}}^{-1} P_{\mathcal{B}} [\mathbf{v}]_{\mathcal{B}}.
  $$
