It is possible to realise a single atomic transition coupled to a single field mode in very high Q cavities (microwave or optical),
$$\hat{H}=\frac{\hbar \omega}{2}\hat{\sigma}_{z}+\hbar \omega \hat{a}^{\dagger}\hat{a}+g_{C}(\hat{a}\hat{\sigma}^{+}+\hat{a}^{\dagger}\hat{\sigma}^{-}). \tag{9.1} $$We can assume $$g_{C}=-i(\vec{d}_{eg}\cdot \vec{e})\sqrt{ \frac{\hbar \omega}{2\varepsilon_{0}V} }\tag{9.2} $$is real without the loss of generality.

Consider the frame transformation $\hat{U}=e^{ i\hat{a}^{\dagger}\hat{a}\omega t/2 }$.
$$\hat{H}=\frac{\hbar \omega_{eg}}{2}\hat{\sigma}_{z}+g_{C}(e^{ -i\omega t/2 }\hat{a}\hat{\sigma}^{+}+e^{ i\omega t/2 }\hat{a}^{\dagger}\hat{\sigma}^{-})\tag{9.3} .$$Define a subsequent unitary transformation $\hat{U}=e^{ i\hat{\sigma}_{z}\omega t/2 }$ which gives
$$\hat{H}=\frac{\hbar\Delta}{2}\hat{\sigma}_{z}+g_{C}(\hat{a}\hat{\sigma}^{+}+\hat{a}^{\dagger}\hat{\sigma}^{-}).\tag{9.4} $$
This is the Jaynes-Cummings model.

The matrix elements form an effective 2-level system,
$$\begin{matrix}
\bra{e,n} \hat{H}\ket{e,n} =\frac{\hbar\Delta}{2} & \bra{e,n} \hat{H}\ket{g,n+1} =g_{C}\sqrt{ n+1 } \\
\bra{g,n+1} \hat{H}\ket{e,n} = g_{C}\sqrt{ n+1 } & \bra{g,n+1} \hat{H}\ket{g,n+1} = -\frac{\hbar\Delta}{2}
\end{matrix}.\tag{9.5} $$
In the basis representation set by $\{ \ket{g,n+1},\ket{e,n} \}$ for some $n$,
$$\hat{H}=\begin{bmatrix}
\frac{\hbar\Delta}{2} & g_{C}\sqrt{ n+1 } \\
g_{C}\sqrt{ n+1 } & -\frac{\hbar\Delta}{2}
\end{bmatrix}\tag{9.6} .$$
In complete analogy to the [[Rabi Model]], for $\Delta=0$, it has eigenvalues $E_{\pm}=\pm g_{C}\sqrt{ n+1 }$ with eigenvectors
$$\ket{\psi_{+}}=\frac{1}{\sqrt{ 2 }}\begin{bmatrix}
1 \\
1
\end{bmatrix},\;\ket{\psi_{-}} =\frac{1}{\sqrt{ 2 }}\begin{bmatrix}
-1 \\
1
\end{bmatrix} .\tag{9.7} $$
Atoms are dressed in the state of the field,
$$\ket{\psi_{+}}=\frac{1}{\sqrt{ 2 }}(\ket{g,n+1} +\ket{e,n} ),\;\ket{\psi_{-}} =\frac{1}{\sqrt{ 2 }}(\ket{g,n+1} -\ket{e,n} ) .\tag{9.8} $$
The basis $\{ \ket{g,n+1},\ket{e,n} \}$ states are called bare states.

For Rabi oscillations, for an initial state $\ket{g,n+1}$, population in this state subsequently evolves as
$$\frac{1}{2}\left[ {1}+\cos\left( \left[ \frac{2g_{C}\sqrt{ n+1 }}{\hbar} \right]t \right)  \right]\tag{9.9} .$$
Excited state $\ket{e,n}$ population evolves as
$$\frac{1}{2}\left[ 1-\cos\left( \left[ \frac{2g_{C}\sqrt{ n+1 }}{\hbar} \right]t \right) \right].\tag{9.10} $$
The effective Rabi frequency is then set by
$$\frac{2g_{C}\sqrt{ n+1 }}{\hbar} \tag{9.11}, $$
also when $n=0$.