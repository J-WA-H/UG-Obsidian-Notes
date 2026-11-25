If $\{\underline{e}_{1}, \underline{e}_{2},\dots,\underline{e}_{n}\}$ is a linearly independent set of unit vectors in $E$ we can decompose any vector in this [vector space](Vector%20Spaces.md) as a linear combination of the elements in this orthonormal basis
$$\underline{x}=\sum_{i=1}^{n}x_{i}\underline{e}_{i}.$$
$x_{i}$ are the coordinates of vector $\underline{x}$ in the basis defined by $\{\underline{e}_{i}\}$.

This can be defined as a matrix equation
$$\underline{x}=\begin{bmatrix}
\underline{e}_{1} & \underline{e}_{2} & \dots & \underline{e}_{n}
\end{bmatrix}\begin{bmatrix}
x_{1} \\
x_{2} \\
\vdots \\
x_{n}
\end{bmatrix}.$$
Properties of matrices:
Symmetric matrices: $\underline{\underline{A}}=\underline{\underline{A}}^T$
Skew-symmetric matrices: $\underline{\underline{A}}=-\underline{\underline{A}}^T$
Inverse: $\underline{\underline{A}}\underline{\underline{A}}^{-1}=\mathbb{I}$
$$\mathbb{I}=\begin{bmatrix}
1 & 0 & \dots & 0 \\
0 & 1 & \dots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \dots & 1
\end{bmatrix}$$
Trace of a matrix: $\text{Tr}(A)=\sum_{i}a_{ii}$.
