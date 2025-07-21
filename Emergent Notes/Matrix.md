#theory 

Linear transformation:
	Tranformation: function -> rule or mapping that assigns each input to exactly one output
		Input: an element in a domain - set of all inputs defined
		Output: an element in a codomain - set of all outputs possible from inputs
			Image/range: subset of codomain - set of actual outputs from inputs
	Linear:
		All lines remain lines
		Origin remains fixed

Numerical representation:
	We can deduce where new vectors land: $\vec v = x \ \vec i + y \ \vec j$ 
	This 2D matrix packages the information about the linear transformation
		! We can represent any vector as a linear combinations of the basis
		 `i(1, 0)` and `j(0, 1)` -> `i(a, c)` and `j(b, d)`
		 $$
		\begin{bmatrix}
		a & b \\
		c & d
		\end{bmatrix}
		\begin{bmatrix}
		x \\
		y
		\end{bmatrix}
		=
		x
		\begin{bmatrix}
		a \\
		c
		\end{bmatrix}
		+ y
		\begin{bmatrix}
		b \\
		d
		\end{bmatrix}
		=
		\begin{bmatrix}
		ax + by \\
		cx + dy
		\end{bmatrix}
		$$
	Essentially, it is the same for matrix multiplication
		! It just means you apply 2 transformations one after another
		We apply M2 first then M1
		`i(1, 0)` and `j(0, 1)` -> `i(ae + bg, ce + dg)` and `j(af + bh, cf + dh)`
		$$
		\begin{bmatrix}
		a & b \\
		c & d
		\end{bmatrix}
		\begin{bmatrix}
		e & f \\
		g & h
		\end{bmatrix}
		=
		\begin{bmatrix}
		e \\
		g
		\end{bmatrix}
		\begin{bmatrix}
		a & b \\
		c & d
		\end{bmatrix}
		+
		\begin{bmatrix}
		f \\
		h
		\end{bmatrix}
		\begin{bmatrix}
		a & b \\
		c & d
		\end{bmatrix}
		=
		\begin{bmatrix}
		ae + bg \quad af + bh \\
		ce + dg \quad cf + dh
		\end{bmatrix}
		$$
		Note: Order matters `M1 M2` $\neq$ `M2 M1`, but group does not `(AB)C = A(BC)` 