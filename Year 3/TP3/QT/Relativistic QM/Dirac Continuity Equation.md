Like with the [Klein-Gordon equation](Interpreting%20Klein-Gordon%20Solutions.md), a continuity equation can be derived to give the probability density and current.

Define the probability density $\rho$ as the norm of a [Dirac spinor](Dirac%20Equation%20Derivation.md),
$$\rho=\begin{bmatrix}
\psi_{1}^{*} & \psi_{2}^{*} & \psi_{3}^{*} & \psi_{4}^{*}
\end{bmatrix}\begin{bmatrix}
\psi_{1} \\
\psi_{2} \\
\psi_{3} \\
\psi_{4}
\end{bmatrix}=|\psi_{1}|^2+|\psi_{2}|^{2}+|\psi_{3}|^{2}+|\psi_{4}|^{2}\geq 0.$$
By definition $\rho\geq 0$ so this fixes one problem of the Klein-Gordon equation.

Take time derivative,
$$\psi ^{\dagger} \frac{ \partial \psi }{ \partial t }+\frac{ \partial \psi ^{\dagger} }{ \partial t } \psi  = \frac{ \partial \rho }{ \partial t }. $$
From the Dirac equation,
$$\psi ^{\dagger} \frac{ \partial \psi }{ \partial t }=\psi ^{\dagger} \frac{1}{i\hbar}H_{D}\psi=\psi ^{\dagger}\left( -c\alpha^{k}\underline{\nabla}^{k}+\frac{mc^2}{i\hbar}\beta \right).$$
Take Hermitian conjugate of the Dirac equation,
$$\frac{ \partial \psi ^{\dagger} }{ \partial t } = -c(\underline{\nabla}\psi ^{\dagger})\cdot\underline{\alpha}\psi-\frac{mc^2}{i\hbar}\psi ^{\dagger}\beta \psi.$$
$$\frac{ \partial \rho }{ \partial t } =-c\psi ^{\dagger}\underline{\alpha}\cdot \underline{\nabla}\psi-c(\underline{\nabla}\psi ^{\dagger})\cdot\underline{\alpha}\psi=-c\underline{\nabla}\cdot(\psi ^{\dagger}\underline{\alpha}\psi)$$
$$\implies \frac{ \partial \rho }{ \partial t }+\underline{\nabla}\cdot \underline{j}=0 $$
where $\rho=\psi ^{\dagger}\psi$, $\underline{j}=c\psi ^{\dagger}\underline{\alpha} \psi$.
This gives a valid continuity equation with a positive definite probability density. This appears to have solved one problem of the Klein-Gordon equation.