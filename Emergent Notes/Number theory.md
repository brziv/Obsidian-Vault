#theory 

The study of integers and their properties.

- Focuses on **divisibility**, **prime numbers**, **congruences**, and **arithmetic functions**.
- Known as the “Queen of Mathematics” (Gauss).

---
### Core Concepts

#### Divisibility
- $a \mid b$ means **a divides b** (there exists an integer $k$ such that $b = ak$).
- **Greatest Common Divisor (GCD):** Largest integer dividing both $a$ and $b$.
  - Euclidean Algorithm is the fastest way to compute GCD.
- **Least Common Multiple (LCM):** Smallest positive integer divisible by both $a$ and $b$.
  - Relation: $\mathrm{gcd}(a,b) \cdot \mathrm{lcm}(a,b) = |ab|$.

#### Prime Numbers
- **Prime:** Integer $p > 1$ with no divisors other than 1 and $p$.
- **Composite:** Integer $n > 1$ that is not prime.
- **Fundamental Theorem of Arithmetic:** Every $n > 1$ is uniquely factored into primes.

---
### Modular Arithmetic

- $a \equiv b \ (\mathrm{mod}\ m)$ means $m \mid (a - b)$.
- **Properties:**
  - $(a + b) \bmod m = (a \bmod m + b \bmod m) \bmod m$.
  - $(a \cdot b) \bmod m = (a \bmod m \cdot b \bmod m) \bmod m$.
- **Modular Inverse:** $a^{-1} \ (\mathrm{mod}\ m)$ is an integer $x$ such that $ax \equiv 1 \ (\mathrm{mod}\ m)$, exists if $\gcd(a, m) = 1$.

---
### Congruences and Theorems

- **Fermat's Little Theorem:**  
  If $p$ is prime and $a \not\equiv 0 \ (\mathrm{mod}\ p)$, then  
  $$ a^{p-1} \equiv 1 \ (\mathrm{mod}\ p). $$
- **Euler's Theorem:**  
  If $\gcd(a, n) = 1$, then  
  $$ a^{\varphi(n)} \equiv 1 \ (\mathrm{mod}\ n), $$  
  where $\varphi(n)$ = Euler's totient function.
- **Chinese Remainder Theorem (CRT):**  
  A system of congruences  
  $$ x \equiv a_i \ (\mathrm{mod}\ m_i) $$  
  has a unique solution modulo $M = m_1 m_2 \cdots m_k$ if the $m_i$ are pairwise coprime.

---
### Arithmetic Functions

- **Euler’s Totient Function:**  
  $\varphi(n) =$ number of integers $\le n$ that are coprime to $n$.
- **Divisor Function:**  
  $d(n) =$ number of positive divisors of $n$.
- **Sum of Divisors:**  
  $\sigma(n) =$ sum of positive divisors of $n$.

---
### Diophantine Equations

- **Linear Diophantine Equation:** $ax + by = c$ has integer solutions iff $\gcd(a, b) \mid c$.
- Famous examples: **Pell’s Equation**, **Pythagorean Triples** $x^2 + y^2 = z^2$.

---
### Important Problems

- Distribution of primes (Prime Number Theorem).
- Perfect numbers (e.g., 6, 28).
- Fermat’s Last Theorem: $x^n + y^n = z^n$ has no non-trivial solutions for $n > 2$.
- Twin primes conjecture (infinitely many primes $p, p+2$?).

---
### Notes

- Number theory blends **algebra**, **combinatorics**, and **analysis**.
- Key computational tools: **Euclidean algorithm**, **modular exponentiation**, **sieve of Eratosthenes**.
