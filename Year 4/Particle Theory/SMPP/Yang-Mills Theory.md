A gauge symmetry leaves the action $S=\int d^4x\mathcal{L}$ invariant. A gauge symmetry is a local symmetry which is dependent on spacetime coordinates $U=U(x)$. For example, take the Dirac Lagrangian
$$\mathcal{L}=\sum \bar{\Psi}(i\gamma^\mu \partial_{\mu}-m)\Psi\tag{2.1} $$
where $\Psi=(\psi_{+},\psi_{-})^T$.
Applying the transformation gives
$$\mathcal{L}\to \bar{\Psi}U^{\dagger}U(i\gamma^\mu \partial_{\mu}-m)\Psi+\bar{\Psi}i\gamma^\mu(\partial_{\mu}U)\Psi\tag{2.2}. $$Since $U^{\dagger}U=1$, this gives an additional term to the Lagrangian,
$$iU\partial_{\mu}U=-\partial_{\mu}\theta T+\mathcal{O}(\theta^2)\tag{2.3} .$$Defining $\partial_{\mu}\to \mathcal{D}_{\mu}=\partial_{\mu}+igA_{\mu}$ with $A_{\mu}\to A_{\mu}-g^{-1}\partial_{\mu}\theta$. If $T=1\implies U=e^{ i\theta }\therefore U\partial_{\mu}U=-\partial_{\mu}\theta$, which cancels the gauge term.

This is QED, an abelian $U(1)$ symmetry.

For a [non-abelian](Non-Abelian%20Group%20Theory.md) theory,
$$A_{\mu}=A_{\mu}^{\,B}T_{B}\tag{2.4} $$which transforms as
$$A_{\mu}\to UA_{\mu}U^{\dagger}-\frac{i}{g}U\partial_{\mu}U^{\dagger}\tag{2.5}. $$
The transformed Lagrangian is
$$\mathcal{L}'=\underbrace{ \bar{\Psi}(i\gamma^\mu \partial_{\mu}-m)\Psi+\bar{\Psi}i\gamma^\mu igU^{\dagger}UA_{\mu}U^{\dagger}U\Psi }_{ \mathcal{L} }+\underbrace{ \bar{\Psi}i\gamma^\mu U^{\dagger}(\partial_{\mu}U)\Psi+\bar{\Psi}U^{\dagger}i\gamma^\mu i(-i)U(\partial_{\mu}U^{\dagger})\Psi }_{ U^{\dagger}\partial_{\mu}U+U\partial_{\mu}U^{\dagger}=\partial_{\mu}(U^{\dagger}U)=\partial_{\mu}(1)=0 }\tag{2.6} $$
$\therefore \mathcal{L}$ is symmetric.

We can't build invariance just from $A_{\mu}$. Define the field strength tensor
$$F_{\mu \nu}=-\frac{i}{g}[\mathcal{D}_{\mu},\mathcal{D}_{\nu}]=\partial_{\mu}A_{\nu}-\partial_{\nu}A_{\mu}+ig[A_{\mu},A_{\nu}]=(\partial_{\mu}A_{\nu}^{\,D}-\partial_{\nu}A_{\mu}^{\,D}-gf_{BCD}A_{\mu}^{\,B}A_{\nu}^{\,C})T_{D}\tag{2.7}. $$
This transforms as $F_{\mu \nu}\to UF_{\mu \nu}U^{\dagger}$.

The Yang-Mills Lagrangian is
$$\mathcal{L}_{YM}=-\frac{1}{2}\mathrm{Tr}[F^{\mu \nu}F_{\mu \nu}]+\bar{\Psi}(i\gamma_{\mu}\mathcal{D}^\mu-m)\Psi\tag{2.8}. $$The trace is equivalent to $-\frac{1}{4}F_{\mu \nu}^{\;\,a}F^{\mu \nu a}$, and $\mathrm{Tr}[T^aT^b]=\frac{1}{2}\delta^{ab}$. This then gives the QCD gauge Lagrangian,
$$\mathcal{L}_{gauge}=-\frac{1}{4}(\partial_{\mu}A_{\nu}^{\,a}-\partial_{\nu}A_{\mu}^{\,a})^2-\frac{1}{2}g_{s}f^{abc}(\partial_{\mu}A_{\nu}^{\,a}-\partial_{\nu}A_{\mu}^{\,a})A^{b\mu}A^{c\nu}-\frac{1}{4}g_{s}^2f^{abe}f^{cde}A_{\mu}^{\,a}A_{\nu}^{\,b}A^{c\mu}A^{d\nu}.\tag{2.9} $$
This Lagrangian allow both 3 and 4 gauge boson, in this case gluon, vertices
![[Pasted image 20260207153412.png]]
Each line is represented by a momentum, Lorentz index, and group index.

Consider the vertex
$$-\frac{1}{2}g_{s}f^{abc}g_{\rho \nu}(\partial_{\mu}A^{a\rho})A^{b\mu}A^{c\nu}=-\frac{1}{2}g_{s}f^{acb}g_{\mu \nu}(\partial_{\rho}A^{a\mu})A^{c\rho}A^{b\nu}=+\frac{1}{2}f^{abc}g_{\mu \nu}(\partial_{\rho}A^{a\mu})A^{c\rho}A^{b\nu}.\tag{2.10}$$using the anti-symmetry of the structure constant, $f^{abc}=-f^{acb}$.
$$\partial_{\rho}A^{a\mu}=\int _{\rho}(-ip_{\mu})A^a_{\,\mu}(p)e^{ -ipx }\tag{2.11} $$
with
$$\int_{\rho}\equiv \int \frac{d^4p}{(2\pi)^4}.\tag{2.12} $$
This can be used to get the Feynman rule for a 3 gluon vertex,
$$-ig_{s}f^{abc}[g_{\mu \nu}(p-q)_{\rho}+g_{\nu \rho}(q-r)_{\mu}+g_{\rho \mu}(r-p)_{\nu}]\tag{2.13} $$where $p,q,r$ are the momenta.

For a 4 gluon vertex,
$$-ig_{s}^2[f^{abe}f^{cde}(g_{\mu \nu}g_{\rho\sigma}-g_{\mu\sigma}g_{\nu \rho}+(b\leftrightarrow c,\rho\leftrightarrow \nu)+(b\leftrightarrow d,\sigma\leftrightarrow \nu))].\tag{2.14} $$
