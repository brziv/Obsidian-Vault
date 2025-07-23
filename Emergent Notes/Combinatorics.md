#theory 

The study of [[Counting]], arrangements, and discrete structures.

[[Graph theory]]

A graph $G = (V, E)$ consists of:
- a set of vertices $V$
- a set of edges $E \subseteq V \times V$

Example problems:
- Eulerian path: a path that uses every edge exactly once.
- Hamiltonian cycle: a cycle visiting every vertex exactly once.
- Graph coloring: minimal number of colors so adjacent vertices differ.

---
#### Set Systems and Designs

Block designs: arranging subsets (blocks) so that elements occur in balanced ways.
Latin squares: $n \times n$ grids filled with $n$ symbols, each appearing once per row and column.
Applications: experiment planning, error-correcting codes, scheduling tournaments.

---
#### Partitions

Integer partitions: ways to write $n$ as a sum of positive integers.
Example: $4 = 4 = 3+1 = 2+2 = 2+1+1 = 1+1+1+1$ (5 partitions).
Set partitions: splitting a set $S$ into non-empty, disjoint subsets whose union is $S$.

---
#### Ramsey Theory

Order emerges in large enough structures.
Example: In any group of 6 people, there are 3 mutual friends or 3 mutual strangers.

---
#### Polya Counting and Symmetry

Counting distinct objects up to symmetry using group actions (Burnside's Lemma, Polya's Enumeration Theorem).
Example: count distinct colorings of a cube with 3 colors, ignoring rotations.

---
#### Generating Functions

Use power series to encode counting problems and study sequences.
Example: ways to make change for $n$ using coins with denominations $1,2,5,\dots$ can be encoded by
$$
(1 + x + x^2 + \cdots)(1 + x^2 + x^4 + \cdots)(1 + x^5 + x^{10} + \cdots)\cdots
$$

---
#### Combinatorial Proofs

Prove identities by interpreting both sides as counting the same structure.
Example: $\binom{n}{k} = \binom{n}{n-k}$ by choosing which $k$ to include versus which $n-k$ to exclude from an $n$-element set.