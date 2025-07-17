#theory

The area "scaling" factor of a transformation.
	It actually measures:
		The area of the parallelogram (2D) relative to the unit square formed by `i` and `j`
		-> 3D: volume of the parallelepiped relative to the unit cube formed by `i`, `j`, `k`
			-> n-dimensional:  signed volume scaling factor of the image of the unit hypercube
		The orientation of the space or basis -> `-` means reversal
	The absolute value (`number`) tells the factor
	The sign (`+ -`) tells the orientation
		$$
		\det\!
		\left(
		\begin{bmatrix}
		a & b \\
		c & d
		\end{bmatrix}
		\right)
		=
		(a+b) (c+d) - ac - bd - 2bc
		=
		ad - bc
		$$
		![[2d_det.png]]
		$$
		\det\!
		\left(
		\begin{bmatrix}
		a & b & c \\
		d & e & f \\
		g & h & i
		\end{bmatrix}
		\right)
		=
		a \
		\det\!
		\left(
		\begin{bmatrix}
		e & f \\
		h & i
		\end{bmatrix}
		\right)
		-
		b \
		\det\!
		\left(
		\begin{bmatrix}
		d & f \\
		g & i
		\end{bmatrix}
		\right)
		+
		c \
		\det\!
		\left(
		\begin{bmatrix}
		d & e \\
		g & h
		\end{bmatrix}
		\right)
		$$ 