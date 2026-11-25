Introducing an arbitrary action scale $\mathcal{A}$, the coordinate $q_{k}$ and canonical momentum $p_{k}$ are from the [[Classical EM Fields]]$$q_{\vec{k}s}=c\sqrt{ \frac{\varepsilon_{0}V}{\mathcal{A}\omega_{k}} }(A_{\vec{k}s}+A^{*}_{\vec{k}s})\tag{3.1} $$$$p_{\vec{k}s}=\frac{i\omega_{k}}{c}\sqrt{ \varepsilon_{0}V\mathcal{A}\omega_{k} }(A^{*}_{\vec{k}s}-A_{\vec{k}s}).\tag{3.2} $$This gives the Hamiltonian$$H=\sum_{\vec{k},s}\left( \frac{p_{\vec{k},s}^2}{2\mathcal{M}_{k}}+\frac{\mathcal{M}_{k}\omega_{k}^2q_{k}^2}{2} \right)\tag{3.3} $$where
$$\mathcal{M}_{k}=\frac{\mathcal{A}_{k}\omega_{k}}{c^2}.\tag{3.4} $$
This is an ensemble of harmonic oscillators.
As $[\hat{q}_{\vec{k}s},\hat{p}_{\vec{k}s}]=i\hbar$, set $\mathcal{A}=\hbar$. Introduce creation $\hat{a}^{\dagger}_{\vec{k}s}$ and annihilation $\hat{a}_{\vec{k}s}$ operators,$$\hat{a}_{\vec{k}s}=\sqrt{ \frac{\mathcal{M}_{k}\omega_{k}}{2\hbar} }\hat{q}_{\vec{k}s}+i \frac{\hat{p}_{\vec{k}s}}{\sqrt{ 2\mathcal{M}_{k}\hbar \omega_{k} }}.\tag{3.5} $$This gives the Hamiltonian
$$\hat{H}=\sum_{\vec{k},s}\left( \hat{a}^{\dagger}_{\vec{k}s}\hat{a}_{\vec{k}s}+\frac{1}{2} \right).\tag{3.6} $$
The creation operator deexcites an electron in an atom - which emits a photon, so the operator can be seen as creating a photon.

The commutation relation is given by
$$[\hat{a}_{\vec{k}s},\hat{a}^{\dagger}_{\vec{k}'s'}]=\delta_{\vec{k}\vec{k}'}\delta_{ss'}.\tag{3.7} $$
Number states are a convenient ordering of the modes, enumerated by $j$:
$$\begin{matrix}
\hat{a}_{j}\ket{n_{1},n_{2},\dots ,n_{j},\dots}=\sqrt{ n_{j} }\ket{n_{1},n_{2},\dots ,n_{j}-1,\dots} \\
\hat{a}^{\dagger}_{j}\ket{n_{1},n_{2},\dots ,n_{j},\dots} =\sqrt{ n_{j}+1 }\ket{n_{1},n_{2},\dots,n_{j}+1,\dots} 
\end{matrix}  \tag{3.8} .$$
These operators give the quantised electric field, which describes how the field couples to matter, typically though a dipole moment.
The quantised electric field is given by$$\hat{E}(\vec{r},t)=i\sum_{\vec{k},s}\sqrt{ \frac{\hbar\omega_{k}}{2\varepsilon_{0}V} }\vec{e}_{\vec{k}s}[\hat{a}_{\vec{k}s}e^{ i\vec{k}\cdot \vec{r} }-\text{H.c.}]\tag{3.9} $$where $\text{H.c.}$ is the Hermitian conjugate.

For a single mode this reduces to
$$\hat{E}=i\sqrt{ \frac{\hbar\omega_{k}}{2\varepsilon_{0}V} }\vec{e}[\hat{a}e^{ i\vec{k}\cdot \vec{r} }-\text{H.c.}]\tag{3.10} .$$
The spatial of the field over the extent of an atomic system frequency is negligible so$$e^{ i\vec{k}\cdot \vec{r} }\approx 1+i\vec{k}\cdot \vec{r}$$so the field can be further reduced to
$$\hat{E}=i\sqrt{ \frac{\hbar\omega_{k}}{2\varepsilon_{0}V} } \vec{e}[\hat{a}-\hat{a}^{\dagger}]. \tag{3.11} $$
