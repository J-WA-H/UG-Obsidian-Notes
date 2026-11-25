A vector is independent of coordinate system, but the coordinates are not.
For $\underline{e}'$ - a new [basis](Basis%20of%20Vectors.md) of eigenvectors - the coordinates satisfy
$$\underline{x}=x_{1}\underline{e}'_{1}+x_{2}\underline{e}'_{2}+\dots+x_{n}\underline{e}'_{n}.$$
The two bases are linked by a set of coefficients $S_{i}^{j}$:
$$\underline{e}_{1}'=e_{1}S_{1}^{1}+\underline{e}_{2}S_{1}^{2}+\dots+\underline{e}_{n}S_{1}^n$$
More generally
$$\underline{e}'_{i}=\sum_{j=1}^{n}\underline{e}_{j}S_{i}^{j}.$$
As a matrix equation this becomes
$$\underline{e}'=\begin{bmatrix}
\underline{e}_{1} & \underline{e}_{2} & \dots & \underline{e}_{n} 
\end{bmatrix}\begin{bmatrix}
S_{1}^{1} & S^{1}_{2} & \dots  & S_{n}^{1} \\
\vdots & \vdots  & \ddots & \vdots \\
S_{1}^{n} & S_{2}^{n} & \dots & S^{n}_{n} 
\end{bmatrix}$$
$$\underline{x}=\sum_{i=1}^{n}\underline{e}_{i}'\underline{x}'_{i}=\sum_{i=1}^{n}\left( \sum_{j=1}^{n}\underline{e}_{j}S_{i}^{j} \right)\underline{x}'_{i}=\sum_{j=1}^{n}\underline{e}_{j}\underline{x}_{j}.$$
$$\underline{x}_{j}=\sum_{i=1}^{n}S_{i}^{j}x_{ij}$$
$$\begin{bmatrix}
x_{1} \\
x_{2} \\
\vdots \\
x_{n}
\end{bmatrix}=\begin{bmatrix}
S_{1}^{1} & S^{1}_{2} & \dots  & S_{n}^{1} \\
S_{1}^{2} & S_{2}^{2} & \dots & S_{n}^{2} \\
\vdots & \vdots  & \ddots & \vdots \\
S_{1}^{n} & S_{2}^{n} & \dots & S^{n}_{n} 
\end{bmatrix}\begin{bmatrix}
x_{1}' \\
x_{2}' \\
\vdots \\
x_{4}'
\end{bmatrix}.$$
We can also take the inverse of this matrix to give the relation between $x'$ and $x$.
$$\begin{bmatrix}
x'_{1} \\
x'_{2} \\
\vdots \\
x'_{n}
\end{bmatrix}=\begin{bmatrix}
R_{1}^{1} & R^{1}_{2} & \dots  & R_{n}^{1} \\
R_{1}^{2} & R_{2}^{2} & \dots & R_{n}^{2} \\
\vdots & \vdots  & \ddots & \vdots \\
R_{1}^{n} & R_{2}^{n} & \dots & R^{n}_{n} 
\end{bmatrix}\begin{bmatrix}
x_{1} \\
x_{2} \\
\vdots \\
x_{4}
\end{bmatrix}.$$
