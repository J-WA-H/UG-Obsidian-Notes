The wavefunction that contains both spatial and [spin](Spin.md) information is given by
$$\psi(\underline{r})\ket{\alpha} \text{ or } \psi(\underline{r})\ket{\beta}.$$
Calculate norm to check to make sure this is normalised.
$$\int d^3r\lvert \psi(\underline{r}) \rvert^2\braket{ \alpha | \alpha }$$
$$\braket{ \alpha | \alpha } =\begin{bmatrix}
1 & 0
\end{bmatrix}\begin{bmatrix}
1 \\
0
\end{bmatrix}=1.$$
This simplifies the norm to
$$\int d^3r\lvert \psi(\underline{r}) \rvert ^2=1$$
if $\psi(\underline{r})$ is normalised.
For example, a [2 electron wavefunction](Two%20Particle%20Systems.md) with spin is given by
$$\psi(\underline{r}.\sigma;\underline{r}',\sigma')=\frac{1}{\sqrt{ 2 }}[\psi_{i}(\underline{r})\alpha(\sigma)\psi_{j}(\underline{r}')\beta(\sigma')-\psi_{i}(\underline{r}')\alpha(\sigma')\psi_{j}(\underline{r})\beta(\sigma)].$$
In the hand written notes for lecture 9 it is shown that the norm of this is 1, assuming $\psi_{i}$, $\psi_{j}$ are normalised.
