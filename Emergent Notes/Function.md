#theory 

A **function** $f: A \to B$ is a special [[Relation]] between $A$ and $B$ such that  
$$
\forall \, a \in A, \ \exists \, ! \ b \in B \ \text{with} \ (a,b) \in f.
$$
Every input $a$ has exactly one output $b$.

#### Properties

- **Injective (One-to-one)**:  
  $$
  f(a_1) = f(a_2) \implies a_1 = a_2.
  $$
  No two different elements of $A$ map to the same element of $B$.

- **Surjective (Onto)**:  
  $$
  \forall \, b \in B, \ \exists \, a \in A \ \text{such that} \ f(a) = b.
  $$
  Every element of $B$ is "hit" by $f$.

- **Bijective**:  
  $f$ is both injective and surjective.  
  Every element of $B$ corresponds to exactly one element of $A$.  
  Bijective functions are invertible.

[[Morphism]]
