From [[Fermion 2nd Quantisation]] we have $a_{j}^{\dagger}a_{j}=\hat{N}_{j}$ and $\hat{N}=\sum_{j}a^{\dagger}_{j}a_{j}=\sum_{j}\hat{N}$.
$$[a^{\dagger}_{\ell},a^{\dagger}_{j}]_{+}=0\tag{13.1} .$$
From this, $a_{j}^{\dagger}a_{j}^{\dagger}\ket{\phi^{(N)}}=0$ since
$$a_{j}^{\dagger}\ket{\phi^{(N)}} =\begin{cases}
0 & \text{occupied} \\
\ket{\phi^{(N+1)}}  & \text{unoccupied}
\end{cases}\tag{13.2}. $$
Since the first creation operator gives 0 if $\ket{\phi^{(N)}}$ is occupied, or $\ket{\phi^{(N+1)}}$ if $\ket{\phi^{(N)}}$ is unoccupied. In this case, $\ket{\phi^{(N+1)}}$ is occupied so $a_{j}^{\dagger}\ket{\phi^{(N+1)}}=0$.

For electrons, we have to consider spin, $\ket{\phi_{i},\sigma}$
$$[a^{\dagger}_{\ell\sigma},a_{j\sigma'}]_{+}=\delta_{j\ell}\delta_{\sigma\sigma'}\tag{13.3}. $$
One-body operator
$$\hat{Q}=\sum_{i=1}^Nq(\vec{r}_{i},\vec{p}_{i})\tag{13.4} .$$
In general this can be written as
$$\hat{Q}=\sum_{\sigma,\sigma'}\sum_{i,j}q^{\sigma\sigma'}_{ij}a^{\dagger}_{i\sigma}a_{j\sigma'}\tag{13.5}. $$Then we need to determine the matrix element $q_{ij}^{\sigma\sigma'}$. We demand that the matrix element in the first and second quantisation are the same.

1st quantisation,
$$\bra{\phi_{k},\sigma}\hat{Q}\ket{\phi_{\ell},\sigma'} =\braket{ \sigma | \sigma' } \int d^3r\phi_{k}^{*}(\vec{r})Q(\vec{r},\vec{p})\phi_{\ell}(\vec{r})\tag{13.6}. $$
2nd quantisation,
$$\bra{\phi_{k},\sigma} =\bra{0} a_{k\sigma},\;\ket{\phi_{\ell},\sigma'}=a^{\dagger}_{\ell\sigma'}\ket{0}.\tag{13.7}$$
$$\therefore  \bra{\phi_{k,\sigma}}\hat{Q}\ket{\phi_{\ell},\sigma'}=\bra{0} a_{k\sigma}\sum_{s,s'}\sum_{i,j}q^{ss'}_{ij}a_{is}^{\dagger}a_{js'}a^{\dagger}_{\ell\sigma'}\ket{0}=\sum_{ss'}\sum_{ij}q^{ss'}_{ij}\bra{0} a_{k\sigma}a^{\dagger}_{ij}a_{js'}a^{\dagger}_{\ell\sigma'}\ket{0}\tag{13.8}. $$
Consider $\bra{0}a_{k\sigma}a^{\dagger}_{is}$, using the anticommutator relation,
$$\bra{0} a_{k\sigma}a^{\dagger}_{is}=\bra{0} \delta_{ik}\delta_{s\sigma}-\cancelto{0}{\bra{0} a^{\dagger}_{is}a_{k\sigma}}\tag{13.9} $$
and $a_{js'}a^{\dagger}_{\ell\sigma'}\ket{0}$,
$$a_{js'}a_{\ell\sigma'}^{\dagger}\ket{0} =\delta_{j\ell}\delta_{s'\sigma'}\ket{0}-\cancelto{0}{a_{\ell\sigma'}^{\dagger}a_{js'}}\ket{0}\tag{13.10}.   $$
This gives
$$\bra{\phi_{k},\sigma}\hat{Q}\ket{\phi_{\ell},\sigma'}=\braket{ 0 | 0 } \sum_{ss'}\sum_{ij}q^{ss'}_{ij}\delta_{ik}\delta_{s\sigma}\delta_{\ell j}\delta_{\sigma's'}=q^{\sigma\sigma'}_{k\ell}\tag{13.11}.$$
This must equal the result from first quantisation, so
$$q^{\sigma\sigma'}_{k\ell}=\delta_{\sigma\sigma'}\int d^3r\phi_{k}^{*}(\vec{r})Q(\vec{r},\vec{p})\phi_{\ell}(\vec{r})\tag{13.12}. $$
Hence we have
$$\hat{Q}=\sum_{\sigma\sigma'}\sum_{ij}q^{\sigma\sigma'}_{ij}a^{\dagger}_{i\sigma}a_{j\sigma'}=\sum_{\sigma}\sum_{k,\ell}q^{\sigma\sigma}_{k\ell}a^{\dagger}_{k\sigma}a_{j\sigma}=\sum_{\sigma}\sum_{k\ell}\int d^{3}r\phi ^{*}_{k}(\vec{r}) a^{\dagger}_{k\sigma}Q(\vec{r},\vec{p})a_{\ell\sigma}\phi_{\ell}(\vec{r})\tag{13.13}. $$Define
$$\sum_{k}\phi ^{\dagger}_{k}(\vec{r})a^{\dagger}_{k\sigma}\equiv \hat{\Psi}^{\dagger}_{\sigma}(\vec{r})\tag{13.14} $$
$$\sum_{\ell}a_{\ell\sigma}\phi_{\ell}(\vec{r})\equiv \hat{\Psi}_{\sigma}(\vec{r})\tag{13.15} $$
$$\implies \hat{Q}=\sum_{\sigma}\int d^{3}r \hat{\Psi}^{\dagger}_{\sigma}(\vec{r})q(\vec{r}) \hat{\Psi}_{\sigma}(\vec{r})\tag{13.16}. $$
This can be used to rewrite the one-body Hamiltonian
$$\hat{H}_{1}=\sum_{\sigma}\sum_{ij}\int d^3r \phi_{i}^{*}(\vec{r})\left[ -\frac{1}{2}\nabla^2+V_{en}(\vec{r}) \right]\phi_{j}(\vec{r})a^{\dagger}_{i\sigma}a_{j\sigma}=\sum_{\sigma}\sum_{ij}h_{ij}a^{\dagger}_{i\sigma}a_{j\sigma}\tag{13.17}. $$
For single particle wavefunctions $h(\vec{r})\phi_{j}(\vec{r})=\varepsilon_{j}\phi_{j}{(\vec{r})}$, This gives a diagonalised Hamiltonian
$$\hat{H}_{1}=\sum_{j,\sigma}\varepsilon_{j}a_{j\sigma}^{\dagger}a_{j\sigma}\tag{13.18} .$$
To obtain the second quantised operator we replace the sum with an integral
$$\sum_{r_{i}}\to \sum_{\sigma}\int d^3r \hat{\Psi}_{\sigma}^{\dagger}(\vec{r})\hat{O}\hat{\Psi}_{\sigma}(\vec{r})\tag{13.19} .$$
Consider the operator for electron charge density,
$$\hat{\rho}(\vec{x})=\sum_{i}\delta^{(3)}(\vec{x}-\vec{x}_{i})\tag{13.20}. $$
This is the 1st quantised operator. The expectation value of this, we expect, is $\rho(\vec{x})$,
$$\bra{\Psi} \hat{\rho}(\vec{x})\ket{\Psi} =\sum_{\sigma_{i}}\int d^3r_{1}\int d^3r_{2}\dots \int d^3r_{N}|\Psi(\vec{r}_{1},\sigma_{1};\vec{r}_{2},\sigma_{2};\dots \vec{r}_{N},\sigma_{N})|^2[\delta(\vec{x}-\vec{r}_{1})+\delta(\vec{x}-\vec{r}_{2})+\dots+\delta(\vec{x}-\vec{r}_{N})]\tag{13.21} $$
$$=\int d^3r_{1}\delta(\vec{x}-\vec{r}_{1})\sum_{\sigma_{i}}\int d^3r_{2}\dots \int d^3r_{N}|\Psi(\vec{r}_{1},\sigma_{1};\vec{r}_{2},\sigma_{2};\dots \vec{r}_{N},\sigma_{N})|^2+\dots+\int d^3r_{N}\delta(\vec{x}-\vec{r}_{N})\sum_{\sigma_{i}}\int d^2r_{1}\dots \int d^3r_{N-1}|\Psi|^2$$
$$=\frac{1}{N}\int d^3r_{1}\delta(\vec{x}-\vec{r}_{1})\rho(\vec{r}_{1})+\frac{1}{N}\int d^3r_{2}\delta(\vec{x}-\vec{r}_{2})\rho(\vec{r}_{2})+\dots+\frac{1}{N}\int d^3r_{N}\delta(\vec{x}-\vec{r}_{N})\rho(\vec{r}_{N})=\frac{N}{N}\rho(\vec{x})=\rho(\vec{x})\;\square \tag{13.22} $$
The second quantised form is
$$\rho(\vec{x})=\sum_{i}\delta(\vec{x}-\vec{r}_{i})\to \hat{\rho}(\vec{x})=\sum_{\sigma}\int d^3r\Psi^{\dagger}_{\sigma}(\vec{r})\delta(\vec{x}-\vec{r})\Psi_{\sigma}(\vec{r})\tag{13.23}\implies \hat{\rho}(\vec{x})+\sum_{\sigma}\Psi_{\sigma}^{\dagger}(\vec{x})\Psi_{\sigma}(\vec{x}). $$
To find the two-body operator for electrons.
$$V_{ee}=\frac{1}{2}\sum_{i,j}^{j\neq j} \frac{1}{|\vec{r}_{i}-\vec{r}_{j}|}=\frac{1}{2}\sum_{i}W(\vec{r}_{i})\tag{13.24} $$
with
$$W(\vec{r})=\sum_{j} \frac{1}{|\vec{r}_{j}-\vec{r}|}\to \sum_{\sigma}\int d^3r \hat{\Psi}_{\sigma}^{\dagger}(\vec{r})W(\vec{r}) \hat{\Psi}_{\sigma}(\vec{r}).\tag{13.25}.$$
This gives
$$V_{ee}=\frac{1}{2}\sum_{\sigma}\int d^3r \hat{\Psi}^{\dagger}_{\sigma}(\vec{r})W(\vec{r}) \hat{\Psi}_{\sigma}(\vec{r})\tag{13.26} $$
and
$$W(\vec{r})=\sum_{\sigma'}\int d^3r' \hat{\Psi}^{\dagger}_{\sigma'}(\vec{r}') \frac{1}{|\vec{r}-\vec{r}'|} \hat{\Psi}_{\sigma'}(\vec{r}')\tag{13.27}. $$
Combining $(13.26-27)$ gives
$$V_{ee}=\frac{1}{2}\sum_{\sigma}\int d^3r \hat{\Psi}_{\sigma}^{\dagger}(\vec{r})\sum_{\sigma'}\int \frac{d^3r'}{|\vec{r}-\vec{r}'|}\hat{\Psi}_{\sigma'}^{\dagger}(\vec{r}') \hat{\Psi}_{\sigma'}(\vec{r}') \hat{\Psi}_{\sigma}(\vec{r})\tag{13.28}=\frac{1}{2} \sum_{\sigma,\sigma'}\iint \frac{d^3rd^3r'}{|\vec{r}-\vec{r}'|} \hat{\Psi}^{\dagger}_{\sigma}(\vec{r}) \hat{\Psi}_{\sigma'}^{\dagger}(\vec{r}') \hat{\Psi}_{\sigma'}(\vec{r}')\hat{\Psi}_{\sigma}(\vec{r}).$$
Therefore, in terms of single particle wavefunctions,
$$V_{ee}=\frac{1}{2}\sum_{\sigma,\sigma'}\iint \frac{d^3rd^3r'}{|\vec{r}-\vec{r}'|}\sum_{i,j,k,\ell}\phi_{i}^{*}(\vec{r})\phi_{j}^{*}(\vec{r}')\phi_{k}(\vec{r}')\phi_{\ell}(\vec{r})a^{\dagger}_{i\sigma}a^{\dagger}_{j\sigma'}a_{k\sigma'}a_{\ell\sigma}.\tag{13.29} $$
Now demonstrate that the N-particle slater determinant formed from a complete set of single particle basis functions forms a complete basis of an N-particle Hilbert space.

For N=2, take $\Psi(\vec{x},\vec{x})$ as a general normalised fermionic wavefunction, with $\vec{x}$ describing both position and spin. $\{ \phi_{i}(\vec{x}) \}$ is a complete basis of single particle wavefunctions, so for sum general function $f(x)=\sum_{n}c_{n}\phi_{n}(\vec{x})$. This means we can write
$$\Psi(\vec{x},\vec{x}')=\sum_{i}c_{i}(\vec{x})\phi_{i}(\vec{x}')=\sum_{i,j}c_{ij}\phi_{j}(\vec{x})\phi_{i}(\vec{x})\tag{13.30}=-\Psi(\vec{x}',\vec{x}). $$
$$\implies\Psi(\vec{x}',\vec{x})=-\sum_{i,k}c_{ij}\phi_{i}(\vec{x})\phi_{j}(\vec{x}')\tag{13.31}\implies\Psi(\vec{x},\vec{x}')=\frac{1}{2}\sum_{ij}c_{ij}[\phi_{i}(\vec{x}')\phi_{j}(\vec{x})-\phi_{i}(\vec{x})\phi_{j}(\vec{x}')]. $$
Consider the cases where $i=j$, $j<i$, and $j>i$.
$$\Psi(\vec{x},\vec{x}')=\frac{1}{2}\sum_{i}\left[ c_{ii}\cdot 0+\sum_{j<i} c_{ij}[\phi_{i}(\vec{x}')\phi_{j}(\vec{x})-\phi_{i}(\vec{x})\phi_{j}(\vec{x}')]+\sum_{j>i}c_{ij}[\phi_{i}(\vec{x}')\phi_{j}(\vec{x})-\phi_{i}(\vec{x})\phi_{j}(\vec{x}')] \right]\tag{13.32} .$$Swap $i\leftrightarrow j$,
$$\Psi(\vec{x},\vec{x}')=\frac{1}{2}\left( \sum_{j<i}c_{ij}(\phi_{i}(\vec{x}')\phi_{j}(\vec{x})-\phi_{i}(\vec{x})\phi_{j}(\vec{x}'))+\sum_{j>i}c_{ji}(\phi_{j}(\vec{x}')\phi_{i}(\vec{x})-\phi_{j}(\vec{x})\phi_{i}(\vec{x}') \right)=\frac{1}{2}\sum_{i,j}^{i\neq j} \frac{{c_{ji}-c_{ij}}}{\sqrt{ 2 }} \frac{{\phi_{i}(\vec{x})\phi_{j}(\vec{x}')-\phi_{j}(\vec{x})\phi_{i}(\vec{x}')}}{\sqrt{ 2 }}\;\square$$
$(13.33)$.

We can do the same for bosons, but the diagonal terms are no longer zero.
$$\Psi(\vec{x},\vec{x}')=\frac{1}{2}\sum_{i,j}c_{ij}(\phi_{i}(\vec{x})\phi_{j}(\vec{x}')+\phi_{j}(\vec{x})\phi_{i}(\vec{x}'))\tag{13.34}. $$
Using the same method gives
$$\Psi(\vec{x},\vec{x}')=\sum_{i}c_{ii}\phi_{i}(\vec{x})\phi_{i}(\vec{x}')+\sum_{i,j}^{i\neq j} \frac{{c_{ij}+c_{ji}}}{\sqrt{ 2 }} \frac{{\phi_{i}(\vec{x})\phi_{j}(\vec{x}')+\phi_{j}(\vec{x})\phi_{i}(\vec{x}')}}{\sqrt{ 2 }}.\tag{13.35} $$
