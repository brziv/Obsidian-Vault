#theory 

### What is Logic?

- **Logic** is the formal study of reasoning, focusing on the structure and validity of arguments rather than their content.
- In mathematics, logic provides the foundation for proofs, definitions, and the formal language of mathematics.

---
### Core Concepts

#### Propositions

- A **proposition** is a statement that is either **true (T)** or **false (F)** (but not both).
- Example:  
  - `2 + 2 = 4` (True)  
  - `5 < 3` (False)

#### Logical Connectives

- **¬p** – NOT p (negation)  
- **p ∧ q** – p AND q (conjunction)  
- **p ∨ q** – p OR q (disjunction)  
- **p → q** – IF p THEN q (implication)  
- **p ↔ q** – p IF AND ONLY IF q (biconditional)

---
### Truth Tables
| p | q | p ∧ q | p ∨ q | p → q | p ↔ q |
|---|---|-------|-------|-------|-------|
| T | T |   T   |   T   |   T   |   T   |
| T | F |   F   |   T   |   F   |   F   |
| F | T |   F   |   T   |   T   |   F   |
| F | F |   F   |   F   |   T   |   T   |

---
### Quantifiers

- **Universal Quantifier (∀):** “for all”  
  - Example: `∀x ∈ ℝ, x² ≥ 0`.
- **Existential Quantifier (∃):** “there exists”  
  - Example: `∃x ∈ ℝ such that x² = 4`.

---
### Laws of Classical Logic

1. **Law of Identity:**  
   `p ≡ p` — Every proposition is identical to itself.

2. **Law of Non-Contradiction:**  
   `¬(p ∧ ¬p)` — A proposition cannot be both true and false at the same time.

3. **Law of Excluded Middle:**  
   `p ∨ ¬p` — Every proposition is either true or false.

4. **Double Negation:**  
   `¬(¬p) ≡ p`.

5. **Principle of Bivalence:**  
   Every proposition has exactly one truth value: true or false.

---
### Logical Equivalence

- Two propositions are **logically equivalent** if they have the same truth value in every situation.  
- Examples:
  - `p → q ≡ ¬p ∨ q`
  - **De Morgan’s Laws:**  
    - `¬(p ∧ q) ≡ ¬p ∨ ¬q`
    - `¬(p ∨ q) ≡ ¬p ∧ ¬q`

---
### Proof Techniques

- **Direct Proof:** Start from assumptions and derive conclusion step by step.
- **Proof by Contradiction:** Assume the negation of the statement and derive a contradiction.
- **Contrapositive:** `p → q` is equivalent to `¬q → ¬p`.
- **Induction:** Prove base case, assume for n, then prove for n+1.

---
### Logic vs. Set Theory

- Logic and set theory form the foundational language of mathematics.  
- Logical operations often correspond to set operations:
  - AND ↔ Intersection (∩)
  - OR ↔ Union (∪)
  - NOT ↔ Complement (ᶜ)

---
### Non-Classical Logics

- **Intuitionistic Logic:** Rejects `p ∨ ¬p` as a universal truth (law of excluded middle). Truth must be *constructively* demonstrated.
- **Multi-Valued Logic:** Allows more than 2 truth values (e.g., `T`, `F`, `U` for unknown).
- **Modal Logic:** Adds operators for *necessity* (□p = "p is necessarily true") and *possibility* (◇p = "p is possibly true").
- **Paraconsistent Logic:** Allows contradictions without implying every statement is true (avoids “explosion”).
- **Fuzzy Logic:** Truth values range continuously between 0 and 1.

---
### Notes

- Logic is not about “truth” in the philosophical sense but **validity of reasoning**.
- All higher mathematics relies on logical structures.