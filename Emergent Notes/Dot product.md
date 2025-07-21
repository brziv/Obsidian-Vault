#theory 

$$
\vec a \ \cdot \vec b
=
\begin{bmatrix}
a_1 \\ a_2
\end{bmatrix}
.
\begin{bmatrix}
b_1 \\ b_2
\end{bmatrix}
=
a_1b_1 + a_2b_2
$$
	$\vec a \ \cdot \vec b =$  $\|$projected $\vec a$ on $\vec b \|$ . $\|\vec b\|$ 
		= $\|\vec{a}\| \; \|\vec{b}\| \cos \theta$ 
			`-` if pointing oppositely
			 0 if perpendicular

Linear transformation from 2D (plane) to 1D (line):
$$
\vec{a} \cdot \vec{b} = 
\begin{bmatrix} a_1 & a_2\end{bmatrix}
\begin{bmatrix} b_1 \\ b_2\end{bmatrix}
$$
	$\begin{bmatrix}  a_1 & a_2 \end{bmatrix}$ : $\mathbb{R}^2 \rightarrow \mathbb{R}$  
	2d vector $\leftrightarrow$ 1x2 matrix
		dot product $\leftrightarrow$ matrix multiplication

Duality:  $\langle \phi, v \rangle = \phi(v)$ 
	A vector is an arrow in space with direction and magnitude:
		$\vec{v} = \begin{pmatrix} x \\ y \end{pmatrix}$ 
	A matrix transforms a vector, moving it in space:  
		$v' = A v, \qquad A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ 
	A covector is a linear map that takes a vector and produces a scalar:
$$\phi = \begin{pmatrix} \alpha & \beta \end{pmatrix}, \qquad
\phi(v) = 
\begin{pmatrix} \alpha & \beta \end{pmatrix}
\begin{pmatrix} x \\ y \end{pmatrix}
= \alpha x + \beta y$$
		Geometry: it defines a family of parallel lines (2D) or planes (3D)
					$\alpha x + \beta y = c$  
	A transpose transforms a covector, moving it in dual space. For any vector $v$,  
		$\langle \phi', v \rangle = \langle \phi, A v \rangle$ 
	This implies:  
		$\phi' = \phi A, \qquad \text{or equivalently} \qquad \phi'^\top = A^\top \phi^\top$ 
	The duality condition is preserved:  
		$\langle A^\top \phi, v \rangle = \langle \phi, A v \rangle$ 
