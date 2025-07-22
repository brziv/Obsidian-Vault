#theory 

A **relation** $R$ on a set $A$ is called an **equivalence relation** if it satisfies **all three properties**:

- **Reflexive:** $\forall a \in A, \ (a,a) \in R.$ 
- **Symmetric:** $\forall a,b \in A, \ (a,b) \in R \implies (b,a) \in R.$ 
- **Transitive:** $\forall a,b,c \in A, \ (a,b) \in R \land (b,c) \in R \implies (a,c) \in R.$ 

We often write $a \sim b$ instead of $(a,b) \in R$.

---
### Equivalence Class

Given $a \in A$, the **equivalence class of $a$** is:
$$
[a] = \{ x \in A \mid x \sim a \}.
$$

- Each equivalence class is a **subset of $A$**.
- Two elements are in the same class iff they are related by $ \sim $.

---
### Quotient Set

The **quotient set** of $A$ by $\sim$ is the set of all equivalence classes:
$$
A / \sim = \{ [a] \mid a \in A \}.
$$

- The quotient set **is not a subset of $A$**;  
  its elements are subsets of $A$.
- Formally: $A / \sim \subseteq \mathcal{P}(A)$ (the power set of $A$).

---
### Partition of a Set

Any equivalence relation on $A$ partitions $A$ into **disjoint equivalence classes**:
$$
A = [a_1] \cup [a_2] \cup \dots, \quad [a_i] \cap [a_j] = \varnothing \text{ if } i \neq j.
$$

Conversely, any partition of $A$ defines an equivalence relation.

---
### Examples

- **Equality on $A$:** $a \sim b \iff a = b$.
- **Congruence modulo $n$:** $a \sim b \iff n \mid (a-b)$.
  - Quotient set: $\mathbb{Z}/n\mathbb{Z} = \{ [0], [1], \dots, [n-1] \}$.
  - Example:
	- **Set:** $A = \mathbb{Z}$.
	- **Relation:** $a \sim b \iff a \equiv b \pmod{2}$.
	- **Classes:**  
	  $[0] = \{\dots, -4, -2, 0, 2, 4, \dots\}$,  
	  $[1] = \{\dots, -3, -1, 1, 3, 5, \dots\}$.
	- **Quotient set:** $\mathbb{Z}/2\mathbb{Z} = \{ [0], [1] \}$.
- **Parallel lines:** Two lines are equivalent if they are parallel (same slope).
- **Fractions → rational numbers:**  
  $(a,b) \sim (c,d) \iff ad = bc$.  
  Quotient set forms $\mathbb{Q}$.
- **Vector directions:**  
  $\mathbf{v} \sim \mathbf{w} \iff \mathbf{w} = k\mathbf{v}$ with $k \neq 0$.
  Quotient set = set of all directions.

---
### Why Important

- Defines a **softer form of "sameness"** than strict equality.
- Builds **quotient structures**:  
  groups $G/H$, rings $R/I$, spaces $V/W$.
- Simplifies problems by working with **classes of objects** instead of individual elements.