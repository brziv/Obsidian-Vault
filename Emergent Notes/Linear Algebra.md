#theory 

[[Vector]]
[[Matrix]]
[[Determinant]]
[[System of linear equations]]
[[Dot product]]
[[Cross product]]
[[Cramer's rule]]
[[Change of basis]]
[[Eigenvector]]
[[Vector space]]

Linear algebra is not just computation—it’s **seeing the hidden structure of change**.  
After walking through 3Blue1Brown’s journey, these truths remain like echoes:


**1. Determinant = Volume of Change**  
When it’s zero, dimensions collapse — information is lost forever.  

$$
\det A = 0 \Leftrightarrow A \text{ not invertible.}
$$

**2. Rank = True Dimension**  
How many dimensions survive the transformation? Rank whispers the answer.  

$$
\mathrm{rank}(A) = \dim(\mathrm{Col}(A)).
$$

**3. Dot Product = Alignment**  
A dialogue between directions — “how much of me is with you?”  

$$
u \cdot v = \|u\|\|v\|\cos \theta.
$$

**4. Duality = Rows vs Columns**  
Questions vs answers, observers vs actors — two sides of the same map.  

$$
\mathrm{Row}(A) = \mathrm{Col}(A^{T}).
$$

**5. Scalar Triple Product = Space Warping**  
Determinant, dot, and cross interweave — measuring how 3D space bends.  

$$
u \cdot (v \times w) = \det [u \ v \ w].
$$

**6. Eigenvectors = Calm Amidst Chaos**  
The directions that remain unmoved, only stretched by their eigenvalues.  

$$
A v = \lambda v.
$$

**7. Diagonalization = God’s Eyes**  
Step into the eigen-world, see pure scalings, then return with answers.  

$$
A = P D P^{-1}.
$$

**8. Spectral Theorem = Perfect Alignment**  
For symmetric transformations, the eigen-world is orthogonal — nature loves clean axes.  

$$
A = Q \Lambda Q^{T}, \quad A = A^{T}.
$$

**9. SVD = The Ultimate Dissection**  
Any transformation, even without eigenvectors, is just rotate → stretch → rotate.  

$$
A = U \Sigma V^{T}.
$$

**10. Pseudoinverse = Resurrection of Lost Dimensions**  
What cannot be reversed is reimagined — the closest echo of the original world.  

$$
A^{+} = V \Sigma^{+} U^{T}.
$$
