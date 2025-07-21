#theory 

Computation (for computers):
	Gaussian elimination
	Row echelon form

Intuition (for human):
	Equations: variables, constants
	$$
	\begin{aligned}
	a_{11} \ x_1 + a_{12} \ x_2 + a_{13} \ x_3 &= b_1 \\
	a_{21} \ x_1 + a_{22} \ x_2 + a_{23} \ x_3 &= b_2 \\
	a_{31} \ x_1 + a_{32} \ x_2 + a_{33} \ x_3 &= b_3
	\end{aligned}
	$$
	Vector equation: $A x = b$ 
		A: coefficient matrix -> the transformation
		x: variable vector -> the initial vector
		b: constant vector -> the result vector
	$$
	\begin{bmatrix}
	a_{11} \; a_{12} \; a_{13} \\
	a_{21} \; a_{22} \; a_{23} \\
	a_{31} \; a_{32} \; a_{33}
	\end{bmatrix}
	\begin{bmatrix}
	x_1 \\ x_2 \\ x_3
	\end{bmatrix}
	=
	\begin{bmatrix}
	b_1 \\ b_2 \\ b_3
	\end{bmatrix}
	$$
		$\det\! \left( A \right) \neq 0$ : $A^{-1} A \, x = A^{-1} \ v \Rightarrow x = A^{-1} \ b$ 
			Inverse matrix: reverse the effect
				 $A^{-1} A$ = 1
		$\det\! \left( A \right) = 0$ :
			Lower dimension, lose information
				-> a function cannot recover -> no $A^{-1}$ 
				Solution still exists if the vector land on the column space
			Column space: span of the columns
			-> Set of all possible outputs $A \, x$ -> image
				Rank: number of dimensions in the column space
				Full rank: rank = number of columns
				Null space (kernel): set of vectors that land on the origin/zero vector