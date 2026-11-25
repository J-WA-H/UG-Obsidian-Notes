For the ground state of this system, the minimum energy is $E=2\epsilon_{1}$ so $i=j=1$ - suggesting that the spatial components of $\psi_i$, $\psi_{j}$ are the same. To obey Pauli's exclusion principle, the spins must be opposite. $\chi_{i}(\sigma)=\alpha(\sigma)$, $\chi_{j}(\sigma)=\beta(\sigma)$.

The wavefunction of this state can be written as a [Slater determinant](Two%20electron%20atoms.md):
$$\Psi_{11}(\underline{r},\sigma;\underline{r}',\sigma')=\frac{1}{\sqrt{ 2 }}\begin{vmatrix}
\psi_{1}(\underline{r})\alpha(\sigma) & \psi_{1}(\underline{r}')\alpha(\sigma') \\
\psi_{1}(\underline{r})\beta(\sigma) & \psi_{1}(\underline{r}')\beta(\sigma')
\end{vmatrix}.$$
We can simplify this by taking out a factor of $\psi_{1}(\underline{r})\psi_{1}(\underline{r}')$:
$$\Psi_{11}(\underline{r},\sigma ;\underline{r}',\sigma')=\frac{1}{\sqrt{ 2 }}\psi_{1}(\underline{r})\psi_{1}(\underline{r}')\begin{vmatrix}
\alpha(\sigma) & \alpha(\sigma') \\
\beta(\sigma) & \beta(\sigma')
\end{vmatrix}.$$
The value of this determinant of the spin states is equivalent to the $\ket{S=0,M=0}$ [singlet state](Measuring%202%20spin-half%20particles.md).

The first excited state has energy $E=\epsilon_{1}+\epsilon_{2}$ so $i=1,j=2$. Since the spatial components aren't in the same state, the spin states can be the same.
First consider two up spins:
$$\Psi_{12}(\underline{r},\sigma;\underline{r}',\sigma')=\frac{1}{\sqrt{ 2 }}\begin{vmatrix}
\psi_{1}(\underline{r})\alpha(\sigma) & \psi_{1}(\underline{r}')\alpha(\sigma') \\
\psi_{2}(\underline{r})\alpha(\sigma) & \psi_{2}(\underline{r}')\alpha(\sigma')
\end{vmatrix}=\frac{\alpha(\sigma)\alpha(\sigma')}{\sqrt{ 2 }}\begin{vmatrix}
\psi_{1}(\underline{r}) & \psi_{1}(\underline{r}') \\
\psi_{2}(\underline{r}) & \psi_{2}(\underline{r}')
\end{vmatrix}.$$
The spin component is the $\ket{S=1,M=1}$ triplet state. Two spin down electrons have a similar wavefunction but the spin component is the $\ket{S=1,M=-1}$ state.
Now consider the mixed spins states
$$\Psi_{12}^{\alpha\beta}=\frac{1}{\sqrt{ 2 }}\begin{vmatrix}
\psi_{1}(\underline{r})\alpha(\sigma) & \psi_{1}(\underline{r}')\alpha(\sigma') \\
\psi_{2}(\underline{r})\beta(\sigma) & \psi_{2}(\underline{r}')\beta(\sigma')
\end{vmatrix}$$
$$\Psi_{12}^{\beta\alpha}=\frac{1}{\sqrt{ 2 }}\begin{vmatrix}
\psi_{1}(\underline{r})\beta(\sigma) & \psi_{1}(\underline{r}')\beta(\sigma') \\
\psi_{2}(\underline{r})\alpha(\sigma) & \psi_{2}(\underline{r}')\alpha(\sigma')
\end{vmatrix}.$$
The spatial and spin components are not separable so they are not eigenstates of $\hat{S}^2$, however we can add/subtract them.
$$\Psi_{12}=\frac{1}{\sqrt{ 2 }}(\Psi_{12}^{\alpha\beta}+\Psi_{12}^{\beta \alpha})=\frac{1}{\sqrt{ 2 }}\begin{vmatrix}
\psi_{1}(\underline{r}) & \psi_{1}(\underline{r}') \\
\psi_{2}(\underline{r}) & \psi_{2}(\underline{r}')
\end{vmatrix} \frac{{\alpha(\sigma)\beta(\sigma')+\beta(\sigma)\alpha(\sigma')}}{\sqrt{ 2 }}$$
The spin component is $\ket{S=1,M=0}$.
$$\Psi_{12}=\frac{1}{\sqrt{ 2 }}(\Psi_{12}^{\alpha\beta}-\Psi_{12}^{\beta \alpha})=\frac{{\psi_{1}(\underline{r})\psi_{2}(\underline{r}')+\psi_{1}(\underline{r}')\psi_{2}(\underline{r})}}{\sqrt{ 2 }} \frac{1}{\sqrt{ 2 }}\begin{vmatrix}
\alpha(\sigma) & \alpha(\sigma') \\
\beta(\sigma) & \beta(\sigma')
\end{vmatrix}.$$
All of these wavefunctions ignore the repulsion force between the electrons, so to include it we will use first order perturbation theory
$$\hat{H}=\hat{H}_{0}+\frac{e^2}{4\pi \varepsilon_{0}\lvert \underline{r}-\underline{r}' \rvert }.$$We will call
$$V_{ee}=\frac{e^2}{4\pi \varepsilon_{0}\lvert \underline{r}-\underline{r}' \rvert }.$$
$$E_{triplet}=\bra{\psi_{12}^{t}}H_{0}\ket{\psi_{12}^t}+\bra{\psi_{12}^t}V_{ee}\ket{\psi_{!2}^t}.$$
$$\bra{\psi_{12}^t}V_{ee}\ket{\psi_{12}^t}=\frac{e^2}{4\pi \varepsilon_{0}}\int d^3rd^3r' \frac{\lvert\psi_{12}^t\rvert^2}{\lvert \underline{r}-\underline{r}' \rvert }. $$
The singlet is more likely to be closer since the spatial component is symmetric so the integral is larger.
$$E_{singlet}>E_{triplet}.$$
