#theory 

A **ring** $R$ is a set with two binary operations:

- Addition $+$: $(R, +)$ is an abelian group.
- Multiplication $\cdot$: $(R, \cdot)$ is a semigroup (associative).

Multiplication **distributes over addition**:
- $a(b + c) = ab + ac$
- $(a + b)c = ac + bc$

---
### Common Variants

- **Commutative ring**: $ab = ba$ for all $a, b$
- **Ring with unity**: has multiplicative identity $1$
- **Integral domain**: commutative ring with no zero divisors
- **Division ring**: all nonzero elements have multiplicative inverses (but not necessarily commutative)

---
### Examples

- $\mathbb{Z}$: integers — commutative ring with identity
- $\mathbb{Z}_n$: integers mod $n$
- $\mathbb{R}[x]$: polynomials with real coefficients
- $M_n(\mathbb{R})$: all $n \times n$ matrices over $\mathbb{R}$ — noncommutative ring
- $\mathbb{Q}$: a field (and hence also a ring)

---
### Related Concepts

- **Ring homomorphism**: preserves both operations
- **Ideal**: like a subgroup, but under multiplication too
- **Quotient ring**: $R/I$ when $I$ is an ideal
- **Zero divisors**: $ab = 0$ but $a, b \ne 0$

---
### Summary

Rings generalize arithmetic: combining additive group structure with multiplication and distributive laws. Many number systems and polynomial structures are rings.