Consider the [2nd quantisation](Boson%202nd%20Quantisation.md) of fermions which have antisymmetric wavefunctions. For example, the vacuum state vector showing the occupations of single particle states $\{ \phi_{i} \}$ is $\ket{0,0,\dots}$ or $\ket{(0)_{0},(0)_{1},\dots}$. As the wavefunction is antisymmetric, the order matters. 

Fermions experience Pauli exclusion, where $n_{i}=0,1$. Thus, the many-body state $\ket{1,0,1,1}$ is the slater determinant
$$\ket{1,0,1,1} =\ket{(1)_{0},(0)_{1},(1)_{2},(1)_{3}}=\frac{1}{\sqrt{ 3! }}\mathrm{\det}[\phi_{0},\phi_{2},\phi_{3}] \tag{12.1} $$$$\braket{ \vec{r}_{1},\vec{r}_{2},\vec{r}_{3} | 1,0,1,1 }=\frac{1}{\sqrt{ 3! }}\begin{bmatrix}
\phi_{0}(\vec{r}_{1}) & \phi_{0}(\vec{r}_{2}) & \phi_{0}(\vec{r}_{3}) \\
\phi_{2}(\vec{r}_{1}) & \phi_{2}(\vec{r}_{2}) & \phi_{2}(\vec{r}_{3}) \\
\phi_{3}(\vec{r}_{1}) & \phi_{3}(\vec{r}_{2}) & \phi_{3}(\vec{r}_{3})
\end{bmatrix}  .\tag{12.2} $$
Since the order of single particle labels matters, we need to keep track of the overall sign when defining creation/annihilation operators.
$$a_{j}\ket{n_{j},n_{0},n_{1},\dots}=\begin{cases}
0, & n_{j}=0 \\
\ket{n_{j}-1,n_{0},n_{1},\dots}, & n_{j}=1 
\end{cases} \tag{12.3} $$
$$a_{j}^{\dagger}\ket{n_{j},n_{0},n_{1},\dots} =\begin{cases}
\ket{n_{j}+1,n_{0},n_{1},\dots}  & n_{j}=0 \\
0, & n_{j}=1
\end{cases}\tag{12.4} $$
To find the overall phase after the action of these operators on a many-body vector state in the occupation number representation, we must first swap the phase of $\phi_j$ with occupation $n_j=1$ in the many-body state and bring it to the front of the determinant state.
$$\ket{n_{0},\dots,n_{j-1},(1)_{j},n_{j+1},\dots} =(-1)^{\eta_{j}}\ket{(1)_{j},n_{0},\dots,n_{j-1},n_{j+1},\dots}\tag{12.5} $$and
$$\ket{(1)_{j},n_{0},\dots ,n_{j-1},n_{j+1},\dots} =(-1)^{\eta_{j}}\ket{n_{0},\dots,n_{j-1},(1)_{j},n_{j+1},\dots}\tag{12.6}  $$
with $$\eta_{j}=\sum_{k=0}^{j-1}n_{k}\tag{12.7}. $$
Finally, we obtain
$$a_{j}\ket{n_{0},\dots,n_{j-1},(1)_{j},n_{j+1},\dots}=(-1)^{\eta_{j}}a_{j}\ket{(1)_{j},n_{0},\dots ,n_{j-1},n_{j+1},\dots}=(-1)^{\eta_{j}}\ket{n_{0},\dots,n_{j-1},(0)_{j},n_{j+1},\dots}\tag{12.8} $$
$$a^{\dagger}_{j}\ket{n_{0},\dots,n_{j-1},(0)_{j},n_{j+1},\dots}=(-1)^{\eta_{j}}a_{j}^{\dagger}\ket{(0)_{j},n_{0},\dots ,n_{j-1},n_{j+1},\dots}=(-1)^{\eta_{j}}\ket{n_{0},\dots,n_{j-1},(1)_{j},n_{j+1},\dots}\tag{12.9} $$
If $\Phi$ contains state $j$ and does not contain state $\ell$, with $\ell>j$,
$$a_{j}^{\dagger}a_{j}\ket{n_{0},\dots,(1)_{j},\dots,(0)_{\ell},\dots} =(-1)^{\eta_{j}}a_{\ell}^{\dagger}\ket{n_{0},\dots ,(0)_{j},\dots,(0)_{\ell},\dots}=(-1)^{\eta_{j}+\eta_{\ell}-1}\ket{n_{0},\dots,(0)_{j},\dots,(1)_{\ell},\dots}\tag{12.10}.   $$On the other hand
$$a_{j}a_{\ell}^{\dagger}\ket{n_{0},\dots,(1)_{j},\dots,(0)_{\ell},\dots} =(-1)^{\eta_{\ell}}a_{j}\ket{n_{0},\dots,(1)_{j},\dots,(1)_{\ell},\dots} =(-1)^{\eta_{j}+\eta_{\ell}}\ket{n_{0},\dots,(0)_{j},\dots,(1)_{\ell},\dots}\tag{12.11}  .$$
Therefore $$[a_{\ell}^{\dagger}a_{j}+a_{j}a_{\ell}^{\dagger}]\Phi=0$$for $j\neq \ell$  so the anticommutator $[a_{\ell}^{\dagger},a_{j}]_{+}=0$.

In general,
$$[a_{\ell}^{\dagger},a_{j}]_{+}=\delta_{j\ell}\tag{12.12} $$
$$[a_{\ell}^{\dagger},a_{j}^{\dagger}]_{+}=[a_{\ell},a_{j}]_{+}=0\tag{12.13}. $$Finally, $a^{\dagger}_{j}a_{j}=\hat{N}_{j}$ counts the number of fermions in state $j$. The total number operator in the many-body state counting particles in any single-particle state is
$$\hat{N}=\sum_{j}a^{\dagger}_{j}a_{j}=\sum_{j}\hat{N}_{j}\tag{12.14} .$$
The fermionic many-body state vector in the ground state is
$$\ket{(1)_{1},(1)_{2},\dots,(1)_{n},(0)_{n+1},\dots} =\frac{1}{\sqrt{ n! }}\det[\phi_{1},\phi_{2},\dots,\phi_{n}]=\frac{1}{\sqrt{ n! }}\sum_{P}(-1)^{P}\phi_{1}\times \phi_{2}\times\dots \times \phi_{n}\tag{12.15} $$where $\phi_{1}\times \phi_{2}\times\dots \times \phi_{n}$ is an n-particle product state where the1st particle is in state $\phi_{1}$, 2nd in $\phi_{2}$ and so on.

We can write the wavefunction as
$$\braket{ \vec{r}_{1},\vec{r}_{2},\dots,\vec{r}_{n} | (1)_{1},(1)_{2},\dots,(1)_{n} }=\frac{1}{\sqrt{ n! }}\det[\phi_{1},\phi_{2},\dots,\phi_{n}](\vec{r}_{1},\vec{r}_{2},\dots,\vec{r}_{n})=\frac{1}{\sqrt{ n! }}\sum_{P}(-1)^{P}\hat{P}\phi_{1}(\vec{r}_{1})\phi_{2}(\vec{r}_{2})\dots \phi_{n}(\vec{r}_{n})\tag{12.16}.  $$
$\hat{P}$ is a permutation operator that acts either on the single-particle states $\phi_{i}$ or on the spatial coordinates $\vec{r}_{i}$ but not on both. The sum is over all permutations of $(1,\dots,n)$. The eigenvalues $P$ of a permutation is $\pm 1$ depending on the even or odd number of exchanges of pairs of labels in the permutation.

In the second quantisation, the $n$-fermion Slater determinant state, $\ket{(1)_{1},(1)_{2},\dots,(1)_{n}}$, takes a simple form
$$\ket{(1)_{1},(1)_{2},\dots,(1)_{n}} =\frac{1}{\sqrt{ n! }}\det[\phi_{1},\phi_{2},\dots,\phi_{n}]=a_{1}^{\dagger}\dots a_{n}^{\dagger}\ket{0}\tag{12.17}  $$