#theory 

Studies ways to count, arrange, and select objects, often under certain constraints.

#### Rule of Sum
If a task can be done in $m$ ways or $n$ ways (but not both), then the total number of ways is
$$
m + n.
$$

#### Rule of Product
If a task consists of two independent stages, with $m$ ways for the first stage and $n$ ways for the second, then the total number of ways is
$$
m \cdot n.
$$

---
### Factorial
The factorial of $n$ is
$$
n! = n \cdot (n-1) \cdot (n-2) \cdots 2 \cdot 1,
$$
with $0! = 1$.

---
### Permutations (nPr)

- **Permutation of $n$ elements**:  
  Number of ways to arrange $n$ distinct objects:
  $$
  P(n) = n!
  $$

- **Permutation of $k$ elements from $n$**:  
  $$
  P(n,k) = \frac{n!}{(n-k)!}
  $$

---
### Combinations (nCr)

Number of ways to choose $k$ elements from $n$ (order does not matter):
$$
C(n,k) = \binom{n}{k} = \frac{n!}{k!(n-k)!}.
$$

---
#### Binomial Theorem
For any non-negative integer $n$,
$$
(x + y)^n = \sum_{k=0}^n \binom{n}{k} x^{n-k} y^k.
$$

---
#### Inclusion-exclusion principle
For two sets $A, B$:
$$
|A \cup B| = |A| + |B| - |A \cap B|.
$$
For three sets:
$$
|A \cup B \cup C| = |A| + |B| + |C| - |A \cap B| - |B \cap C| - |C \cap A| + |A \cap B \cap C|.
$$

---
#### Pigeonhole Principle

If $n$ items are placed into $m$ boxes and $n > m$, then at least one box contains at least
$$
\left\lceil \frac{n}{m} \right\rceil
$$
items.

**Example:**  
If 13 socks are placed in 12 drawers, then at least one drawer must contain at least 2 socks.