#theory 

## From [[Linear Algebra]] to Fourier & beyond

### 1. Where I am now

- I understand **linear algebra basics**: eigenvectors, determinants, and basis change.
- I have started exploring **polynomial spaces** as vector spaces.

---
### 2. Next concept: What is a Polynomial?

- A polynomial 
  $$ p(x) = a_0 + a_1 x + \dots + a_n x^n $$
  can be seen as the vector 
  $$ (a_0, a_1, \dots, a_n) \in \mathbb{R}^{n+1}. $$

- The set of all polynomials of degree $\le n$ (denoted $P_n$) forms a **finite-dimensional vector space**.

- Extending to **infinite-degree polynomials** leads to an **infinite-dimensional vector space**, where derivative and integration are **linear operators** represented by infinite matrices:
  $$ D[a_0, a_1, a_2, \dots] = [a_1, 2a_2, 3a_3, \dots]. $$

---
### 3. Derivatives and Integrals (from limits to matrices)

- **Derivative (definition):**
  $$ f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}. $$

- For monomials:
  $$ \frac{d}{dx} x^n = n x^{n-1}. $$

- **Integration (inverse operation):**
  $$ \int x^n dx = \frac{x^{n+1}}{n+1} + C. $$

- If we choose the basis $\{1, x, x^2, \dots, x^n \}$ for $P_n$,  
  the derivative is represented by the matrix:
  $$
  D = \begin{pmatrix}
  0 & 1 & 0 & 0 & \dots & 0 \\
  0 & 0 & 2 & 0 & \dots & 0 \\
  0 & 0 & 0 & 3 & \dots & 0 \\
  \vdots & \vdots & \vdots & \vdots & \ddots & \vdots \\
  0 & 0 & 0 & 0 & \dots & n
  \end{pmatrix}.
  $$

- Similarly, the indefinite integral (ignoring constants) acts as:
  $$
  I = \begin{pmatrix}
  0 & 0 & 0 & \dots & 0 \\
  1 & 0 & 0 & \dots & 0 \\
  0 & \frac{1}{2} & 0 & \dots & 0 \\
  0 & 0 & \frac{1}{3} & \dots & 0 \\
  \vdots & \vdots & \vdots & \ddots & \vdots
  \end{pmatrix}.
  $$

- This matrix viewpoint generalizes: **derivative and integral are just linear operators** acting on the coordinate vector $(a_0, a_1, \dots)$ of the polynomial.

---
### 4. Function spaces

- Polynomials are just a subset of all **functions**.
- Any space of functions (continuous, differentiable, integrable) can be treated as a **vector space**.
- Operations like differentiation, integration, and shifts are linear operators.

---
### 5. Fourier and basis change

- A function $f(x)$ can be expressed as a combination of **orthogonal basis functions**:
  $$ f(x) = \sum_{n} c_n \phi_n(x). $$
- **Fourier series** uses the basis $\{ \sin(nx), \cos(nx) \}$.
- **Fourier transform** generalizes this to a continuous basis $e^{i \omega x}$.
- **DFT/FFT** are just matrix multiplications in finite-dimensional spaces.

---
### 6. Complex numbers and trigonometry

- Complex numbers elegantly combine $\cos$ and $\sin$ via Euler's formula:
  $$ e^{i \theta} = \cos \theta + i \sin \theta. $$

- Fourier transform relies heavily on $e^{i \omega x}$ as eigenfunctions of differential operators.

---
### 7. Convolution

- Convolution is defined as:
  $$ (f * g)(x) = \int f(t) g(x - t) \, dt. $$
- In Fourier space, convolution becomes simple multiplication:
  $$ \mathcal{F}(f * g) = \mathcal{F}(f) \cdot \mathcal{F}(g). $$
- Think of convolution as a **Toeplitz matrix operator** acting on a vector.

---
### 8. Normed and Hilbert spaces

- For infinite-dimensional function spaces, we need a way to measure size and angle:
  - **Normed space (Banach space):** Has a norm $\|f\|$.
  - **Hilbert space:** A normed space with an **inner product** $(f,g)$.
- **$L^2$ space:** Functions with finite energy:
  $$ \|f\|_2 = \sqrt{\int |f(x)|^2 dx}. $$
- Fourier series arises naturally from the orthogonal basis in $L^2$.

---
### 9. Next steps

1. **Revisit limits, derivatives, and integrals:**
   - Understand the limit definition of the derivative.
   - Practice moving from definition to the power rule.
   - Visualize derivative and integral as linear maps in $P_n$.

2. **Deepen polynomial spaces:**
   - Write derivative and integral as matrices on $\{1, x, x^2, \dots\}$.
   - Explore **orthogonal polynomials** (Legendre, Chebyshev).

3. **Introduce function spaces:**
   - Think of functions as infinite-dimensional vectors.
   - Learn about **linear operators** on them.

4. **Normed & inner product spaces:**
   - Understand $\ell^2$ and $L^2$ spaces.

5. **Fourier series and transforms:**
   - See them as basis change in Hilbert spaces.

6. **Convolution and eigenfunctions:**
   - Analyze why exponentials are eigenfunctions of convolution.

7. **(Optional next)**: Laplace transform, wavelets, PDEs.

---
### 10. Key insight

Everything I learned in linear algebra **extends naturally**:

- **Vector → Function.**
- **Matrix → Linear Operator.**
- **Basis change → Fourier and other expansions.**
- **Dot product → Inner product of functions.** 