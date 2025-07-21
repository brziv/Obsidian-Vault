#theory 

### Axioms

$$
\textbf{1. Extensionality:} \ 
\forall A \, \forall B \, [ \forall x (x \in A \iff x \in B) \implies A = B ].
$$

$$
\textbf{2. Empty Set:} \ 
\exists A \, \forall x (x \notin A), \ \text{denoted} \ \varnothing.
$$

$$
\textbf{3. Pairing:} \ 
\forall a \, \forall b \, \exists A \, \forall x (x \in A \iff x = a \lor x = b).
$$

$$
\textbf{4. Union:} \ 
\forall A \, \exists U \, \forall x \, [ x \in U \iff \exists B (x \in B \land B \in A) ].
$$

$$
\textbf{5. Power Set:} \ 
\forall A \, \exists P \, \forall x \, [ x \in P \iff x \subseteq A ].
$$

$$
\textbf{6. Infinity:} \ 
\exists I [ \varnothing \in I \land \forall x (x \in I \implies x \cup \{x\} \in I) ].
$$

$$
\textbf{7. Separation:} \ 
\forall A \, \exists B \, \forall x (x \in B \iff x \in A \land P(x)).
$$

$$
\textbf{8. Replacement:} \ 
\forall A \, [ \forall x \in A \, \exists ! y \, P(x,y) ] \implies
\exists B \, \forall y (y \in B \iff \exists x \in A \, P(x,y)).
$$

$$
\textbf{9. Foundation:} \ 
\forall A [ A \neq \varnothing \implies \exists x \in A (x \cap A = \varnothing) ].
$$

$$
\textbf{10. Choice (AC):} \ 
\forall \mathcal{F} [ \mathcal{F} \neq \varnothing \land
\forall A \in \mathcal{F} (A \neq \varnothing) \implies
\exists f : \mathcal{F} \to \bigcup \mathcal{F}, \ f(A) \in A ].
$$

---
### Consequences

$$
0 = \varnothing, \quad 1 = \{0\}, \quad 2 = \{0,1\}, \dots
$$

$$
(a,b) = \{ \{a\}, \{a,b\} \}.
$$

$$
|A| < |\mathcal{P}(A)| \quad \text{(Cantor’s theorem)}.
$$

$$
V_0 = \varnothing, \quad V_{\alpha+1} = \mathcal{P}(V_\alpha),
\quad V_\lambda = \bigcup_{\alpha < \lambda} V_\alpha.
$$
