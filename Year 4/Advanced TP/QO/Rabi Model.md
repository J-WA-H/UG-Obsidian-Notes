 Consider the [semiclassical Hamiltonian](Atom-Field%20Interactions.md) in terms of atomic eigenstates $\ket{\psi_{j}}$,
$$\hat{H}=\sum_{j}E_{j}\ket{\psi_{j}} \bra{\psi_{j}}-\sum_{j\neq j'}\vec{d}_{jj'}\cdot \vec{E}(t)\ket{\psi_{j}} \bra{\psi_{j'}}\tag{8.1}   .$$
Using the dipole approximation, where $\vec{E}$ is spatially invariant over the relevant length scales so we can rewrite this using [(2.8)](Classical%20EM%20Fields.md),
$$\vec{d}_{jj'}\cdot \vec{E}(t)=i\sum_{\vec{k},s}\vec{d}_{jj'}\cdot \vec{e}_{\vec{k}s}\omega_{\vec{k}}[A_{\vec{k},s}(0)e^{ -i\omega_{k}t }-\text{c.c.}]\tag{8.2} .$$
In the rotating wave approximation, eliminate terms which are counter-rotating in the interaction picture,
$$\hat{H}=\sum_{j}E_{j}\ket{\psi_{j}} \bra{\psi_{j}} +\frac{\hbar}{2}\sum_{\vec{k},s}\sum_{j>j'}[\Omega_{jj'\vec{k}s}e^{ -i\omega_{k}t }\ket{\psi_{j}} \bra{\psi_{j'}} +\text{c.c.}]\tag{8.3} $$
where
$$\frac{\hbar}{2} \Omega_{jj'\vec{k}s}=-i(\vec{d}_{jj'}\cdot \vec{e}_{\vec{k}s})\omega_{\vec{k}}A_{\vec{k}s}(0).\tag{8.4} $$
The first term is the standard atomic Hamiltonian and the second is the driving term, which describes the coupling to the classical electric field.

The polarised monochromatic field is where $A_{\vec{k}s},A^{*}_{\vec{k}s}$ is only significant for particular polarisation $s$ and frequency $\omega$.

The frequency is provided by a laser where $\omega_{L}\approx\omega_{eg}=\frac{E_{e}-E_{g}}{\hbar}$ and $\vec{d}_{eg}\neq 0$,
$$\hat{H}=\sum_{j}E_{j}\ket{\psi_{j}} \bra{\psi_{j}} +\frac{\hbar}{2}[\Omega e^{ -i\omega_{L}t }\ket{\psi_{e}} \bra{\psi_{g}}+\text{c.c.} ]\tag{8.5}. $$
In the Rabi model, subtract $\left[ \frac{E_{e}-E_{g}}{2} \right]\sum_{j}\ket{\psi_{j}}\bra{\psi_{j}}$ from the Hamiltonian. Set $\ket{e}=\ket{\psi_{e}}$ at $+\hbar \omega_{eg}/2$ and $\ket{g}=\ket{\psi_{g}}$ at $-\hbar \omega_{eg}/2$.
This gives the Hamiltonian,
$$\hat{H}=\frac{\hbar\omega}{2}(\ket{e} \bra{e} -\ket{g} \bra{g} )+\frac{\hbar}{2}[\Omega e^{ -i\omega_{L}t }\ket{e} \bra{g} + \text{c.c.}]\tag{8.6}. $$
It is common to use the ground $\ket{g}$ and excited $\ket{e}$ states to define Pauli spin operators,
$$\hat{\sigma}_{z}=\ket{e} \bra{e} -\ket{g} \bra{g} $$
$$\hat{\sigma}^{+}=\ket{e} \bra{g} \tag{8.7} $$
$$\hat{\sigma}^{-}=\ket{g} \bra{e}. $$
May assume $\Omega$ is real with no loss of generality. This mean we can rewrite the Hamiltonian as
$$\hat{H}=\frac{\hbar \omega_{eg}}{2}\hat{\sigma}_{z}+\frac{\hbar \Omega}{2}(e^{ -i\omega_{L}t }\hat{\sigma}^{+}+e^{ i\omega_{L}t }\hat{\sigma}^{-}).\tag{8.8} $$
Consider a transformation defined by the unitary operator
$$\hat{U}=e^{ i\hat{\sigma}_{z}\omega_{L}t/2 }\tag{8.9} $$
so the transformed Hamiltonian is
$$\hat{H}'=\hat{U}\hat{H}\hat{U}^{\dagger}-\frac{\hbar \omega_{L}\hat{\sigma}_{z}}{2}.\tag{8.10} $$
In particular, 
$$\hat{U}\ket{e} \bra{g} \hat{U}^{\dagger}=e^{ i\ket{e} \bra{e} \omega_{L}t/2 }e^{ -i\ket{g} \bra{g} \omega_{L}t/2 }\ket{e} \bra{g} e^{ -i\ket{e} \bra{e} \omega_{L}t/2 }e^{ i\ket{g} \bra{g} \omega_{L}t/2 }\tag{8.11} =e^{ i\ket{e} \bra{e} \omega_{L}t/2 }\ket{e} \bra{g} e^{ i\ket{g} \bra{g} \omega_{L}t/2 }= e^{ i\omega_{L}t/2 }\ket{e} \bra{g} e^{ i\omega_{L}t/2 }.$$
Consider the corotating frame,
$$\hat{U}e^{ -i\omega_{L}t }\ket{e} \bra{g}\hat{U}^{\dagger}=\ket{e} \bra{g}\tag{8.12}  $$
and 
$$\hat{H}=\frac{\hbar\Delta}{2}\hat{\sigma}_{z}+\frac{\hbar\Omega}{2}(\hat{\sigma}^{+}+\hat{\sigma}^{-}).\tag{8.13} $$
Here $\Delta=\omega_{eg}-\omega_{L}$ is the detuning (difference of laser frequency from atomic transition frequency).

This gives a time independent Hamiltonian.

In a basis $\{ \ket{g},\ket{e} \}$, the matrix representation of the Hamiltonian is
$$\hat{H}=\frac{\hbar}{2}\begin{bmatrix}
\Delta & \Omega \\
\Omega & -\Delta
\end{bmatrix}.\tag{8.14} $$
This is straightforward to diagonalise.
The on-resonance case simplifies this to the $\Delta=0$ case,
$$\hat{H}=\frac{\hbar}{2}\begin{bmatrix}
0 & \Omega \\
\Omega & 0
\end{bmatrix}.\tag{8.15} $$
This gives eigenvalues $E_{\pm}=\pm\frac{\hbar\Omega}{2}$ with eigenvectors
$$\ket{\psi_{+}}=\frac{1}{\sqrt{ 2 }}\begin{bmatrix}
1 \\
1
\end{bmatrix},\;\ket{\psi_{-}} =\frac{1}{\sqrt{ 2 }}\begin{bmatrix}
-1 \\
1
\end{bmatrix}.\tag{8.16}  $$
To consider time evolution, the general state $\ket{\psi(0)}=a\ket{\psi_{+}}+b\ket{\psi_{-}}$ evolves as
$$\ket{\psi(t)} =ae^{ -i\Omega t/2 }\ket{\psi_{+}} +be^{ i\Omega t/2 }\ket{\psi_{-}} \tag{8.17} .$$
From this, the initial state $\ket{g}=\frac{1}{\sqrt{ 2 }}(\ket{\psi_{+}}+\ket{\psi_{-}})$ evolves as
$$\ket{\psi(t)} =\begin{bmatrix}
-i\sin\left( \frac{\Omega t}{2} \right) \\
\cos\left( \frac{\Omega t}{2} \right)
\end{bmatrix}.\tag{8.18} $$
The population of the ground state $\ket{g}$ evolves as $[1+\cos(\Omega t)]/2$, for the excited state, the population evolves as $[1-\cos(\Omega t)]/2$. The parameter $\Omega$ is the Rabi frequency.

