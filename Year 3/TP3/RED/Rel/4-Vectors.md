In Euclidean space, a transformation between two coordinate systems $(x,y,z)$ and $(x',y',z')$ is given by:
$$\begin{bmatrix}
x' \\
y' \\
z'
\end{bmatrix}=\begin{bmatrix}
\frac{\partial x'}{\partial x} & \frac{\partial x'}{\partial y} & \frac{\partial x'}{\partial z} \\
\frac{\partial y'}{\partial x} & \frac{\partial y'}{\partial y} & \frac{\partial y'}{\partial z} \\
\frac{\partial z'}{\partial x} & \frac{\partial z'}{\partial y} & \frac{\partial z'}{\partial z}
\end{bmatrix}\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}.$$
Example, a rotation around the $z$ axis is represented by
$$\begin{bmatrix}
x' \\
y' \\
z'
\end{bmatrix}=\begin{bmatrix}
\cos \alpha & \sin \alpha & 0 \\
-\sin \alpha & \cos \alpha & 0 \\
0 & 0 & 1
\end{bmatrix}\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}.$$
For a [Lorentz transform](Lorentz%20Transforms.md) we have 4 dimensions, three space and one time so we extend the vectors and matrices into 4 dimensions, with the same logic.

The Lorentz transform for two frames moving away from each other parallel to the $x$ axis is given by $\Lambda$:
$$\underline{\underline{\Lambda}}=\begin{bmatrix}
\gamma & -\gamma \beta & 0 & 0 \\
-\gamma \beta & \gamma & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}.$$
This is of similar form of the rotation matrix, which can be shown be defining $\beta=\tanh \phi$, $\gamma \beta=\sinh \phi$ and $\gamma=\cosh \phi$.
$$\underline{\underline{\Lambda}}=\begin{bmatrix}
\cosh \phi & -\sinh \phi & 0 & 0 \\
-\sinh \phi & \cosh \phi & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}.$$
This gives the transform $\underline{x}'=\underline{\underline{\Lambda}}\underline{x}'$.