We can write objects that are invariant under Lorentz transformations, e.g. the Minkowski norm.

Consider Lorentz invariance involving [spinors](Dirac%20Equation%20Derivation.md).
Consider $\psi ^{\dagger}\psi$ as a first guess.
As Lorentz rotations are Hermitian, $S^{\dagger}(R)S(R)=\mathbb{I}_{4}$
$$\implies \psi ^{\dagger}\psi=\psi'^{\dagger}S^{\dagger}(R)S(R)\psi'=\psi'^{\dagger}\psi'.$$
The spinor is invariant under a rotation.

For a boost, $S(R)$ is not Hermitian so $S^{\dagger}(R)S(R)\neq \mathbb{I}_{4}$, so the spinor is not invariant under a boost.

Define the adjoint spinor,
$$\bar{\psi}=\psi ^{\dagger}\gamma^{0}.$$
Consider how this transforms
$$\psi'=S\psi \implies \psi'^{\dagger}=\psi ^{\dagger}S^{\dagger}\implies \bar{\psi}'=\psi ^{\dagger}S^{\dagger}\gamma^{0}.$$
It can be shown that $S^{\dagger}\gamma^{0}=b\gamma^{0}S^{-1}$ where
$$b=\begin{cases}
1 & \Lambda^{0}_{\;0}\geq 1 \\
-1 & \Lambda^{0}_{\;0}\leq 1
\end{cases}.$$
This is [proper orthochronous](Relativistic%20Wave%20Equations.md).
$$\bar{\psi}'=\psi ^{\dagger}\gamma^{0}S^{-1}$$
$$\implies \bar{\psi}'\psi'=\psi ^{\dagger}\gamma^0S^{-1}S\psi=\bar{\psi}\psi.$$
This is Lorentz invariant.
Generalising this analysis finds quantities that are Lorentz invariant.

Under $\psi'=S(\Lambda)\psi$,
$$\bar{\psi}'\psi'=\bar{\psi}\psi\to \text{Scalar}$$
$$\bar{\psi}'\gamma^{\mu}\psi'=\Lambda^{\mu}_{\;\alpha}\bar{\psi}\gamma^{\alpha}\psi\to\text{4-vector}$$
$$\bar{\psi}'\sigma^{\mu \nu}\psi'=\Lambda^{\mu}_{\;\alpha}\Lambda^{\nu}_{\;\beta}\bar{\psi}\sigma^{\alpha\beta}\psi\to\text{Tensor}$$
where
$$\sigma^{\mu \nu}=\frac{1}{2}[\gamma^{\mu},\gamma^{\nu}].$$
We can find Lorentz invariants by contraction of the space-time indices with other 4-vectors.

Example: [[4-Potential]],
$$A_{\mu}\bar{\psi}\gamma^{\mu}\psi.$$
This describes the interaction of photons with charge particles, e.g. electrons.

$$\bar{\psi}_{1}\gamma^{\mu}\psi_{2}\bar{\psi}_{3}\gamma_{\mu}\psi_{4}$$
is the Fermi theory of the weak interaction.
