#theory 

### 0. Foundational Vocabulary

- **Primitive concept:** Taken as given; not defined inside the system.  
- **Axiom:** Rule you *stipulate* about primitives; starting truths of the game.  
- **Logic:** Allowed moves for deriving consequences from axioms.  
- **Definition:** New shorthand built from old terms; no new content, just naming.  
- **Proof:** Finite sequence of justified steps from axioms by logic.  
- **Theorem:** Any statement you can prove from the axioms.  
- **Model:** Interpretation where all axioms come out true.  
- **Consistency:** No contradictions; equivalently, at least one model (semantic).  
- **Soundness:** Provable ⇒ true in every model.  
- **Completeness (logic-level):** True in every model ⇒ provable.  
- **Independence:** Statement neither provable nor refutable (if system consistent).

---
### 1. Peano axioms

**Primitives:** `0`, `S(x)` (successor), equality `=`; later define `+`, `×`, etc.

**Core Axioms**:

| Tag    | Core Idea                                  | Why You Need It (What breaks if absent?) | Mnemonic         |
|--------|--------------------------------------------|------------------------------------------|------------------|
| Seed   | There exists 0.                            | No starting number.                      | “Start.”         |
| Step   | Every number has a successor.              | Stops growth; no chain.                  | “Next.”          |
| No-Back| 0 isn’t successor of any number.           | Looping back could collapse chain.       | “No wrap.”       |
| Inject | Equal successors ⇒ equal predecessors.     | Prevents merging branches; keeps chain 1-way. | “Distinct stays distinct.” |
| Induct | If a property holds for 0 and passes to successors, it holds for all. | Can’t prove general facts like `n+0=n`. | “Climb forever.” |

---
### 2. Hilbert’s axioms

**Primitives:** point, line, plane; relations: incidence (“lies on”), betweenness, congruence.

Hilbert grouped axioms into *blocks*. Remember the *story of building space*:

| Block          | Core Idea                                  | Minimal Memory            | If Missing…                  |
|----------------|--------------------------------------------|---------------------------|------------------------------|
| **I. Incidence** | Which points lie on which lines/planes; two points determine a unique line; enough points exist. | “Who touches what.”         | Geometry can’t even draw lines correctly. |
| **II. Order**   | A notion of one point between two others; linear order on lines. | “In what order.”            | No notion of segments or intervals. |
| **III. Congruence** | Copy/compare lengths & angles; transport segments rigidly. | “How big / same shape.”     | No measurement; triangles meaningless. |
| **IV. Parallels** | Euclidean parallel postulate (one parallel through a point). | “Parallel behavior.”        | Could drift into non-Euclidean worlds. |
| **V. Continuity** | No gaps; lines behave like the real number line (completeness). | “No gaps.”                  | Fragmented or Archimedean failures. |

---
### 3. ZF set theory

**Primitives:** *set*, *membership* `∈` (everything is a set; elements are sets too).

| Axiom              | Core Idea                                                 | Role / What It Ensures                                               | Mnemonic                   |
| ------------------ | --------------------------------------------------------- | -------------------------------------------------------------------- | -------------------------- |
| **Extensionality** | Sets equal if same members.                               | Identity by contents; no hidden tags.                                | “Same insides = same set.” |
| **Empty Set**      | There exists a set with no members.                       | Gives you ∅; base object.                                            | “Nothing exists.”          |
| **Pairing**        | From a,b build {a,b}.                                     | Lets you make 2-element sets; basis for ordered pairs.               | “Make pairs.”              |
| **Union**          | From A get ⋃A.                                            | Flatten a collection-of-sets one level; collect elements.            | “Flatten.”                 |
| **Power Set**      | For any A, set of all subsets exists.                     | Builds big combinatorial universes; functions as subsets of product. | “All sub-sets.”            |
| **Infinity**       | A set containing ∅ and closed under successor exists.     | Ensures an inductive set; anchors ℕ.                                 | “Natural numbers live.”    |
| **Separation**     | Subset of a set by a property.                            | Safe comprehension; blocks paradoxes.                                | “Slice safely.”            |
| **Replacement**    | Image of a set under a definable function is a set.       | Build large transfinite sequences.                                   | “Map images exist.”        |
| **Foundation**     | Every nonempty set has an ∈-minimal element; no ∈-cycles. | Enforces well-founded membership.                                    | “No loops down.”           |
| **Choice** (ZFC)   | Choose an element from each of many nonempty sets.        | Supports product constructions, bases, etc.                          | “Pick everywhere.”         |
