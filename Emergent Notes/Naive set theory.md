#theory 

$$
\begin{array}{c}
A = \{1,2,3\} \\
\{1,2\} \notin A, \quad \{1,2\} \subseteq A
\end{array}
$$

$$
\begin{array}{c}
B = \{\{1,2\}, 3\} \\
\{1,2\} \in B, \quad 1 \in \{1,2\}, \quad 1 \notin B, \quad \{1,2\} \not \subseteq B
\end{array}
$$

$$
\begin{array}{c}
C = \{\{1\}, 1\} \\
\{1\} \in C, \quad 1 \in \{1\}, \quad 1 \in C, \quad \{1\} \subseteq C
\end{array}
$$

---
#### Empty set

$$
\begin{array}{c}
\varnothing = \{\} \\
\varnothing \in \{\varnothing\}, \quad \varnothing \subseteq A, \quad A \notin A
\end{array}
$$

---
#### Power set

$$
\begin{array}{c}
\mathcal{P}(A) = \{\varnothing, \{1\}, \{2\}, \{3\}, \{1,2\}, \{1,3\}, \{2,3\}, \{1,2,3\}\} \\
\{1,2\} \in \mathcal{P}(A), \quad \{1,4\} \notin \mathcal{P}(A)
\end{array}
$$

---
#### Operations

$$
A \cup B = \{1,2,3,\{1,2\}\}, \quad A \cap B = \{3\}, \quad A \setminus B = \{1,2\}
$$

**Laws of Set Algebra:**
$$
A \cup \varnothing = A, \quad A \cap \varnothing = \varnothing
$$
$$
A \cup A = A, \quad A \cap A = A
$$
$$
A \cup (B \cap C) = (A \cup B) \cap (A \cup C)
$$
$$
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
$$

---
#### Cartesian product

$$
A \times \{x,y\} = \{(1,x), (1,y), (2,x), (2,y), (3,x), (3,y)\}
$$

---
#### Relations and functions

A **relation** on $A$ is any subset of $A \times A$:
$$
R = \{(1,2), (2,3)\} \subseteq A \times A
$$

A **function** $f : A \to B$ is a relation where each $a \in A$ appears exactly once as a first element:
$$
f = \{ (1,x), (2,x), (3,y) \}
$$

---
#### Cardinality

$$
|A| = 3, \quad |\varnothing| = 0
$$

A set is **finite** if it can be matched with $\{1,2,\dots,n\}$ for some $n$.

Infinite set:
$$
\mathbb{N} = \{0,1,2,3,\dots\}
$$

**Cantor’s theorem:**
$$
|\mathcal{P}(A)| > |A|
$$

---
#### Russell’s paradox

$$
\forall P(x), \ \exists \, S \ \text{such that} \ S = \{ x \mid P(x) \}.
$$

$$
R = \{ x \mid x \notin x \}
$$

##### Case 1: $R \in R$ 
$$
x \in R \implies x \notin x.
$$
Therefore,
$$
R \in R \implies R \notin R.
$$
Contradiction.

##### Case 2: $R \notin R$ 

Satisfies the property $x \notin x$ , so:
$$
R \notin R \implies R \in R.
$$
Contradiction.

Conclusion: $R$ cannot exist.

In ZFC:
$$
\forall A, \ \exists S = \{ x \in A \mid P(x) \}.
$$
