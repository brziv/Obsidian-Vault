#theory 

The study of algebraic structures and the rules that govern them. Instead of focusing on numbers, it focuses on **operations and relations** that behave like arithmetic, but in a much more general and structural way.

- Unifies seemingly different mathematical objects under a common language.
- Provides tools to study **symmetry, number theory, polynomials, geometry**, and more.
- Essential for **modern mathematics**, **physics**, **cryptography**, and **algebraic geometry**.

---
### Core Structures

#### 1. **Group**

- Single operation
- Models symmetry, invertibility, and structure
- Examples: $(\mathbb{Z}, +)$, $S_n$, $D_n$

→ See: [[Group]]

#### 2. **Ring**

- Two operations: addition and multiplication
- Generalizes integers and polynomial arithmetic
- Examples: $\mathbb{Z}$, $\mathbb{Z}_n$, $\mathbb{R}[x]$

→ See: [[Ring]]

#### 3. **Field**

- Ring where every nonzero element has a multiplicative inverse
- Enables full arithmetic: addition, subtraction, multiplication, division
- Examples: $\mathbb{Q}, \mathbb{R}, \mathbb{C}, \mathbb{F}_p$

→ See: [[Field]]

#### 4. **Module**

- Generalizes vector spaces: scalar multiplication from a **ring**, not necessarily a field
- Used to study systems of equations, representations, and algebraic geometry
- Examples: $\mathbb{Z}$-modules = abelian groups, $R^n$, polynomial modules

→ See: [[Module]]

---
### How They Relate

$\text{Group} \rightarrow \text{Ring} \rightarrow \text{Field}$ 

- A **ring** includes an **abelian group** under addition.
- A **field** is a special kind of **ring** where every nonzero element is invertible under multiplication (forming a multiplicative abelian group).
- A **module** is a generalization of vector space: it’s a structure where a **ring** acts on an abelian group.
- A **vector space** is just a **module over a field**.

---
### Common Themes

- **Binary operations**: addition, multiplication, etc.
- **Identities and inverses**
- **Homomorphisms**: structure-preserving maps
- **Substructures**: subgroups, subrings, submodules
- **Quotients and ideals**: factor out structure
- **Isomorphism**: structural equivalence

---
### Where It Leads

- **Galois Theory**: field extensions and polynomial solvability via groups
- **Representation Theory**: groups/rings via matrices and modules
- **Algebraic Geometry**: geometry from rings and modules
- **Homological Algebra**: algebraic methods to study structure and invariants
- **Commutative Algebra**: study of commutative rings (especially local rings, Noetherian rings, etc.)