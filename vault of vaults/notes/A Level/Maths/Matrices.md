An $m \times n$ matrix is a rectangular array with $m$ rows and $n$ columns.

Let
$$
M = 
	\left ({\begin{array}{cc}
		1 & 4 \\
		2 & 3 \\
	\end{array}} \right)
$$
$M_{i,j}$ refers to the entry in the $i^\textup{th}$ row and the $j^\textup{th}$ column.
There are some special matrices, being the zero and identity matrices, which are
$$
O =
	\left ({\begin{array}{ccc}
		0 & \ldots & 0 \\
		\vdots & \ddots & \vdots \\
		0 & \ldots & 0 \\
		\end{array}} \right)
$$
$$
I =
	\left ({\begin{array}{ccc}
		1 & \ldots & 0 \\
		\vdots & \ddots & \vdots \\
		0 & \ldots & 1 \\
		\end{array}} \right)
$$
The zero matrix can have any number of rows and columns whereas the identity matrix must be a square matrix.

Matrices have different rules of operation to normal numbers:
For $A,\, B,\, C \in \mathbb{R}^{m \times n},\, \lambda,\, \mu \in \mathbb{R}:$
$$
A + O = O + A = A
$$
$$
A + B = B + A % addition is commutative
$$
$$
(A + B) + C = A + (B + C) % addition is associative
$$
$$
\lambda(\mu A) = (\lambda \mu)A
$$
$$
(\lambda + \mu)A = \lambda A + \mu A
$$
$$
\lambda(A + B) = \lambda A + \lambda B
$$
# Linear transformations
Let 