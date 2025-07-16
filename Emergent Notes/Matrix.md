#theory 

Linear transformation:
	Tranformation: function -> rule or mapping that assigns each input to exactly one output
		Input: an element in a domain - set of all inputs defined
		Output: an element in a codomain - set of all outputs possible from inputs
			Image: subset of codomain - set of actual outputs from inputs
	Linear:
		All lines remain lines
		Origin remains fixed

Numerical representation:
	We can deduce where new vectors land: $\vec v = x \ \vec i + y \ \vec j$ 
	This 2D matrix packages the information about the linear transformation
		 `i(1, 0)` and `j(0, 1)` -> `i(a, c)` and `j(b, d)`$$
		\begin{bmatrix}
		x \\
		y
		\end{bmatrix}
		\begin{bmatrix}
		a & b \\
		c & d
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
		\end{bmatrix}$$
		