#theory 

### 1. The starting point: Sets

A **set** is simply a collection of elements:
$$
X = \{ x_1, x_2, \dots, x_n, \dots \}
$$
At this stage, no additional structure is present. The set only allows us to ask:
- **Is $x$ an element of $X$?**

**Example:**
- $X = \{ 1, 2, 3 \}$.
- $X = \mathbb{R}$, the set of real numbers.

---
### 2. From Sets to Topological Spaces

To turn a set into a **topological space**, we specify which subsets are considered **open**.  
A topological space is a pair $(X, \mathcal{T})$ where:
- $X$ is a set.
- $\mathcal{T} \subseteq \mathcal{P}(X)$ (the power set of $X$) satisfies:
  1. $\emptyset, X \in \mathcal{T}$.
  2. Any union of sets in $\mathcal{T}$ is in $\mathcal{T}$.
  3. Any finite intersection of sets in $\mathcal{T}$ is in $\mathcal{T}$.

This gives $X$ a **notion of continuity and neighborhood**.

**Examples:**
- $(\mathbb{R}, \mathcal{T}_{\text{std}})$, where $\mathcal{T}_{\text{std}}$ is the standard topology (open intervals $(a,b)$).
- A finite set with **discrete topology**: every subset is open.

---
### 3. Metric Spaces: Adding Distance

A **metric space** $(X, d)$ introduces a function:
$$
d: X \times X \to \mathbb{R}_{\ge 0}
$$
such that:
1. $d(x,y) = 0 \iff x = y$.
2. $d(x,y) = d(y,x)$.
3. $d(x,z) \le d(x,y) + d(y,z)$ (triangle inequality).

This allows us to measure **how far points are**.

**Examples:**
- $(\mathbb{R}, d(x,y) = |x-y|)$.
- The Euclidean plane $\mathbb{R}^2$ with $d((x_1, y_1), (x_2, y_2)) = \sqrt{(x_1 - x_2)^2 + (y_1 - y_2)^2}$.
- Discrete metric: $d(x,y) = 0$ if $x=y$, else $1$.

---
### 4. Vector Spaces: Adding Algebraic Structure

A **vector space** $V$ over a field $\mathbb{F}$ is a set equipped with:
- **Vector addition:** $+: V \times V \to V$.
- **Scalar multiplication:** $\cdot : \mathbb{F} \times V \to V$.

These operations satisfy linearity axioms (associativity, distributivity, etc.).  
Vector spaces allow for **linear combinations** of elements.

**Examples:**
- $\mathbb{R}^n$ with usual vector addition and scalar multiplication.
- The set of polynomials $\mathbb{R}[x]$ with real coefficients.
- The space of continuous functions $C([0,1])$ with pointwise addition.

---
### 5. Normed and Inner Product Spaces

Adding a **norm** $\|\cdot\| : V \to \mathbb{R}_{\ge 0}$ gives a **normed vector space**.  
If this norm is induced by an **inner product** $\langle \cdot, \cdot \rangle$, we get an **inner product space**.

**Examples:**
- $\mathbb{R}^n$ with $\|x\|_2 = \sqrt{x_1^2 + \dots + x_n^2}$.
- $L^2([0,1])$ with $\langle f,g \rangle = \int_0^1 f(x) g(x) \, dx$.

---
### 6. Hilbert Spaces: Completing the Structure

A **Hilbert space** is a complete inner product space. Completeness means **every Cauchy sequence converges** in the space.

**Examples:**
- $\mathbb{R}^n$ (finite-dimensional Euclidean space).
- $L^2(\mathbb{R})$, the space of square-integrable functions.

---
### 7. The Hierarchy of Spaces

We can see the progression as:
$$
\text{Set} \subset \text{Topological Space} \subset \text{Metric Space} \subset \text{Normed Space} \subset \text{Inner Product Space} \subset \text{Hilbert Space}
$$
Each step adds **new structure and new properties**.


---
### 8. Beyond Hilbert Spaces

Hilbert spaces are not the ultimate end; beyond them, we encounter generalizations:

- **Banach Spaces:** Complete normed spaces (not necessarily with inner product).  
  Example: $C([0,1])$ with the supremum norm is Banach but not Hilbert.
  
- **Fréchet Spaces:** Topological vector spaces with a metric defined by a countable family of seminorms.  
  Example: The space of smooth functions $C^\infty(\mathbb{R})$.
  
- **Rigged Hilbert Spaces (Gelfand triplets):**  
  $$
  \Phi \subset H \subset \Phi'
  $$
  Used in quantum mechanics to handle distributions and unbounded operators.

- **C*-Algebras / von Neumann Algebras:** Operator-algebraic generalizations of Hilbert space structures.