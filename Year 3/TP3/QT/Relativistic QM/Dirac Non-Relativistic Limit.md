The non-relativistic limit of the [Klein-Gordon equation](Charged%20Particles%20in%20an%20EM%20Field.md) gives the Schrodinger equation, so we expect the same for the [Dirac equation](Dirac%20Equation%20Derivation.md) but the fact that the wavefunction has multiple components causes issues.
This gives spin in a natural and consistent way.

First couple the Dirac equation to the EM-field.
Using minimal coupling, $p^{\mu}\to p^{\mu}-eA^{\mu}$, and the correspondence principal, $p^{\mu}\to i\hbar \partial^{\mu}-eA^{\mu}$.

This yields the Dirac equation,
$$(i\hbar \partial \!\!\!/-eA\!\!\!/-mc)\psi(\underline{x},t)=0.$$
Expanding this into component form gives
$$\frac{i\hbar\gamma^{0}}{c} \frac{{\partial \psi}}{\partial t}+i\hbar \gamma^{k}\nabla_{k}\psi-e\gamma^{0} \frac{\phi}{c}\psi+e\gamma^{k}A_{k}\psi-mc\psi=0.$$
Decompose $\psi$ into 2 2-component spinors,
$$\psi=\begin{bmatrix}
\tilde{\Phi} \\
\tilde{\chi}
\end{bmatrix};\;\tilde{\Phi}=\begin{bmatrix}
\tilde{\Phi}_{1} \\
\tilde{\Phi}_{2}
\end{bmatrix};\;\tilde{\chi}=\begin{bmatrix}
\tilde{\chi}_{1} \\
\tilde{\chi}_{2}
\end{bmatrix}.$$
Use the gamma matrices
$$\gamma^{0}=\begin{bmatrix}
\mathbb{I}_{2} & 0 \\
0 & -\mathbb{I}_{2}
\end{bmatrix};\;\gamma^{k}=\begin{bmatrix}
0 & \sigma^{k} \\
-\sigma^{k} & 0
\end{bmatrix}.$$
It is easier to write $-i\hbar \nabla_{k}$ as $\underline{p}_{k}$ and $\underline{\pi}=\underline{p}-e\underline{A}$.
$$i\hbar \gamma^{0} \frac{1}{c} \frac{{\partial \psi}}{\partial t}=-i\hbar\gamma^{k}\nabla_{k}\psi-e\gamma^{k}A_{k}\psi+e\gamma^{0} \frac{\phi}{c}\psi+mc^2\psi.$$
$$\frac{i\hbar}{c}\begin{bmatrix}
\mathbb{I}_{2} & 0 \\
0 & -\mathbb{I}_{2}
\end{bmatrix} \frac{\partial}{\partial t}\begin{bmatrix}
\tilde{\Phi} \\
\tilde{\chi}
\end{bmatrix}=\begin{bmatrix}
\left( mc+\frac{e\phi}{c} \right)\mathbb{I}_{2} & \underline{\sigma}\cdot \underline{\pi} \\
-\underline{\sigma}\cdot \underline{\pi} & \left( mc-\frac{e\phi}{c} \right)
\end{bmatrix}\begin{bmatrix}
\tilde{\Phi} \\
\tilde{\chi}
\end{bmatrix}.$$
As with the Klein-Gordon equation, define a new energy,
$$\psi=\begin{bmatrix}
\tilde{\Phi} \\
\tilde{\chi}
\end{bmatrix}=e^{-imc^2t/\hbar}\begin{bmatrix}
\Phi \\
\chi
\end{bmatrix}$$
$$\therefore \frac{i\hbar}{c} \frac{\partial}{\partial t}\begin{bmatrix}
\tilde{\Phi} \\
\tilde{\chi}
\end{bmatrix}=\frac{i\hbar}{c}\left( -\frac{im}{\hbar}c^2\begin{bmatrix}
\Phi \\
\chi
\end{bmatrix}+\frac{\partial}{\partial t}\begin{bmatrix}
\Phi \\
\chi
\end{bmatrix} \right)e^{-imc^2t/\hbar}.$$
$$=e^{-imc^2t/\hbar}\left( \frac{i\hbar}{c} \frac{\partial}{\partial t}\begin{bmatrix}
\Phi \\
\chi
\end{bmatrix}+mc \begin{bmatrix}
\Phi \\
\chi
\end{bmatrix} \right).$$
Substituting this into the Dirac equation gives
$$\frac{i\hbar}{c}\begin{bmatrix}
\mathbb{I}_{2} & 0 \\
0 & -\mathbb{I}_{2}
\end{bmatrix} \frac{\partial}{\partial t}\begin{bmatrix}
\Phi \\
\chi
\end{bmatrix}=\begin{bmatrix}
\frac{e\phi}{c}\mathbb{I}_{2} & -\underline{\sigma}\cdot \underline{\pi} \\
-\underline{\sigma}\cdot \underline{\pi} & \left( 2mc-\frac{e\Phi}{c} \right)\mathbb{I}_{2}
\end{bmatrix}\begin{bmatrix}
\Phi \\
\chi
\end{bmatrix}.$$
Take the non-relativistic limit,
$$E=i\hbar \frac{{\partial \chi}}{\partial t}\ll mc^2\chi;\;e\phi \chi\ll mc^2\chi.$$
Start with the lower row:
$$\frac{i\hbar}{c}\left( -\frac{{\partial \chi}}{\partial t} \right)=-\underline{\sigma}\cdot \underline{\pi}+\left( 2mc-\frac{e\phi}{c} \right)\chi \implies{2}mc\chi=\underline{\sigma}\cdot \underline{\pi}\Phi$$
$$\implies \chi=\frac{{\underline{\sigma}\cdot \underline{\pi}}}{2mc}\Phi \thicksim \frac{v}{c}$$
$\implies \chi$ is small.
In the non-relativistic limit, $\chi\ll \Phi$.

For the first row,
$$\frac{i\hbar}{c} \frac{{\partial \Phi}}{\partial t}=\frac{e\phi}{c}\Phi+\underline{\sigma}\cdot \underline{\pi}\chi$$
$$i\hbar \frac{{\partial \Phi}}{\partial t}=e\phi \Phi+c\underline{\sigma}\cdot \underline{\pi}\chi=e\phi \Phi+\frac{(\underline{\sigma}\cdot \underline{\pi})^2}{2m}\Phi.$$
Evaluating the dot product,
$$(\underline{\sigma}\cdot \underline{\pi})^2=|\underline{\pi}|^2+i(\underline{\pi}\times \underline{\pi})\cdot\underline{\sigma}.$$
As $\pi$ is an operator, the cross product is not necessarily zero.
$$(\underline{\pi}\times \underline{\pi})_{i}=\epsilon_{ijk}\pi_{i}\pi_{k}=\epsilon_{ijk}(p_{j}-eA_{j})(p_{k}-eA_{k})$$
$$=-e\epsilon_{ijk}(A_{j}p_{k}+p_{j}A_{k})=ei\hbar\epsilon_{ijk}\left( A_{j} \frac{\partial}{\partial x^{k}}+\frac{\partial}{\partial x^{j}}A_{k} \right)$$
$$=ei\hbar\epsilon_{ijk}\left( \cancel{A_{j} \frac{\partial}{\partial x^{k}}}+\cancel{A_{k} \frac{\partial}{\partial x^{j}}}+\frac{\partial A_{k}}{\partial x^{j}} \right).$$
$$\therefore (\underline{\pi}\times \underline{\pi})_{i}=ei\hbar\epsilon_{ijk} \frac{{\partial A_{k}}}{\partial x^{j}}=i\hbar e(\underline{\nabla}\times \underline{A})_{i}=i\hbar e\underline{B}_{i}.$$
$$\therefore \underline{\sigma}\cdot \underline{\pi}=|\underline{\pi}|^2-e\hbar\underline{\sigma}\cdot \underline{B}$$
$$\implies i\hbar \frac{{\partial \Phi}}{\partial t}=\left( \frac{|\underline{\pi}|^2}{2m}-\frac{e\hbar{\underline{\sigma}\cdot \underline{B}}}{2m}+e\phi \right)\Phi.$$
This is the Pauli-equation for spin-$\frac{1}{2}$ particles.

We aimed for a first order differential equation consistent with $E^2=p^2c^2+m^2c^4$ but spin has naturally appeared, but this goes further.

Consider the constant magnetic field with vector potential
$$\underline{A}=\frac{1}{2}\underline{B}\times \underline{x}$$
and introduce 
$$\underline{S}=\frac{\hbar}{2}\underline{\sigma};\;\underline{L}=\underline{x}\times \underline{p}.$$
This gives the Pauli equation
$$i\hbar \frac{\partial \Phi}{\partial t}=\left( \frac{|\underline{p}|^2}{2m}+\frac{e^2|\underline{A}|^2}{2m}-\frac{e}{2m}(\underline{L}+2\underline{S})\cdot \underline{B}+e\phi \right)\Phi.$$
The factor of 2 in front of the $\underline{S}$ is the Landé g-factor, which the Dirac equation predicts to be $g=2.$
Adjusting for the quantum corrections the precise value is
$$a_{e}=\frac{{g_{e}-2}}{2}=0.00115965218073$$
and the Dirac prediction is $0.00115965218178$.
This is one of the most precise tests in physics.

The correction for the muon is larger as it is harder to observe due to its short lifetime.
