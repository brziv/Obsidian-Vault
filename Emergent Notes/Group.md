#theory 

A **group** is a set $G$ with a binary operation $\cdot : G \times G \to G$ satisfying:

1. **Closure**: $\forall$ $a, b \in G$, $a \cdot b \in G$
2. **Associativity**: $(a \cdot b) \cdot c = a \cdot (b \cdot c)$
3. **Identity**: $\exists$ $e \in G$ such that $e \cdot a = a \cdot e = a$ for all $a \in G$
4. **Inverses**: $\forall$ $a \in G$, $\exists$ $a^{-1} \in G$ such that $a \cdot a^{-1} = a^{-1} \cdot a = e$

If $a \cdot b = b \cdot a$ for all $a, b \in G$, the group is **abelian** (commutative).

---
### Examples

- $(\mathbb{Z}, +)$: additive abelian group
- $(\mathbb{R}^*, \cdot)$: nonzero reals under multiplication
- $(\mathbb{Z}_n, +)$: integers modulo $n$
- $\mathbb{Z}/n\mathbb{Z}$ — finite cyclic group of order $n$.  
- $S_n$: symmetric group of permutations on $n$ elements
- $D_n$: dihedral group (symmetries of an $n$-gon)

---
### Symmetry as a Group Action

A **group action** describes how a group "acts" on a set — formalizing symmetry.

Examples:
- $S_n$ acting on $\{1, 2, ..., n\}$ via permutations.  
- $D_n$ acting on the vertices of a regular polygon.  
- Molecule symmetry in chemistry: point groups.  
- Crystals: space groups in 3D.

**Physics & Chemistry**:
- Conservation laws ⇔ symmetries (Noether’s theorem).  
- Particle physics: Lie groups like SU(3), SU(2), U(1).  
- Chemistry: analyze molecular vibrations via group representations.  

---
### Galois Theory and the Quintic

- Solving polynomials = understanding symmetry of **roots**.  
- For degree $\le 4$, symmetry group of roots is **solvable**.  
- Degree 5: $S_5$ is **not solvable** $\Rightarrow$ no general quintic formula.  
- Galois theory connects:
  - Field extensions  
  - Permutation groups of roots  
  - Solvability of equations  

---
### Finite and Infinite Groups

The question isn't “what things have symmetry?” but:
	What are **all the possible structures of symmetry**?

- **Finite**: $S_n$, $D_n$, $\mathbb{Z}/n\mathbb{Z}$, matrix groups over finite fields.  
- **Infinite**: $\mathbb{Z}$, $\mathbb{Q}$, $\text{GL}_n(\mathbb{R})$, Lie groups.  

---
### Classification of Finite Simple Groups
 
**Simple groups**: no nontrivial normal subgroups. Building blocks of all finite groups.

#### Jordan-Hölder Theorem:

Every finite group has a composition series of simple groups — like factoring integers into primes.

#### Classification Project (1955–2004):

- Goal: find **all finite simple groups**.  
- Result:
  - **18 infinite families**, including:
    - Cyclic groups $\mathbb{Z}/p\mathbb{Z}$  
    - Alternating groups $A_n$ for $n \ge 5$  
    - Lie-type groups over finite fields (e.g. $PSL_n(q)$)  
  - **26 sporadic groups** (“leftovers”):
    - 20 in the “happy family” (subquotients of the Monster)  
    - 6 “pariahs” that don’t fit in  

---
### The Monster Group

- Largest sporadic group: order $\approx 8 \times 10^{53}$.  
- Symmetry group in **196,883** dimensions.  
- Connects to string theory, vertex operator algebras, and **modular forms**.

#### Monstrous Moonshine:

Strange link between:
- Fourier coefficients of modular functions  
- Representation theory of the Monster  
- Functions on elliptic curves