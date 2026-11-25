The rising/lowering spin operators are similar to that of the [orbital angular momentum](Hydrogen%20atom%20and%20Angular%20Momentum.md) operators
$$\hat{S}^2\ket{s,m}=s(s+1)\hbar^2\ket{s,m}$$
$$\hat{S}_{z}\ket{s,m} = m\hbar \ket{s,m}$$
##### Special case s=$1/2$
In this case, $m=\pm \frac{1}{2}$, where the $m=\frac{1}{2}$ state is the spin up state and $m=-\frac{1}{2}$ state is the spin down state.
$$\ket{\uparrow} = \ket{\frac{1}{2}, \frac{1}{2}}=\ket{\alpha}=\begin{bmatrix}
1 \\
0
\end{bmatrix}$$
$$\ket{\downarrow}=\ket{\frac{1}{2}, \frac{1}{2}} =\ket{\beta}=\begin{bmatrix}
0 \\
1
\end{bmatrix}.
$$
These spin operators for $s=\frac{1}{2}$ can be represented matrices
$$\hat{S}_{x}=\frac{\hbar}{2}\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}, \;\hat{S}_{y}=\frac{\hbar}{2} \begin{bmatrix}
0 & -i \\
i & 0
\end{bmatrix}, \;\hat{S}_{z}=\frac{\hbar}{2}\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}$$
Using these we can define the ladder operators:
$$\hat{S}_{+}=\hat{S}_{x}+i\hat{S}_{y}=\frac{\hbar}{2}\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}+i\frac{\hbar}{2}\begin{bmatrix}
0 & -i \\
i & 0
\end{bmatrix}=\hbar\begin{bmatrix}
0 & 1 \\
0 & 0
\end{bmatrix}$$
Similarly,
$$\hat{S}_{-}=\hbar \begin{bmatrix}
0 & 0 \\
1 & 0
\end{bmatrix}.$$
The ladder operators flip the spin of the particle.