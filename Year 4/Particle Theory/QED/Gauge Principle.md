Consider the [Dirac Lagrangian](Dirac%20Equation.md)
$$\mathcal{L}=\bar{\psi}(i\partial \!\!\!/-m)\psi \tag{7.1} .$$
Transform the matter fields using
$$\begin{matrix}
\psi\to\psi'=e^{ i\vartheta }\psi & \bar{\psi}\to \bar{\psi}'=e^{ -i\vartheta }\bar{\psi}
\end{matrix}\tag{7.2} .$$Substituting these into $(7.1)$ does not change the Lagrangian, so it is invariant under this transformation. This is a global $U(1)$ symmetry.

For interactions, the global symmetries become local symmetries, where $\vartheta$ becomes dependent on spacetime coordinates. This breaks the invariance in the Lagrangian,
$$\mathcal{L}\to \mathcal{L}'=\bar{\psi}(i\partial \!\!\!/-m)\psi-\bar{\psi}\gamma^\mu \psi(\partial_{\mu}\vartheta)\tag{7.3} .$$
This leaves an additional $\partial_{\mu}\vartheta$ term which needs to be compensated for. Consider the interaction Lagrangian $\mathcal{L}+\mathcal{L}_{int}$ where $\mathcal{L}_{int}=-ie\bar{\psi}\gamma^\mu \psi A_{\mu}$. Since we have introduced a gauge field, we need to [include a](Photons) $\mathcal{L}_{A}=-\frac{1}{4}F_{\mu \nu}F^{\mu \nu}$ term. Consider the gauge transformation$$A_{\mu}(x)\to A_{\mu}'(x)=A_{\mu}(x)-\partial_{\mu}\Lambda(x)=A_{\mu}-\frac{i}{e}\partial_{\mu}\vartheta \tag{7.4} .$$This implies that $\Lambda$ and $\vartheta$ are connected up to a scale factor.
Therefore to compensate for the $\partial_{\mu}\vartheta$ term from the local symmetry, we introduce a gauge field $A^\mu$ with the correct transformation behaviour
![[Pasted image 20260113183840.png]]
This is accounted for by introducing the covariant derivative
$$i\mathcal{D}^{\mu}=i\partial^\mu-eA^\mu.\tag{7.5} $$
This gives the Lagrangian
$$\mathcal{L}=\bar{\psi}(i\mathcal{D}\!\!\!/-m)\psi \tag{7.6}. $$
