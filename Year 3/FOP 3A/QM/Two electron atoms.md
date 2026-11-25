For a single electron bound atom.
$$V(r)=-\frac{Ze^2}{4\pi\varepsilon_{0}r}$$
and for a molecule with multiple nuclei
$$V(r)=-\frac{e^2}{4\pi\varepsilon_{0}} \sum_{n} \frac{Z_{n}}{\lvert \underline{r}-\underline{R}_{n} \rvert }$$
where $\underline{R}_{n}$ is the position of the nuclei.
The Schrodinger equation for this system is
$$\left[ -\frac{\hbar^2}{2m}\nabla^2+V(r) \right]\psi_{i}(r)=\epsilon_{i}\psi_{i}(\underline{r}).$$
As this equation is in terms of spatial coordinates, the spin component will remain unchanged when passed through the Hamiltonian.
$$\hat{H}\psi_{i}\alpha(\sigma)=\epsilon_{i}\psi_{i}\alpha(\sigma)$$
$$\hat{H}\psi_{i}\beta(\sigma)=\epsilon_{i}\psi_{i}\beta(\sigma).$$
The total Hamiltonian for a two particle system is
$$\hat{H}=\hat{h}(\underline{r},\underline{p})+\hat{h}(\underline{r}',\underline{p}')=\left[ -\frac{\hbar^2}{2m}\nabla^2+V(r)-\frac{\hbar^2}{2m}\nabla'^2+V(r') \right].$$
Applying this Hamiltonian gives:
$$\hat{H}\psi_{i}(\underline{r},\sigma)\psi_{j}(\underline{r}',\sigma')=(\epsilon_{i}+\epsilon_{j})\psi_{i}(\underline{r},\sigma)\psi_{j}(\underline{r}',\sigma').$$
$$\hat{H}\psi_{i}(\underline{r}',\sigma')\psi_{j}(\underline{r},\sigma)=(\epsilon_{i}+\epsilon_{j})\psi_{i}(\underline{r}',\sigma')\psi_{j}(\underline{r},\sigma).$$
As both of these wavefunctions give the same energy level, this energy level is degenerate so the difference between them will also satisfy the Schrodinger equation, giving an antisymmetric wavefunction
$$[\hat{h}+\hat{h}']\left[ \frac{1}{\sqrt{ 2 }}(\psi_{i}(\underline{r}))\chi_{i}(\sigma)\psi_{j}(\underline{r}')\chi_{j}(\sigma')-\psi_{j}(\underline{r})\chi_{j}(\sigma)\psi_{i}(\underline{r}')\chi_{i}(\sigma) \right]$$$$=(\epsilon_{i}+\epsilon_{2})\left[ \frac{1}{\sqrt{ 2 }}(\psi_{i}(\underline{r})\chi_{i}(\sigma)\psi_{j}(\underline{r}')\chi_{j}(\sigma')-\psi_{j}(\underline{r})\chi_{j}(\sigma)\psi_{i}(\underline{r}')\chi_{i}(\sigma)) \right]$$
This wavefunction can be rewritten as a determinant
$$\Psi(\underline{r},\sigma;\underline{r}',\sigma')=\frac{1}{\sqrt{ 2 }}\begin{vmatrix}
\psi_{i}(\underline{r})\chi_{i}(\sigma) & \psi_{i}(\underline{r}')\chi_{i}(\sigma') \\
\psi_{j}(\underline{r})\chi_{j}(\sigma) & \psi_{j}(\underline{r}')\chi_{j}(\sigma')
\end{vmatrix}.$$
These determinants are known as **Slater determinants** that describe the wavefunctions of a multi electron system, making sure it obeys the Pauli exclusion principle and the antisymmetric requirement for fermions.

For an N-electron system this can be generalised to
$$\Psi(\underline{r},\sigma;\underline{r}',\sigma';\dots ;\underline{r}''',\sigma''')=\frac{1}{\sqrt{ 2 }}\begin{vmatrix}
\psi_{1}(\underline{r})\chi_{1}(\sigma) & \dots & \psi_{1}(\underline{r}''')\chi_{1}(\sigma''') \\
\vdots  & \ddots & \vdots\\
\psi_{N}(\underline{r})\chi_{N}(\sigma) & \dots &  \psi_{N}(\underline{r}''')\chi_{N}(\sigma''')
\end{vmatrix}.$$
