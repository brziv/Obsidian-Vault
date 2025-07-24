#theory 

A **vector space** (or linear space) over a field $F$ is a set $V$ equipped with two operations:
1. **Vector addition**: $+: V \times V \to V$,
2. **Scalar multiplication**: $\cdot: F \times V \to V$,

satisfying the following axioms for all $u,v,w \in V$ and all scalars $a,b \in F$:

- **Associativity of addition:** $(u + v) + w = u + (v + w)$,
- **Commutativity of addition:** $u + v = v + u$,
- **Existence of additive identity:** There exists $0 \in V$ such that $u + 0 = u$,
- **Existence of additive inverse:** For each $u \in V$, there exists $-u$ such that $u + (-u) = 0$,
- **Compatibility of scalar multiplication:** $a (b u) = (ab) u$,
- **Identity element of scalar multiplication:** $1 u = u$,
- **Distributivity of scalar multiplication with respect to vector addition:** $a (u + v) = a u + a v$,
- **Distributivity of scalar multiplication with respect to field addition:** $(a + b) u = a u + b u$.

---
#### What Is a Vector?

A **vector** is any element $v \in V$ of a vector space $V$.

- In $\mathbb{R}^n$, vectors are usually represented as tuples: $v = (v_1, v_2, \dots, v_n)$
- In function spaces, vectors can be functions: $f \in C^\infty(\mathbb{R})$, etc.
- In abstract algebra, a vector might be a formal object with no concrete representation, defined only by the axioms.

---
### Infinite-Dimensional Polynomial Space

The set of all polynomials in one variable $x$ with real coefficients is:
$$
\mathbb{R}[x] = \{\, p(x) = a_0 + a_1 x + a_2 x^2 + \dots + a_n x^n \mid n \in \mathbb{N}, \, a_i \in \mathbb{R} \,\}.
$$

#### Basis

The natural basis of $\mathbb{R}[x]$ is:
$$
\mathcal{B} = \{ 1, x, x^2, x^3, \dots \}.
$$

This basis is **countably infinite**, meaning $\mathbb{R}[x]$ is an **infinite-dimensional vector space**.

---
### Linear Operators on $\mathbb{R}[x]$

#### Derivative Operator

The derivative $D: \mathbb{R}[x] \to \mathbb{R}[x]$ is a **linear map**:
$$
D(p+q) = Dp + Dq, \quad D(cp) = c Dp.
$$

In terms of the basis $\{1, x, x^2, \dots\}$, we can represent $D$ as an infinite matrix acting on the coefficient vector $\mathbf{a} = (a_0, a_1, a_2, \dots)^T$:

$$
D =
\begin{pmatrix}
0 & 1 & 0 & 0 & 0 & \dots \\
0 & 0 & 2 & 0 & 0 & \dots \\
0 & 0 & 0 & 3 & 0 & \dots \\
0 & 0 & 0 & 0 & 4 & \dots \\
\vdots & \vdots & \vdots & \vdots & \vdots & \ddots
\end{pmatrix}.
$$

#### Integral Operator

Similarly, the (indefinite) integral operator $I$, taking constant of integration to be $0$, has matrix:
$$
I =
\begin{pmatrix}
0 & 0 & 0 & 0 & \dots \\
1 & 0 & 0 & 0 & \dots \\
0 & \frac{1}{2} & 0 & 0 & \dots \\
0 & 0 & \frac{1}{3} & 0 & \dots \\
\vdots & \vdots & \vdots & \vdots & \ddots
\end{pmatrix}.
$$

Thus, differentiation and integration can be viewed as **matrix multiplications** on the infinite-dimensional vector of polynomial coefficients.

---
### Key Idea

This example illustrates that:
- A polynomial can be seen as a **vector** in an infinite-dimensional space.
- Differentiation and integration are **linear operators**, represented by infinite matrices with specific patterns (e.g., subdiagonal entries $1,2,3,\dots$ for $D$).