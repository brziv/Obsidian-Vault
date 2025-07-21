#theory 

A **relation** $R$ on a set $A$ is a subset of $A \times A$.  
We write $aRb$ if $(a,b) \in R$.

#### Properties

- **Reflexive**: $R$ is reflexive if  
  $$
  \forall a \in A, \ (a,a) \in R.
  $$
  Example: The relation $\le$ on real numbers is reflexive.

- **Symmetric**: $R$ is symmetric if  
  $$
  \forall a,b \in A, \ (a,b) \in R \implies (b,a) \in R.
  $$
  Example: "is a sibling of" is symmetric.

- **Transitive**: $R$ is transitive if  
  $$
  \forall a,b,c \in A, \ (a,b) \in R \wedge (b,c) \in R \implies (a,c) \in R.
  $$
  Example: $\le$ on real numbers is transitive.