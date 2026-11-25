Quantising a [[Classical Field Theory]] gives a quantum field theory. 

There is a canonical quantisation procedure:
- Coordinate $\phi(x)$ and conjugate momentum $\pi(x)$ become operators $\hat{\phi}(x),\hat{\pi}(x)$ with commutator relations
$$[\hat{\phi}(\vec{x},t),\hat{\pi}(\vec{y},t)]=i\hbar\delta^{(3)}(\vec{x}-\vec{y})\tag{4.1} $$
$$[\hat{\phi}(\vec{x},t),\hat{\phi}(\vec{y},t)]=0\tag{4.2} $$
$$[\hat{\pi}(\vec{x},t),\hat{\pi}(\vec{y},t)]=0\tag{4.3} .$$Where all these commutators are evaluated at the same time.

This is canonical quantisation, but also known as the method of second quantisation. This gives
$$\hat{\phi}(x)=\int \frac{d^3k}{(2\pi)^32k_{0}}[\hat{a}(k)e^{ -k_{\mu}x^{\mu} }+\hat{a}^{\dagger}(k)e^{ ik_{\mu}x^{\mu} }]\tag{4.4} $$and
$$\hat{\pi}(x)=\partial_{t}\hat{\phi}.\tag{4.5} $$
The [Hamiltonian](Hamiltonian%20Formulism.md) operator for a real quantum field theory is then
$$\hat{H}=\int d^3x(\hat{\pi}\hat{\dot{\phi}}-\hat{\mathcal{L}})=\frac{1}{2}\int d^3x(\hat{\pi}^2(x)+(\partial_{i}\hat{\phi}(x))^2+m^2\hat{\phi}^2(x)).\tag{4.6} $$
The $\hat{a}^{\dagger},\hat{a}$ are creation and annihilation operators of a particle with commutator relations
$$\begin{matrix}
[\hat{a}(\vec{k}),\hat{a}^{\dagger}(\vec{q})]=2E_{k}(2\pi)^3\delta^{(3)}(\vec{k}-\vec{q}), \\
[\hat{a}(\vec{k}),\hat{a}(\vec{q})]=0, \\
[\hat{a}^{\dagger}(\vec{k}),\hat{a}^{\dagger}(\vec{q})]=0.
\end{matrix}\tag{4.7} $$
The Hamiltonian can be rewritten in terms of $\hat{a},\hat{a}^{\dagger}$,
$$\hat{H}=\int \frac{d^3k}{(2\pi)^32E_{k}}E_{k} \frac{1}{2}(\hat{a}^{\dagger}(\vec{k})\hat{a}(\vec{k})+\hat{a}(\vec{k})\hat{a}^{\dagger}(\vec{k})).\tag{4.8} $$
These creation and annihilation operators can be written in terms of $\hat{\phi},\hat{\pi}$. Consider the combination of the field and its conjugate momentum to cancel $\hat{a}$ but leaves $\hat{a}^{\dagger}$,
$$k_{0}\hat{\phi}(x)-i\hat{\pi}(x)=\int \frac{d^3k}{(2\pi)^32E_{k}}(2k_{0}\hat{a}^{\dagger}(\vec{k})e^{ ik_{\mu}x^{\mu} }).\tag{4.9} $$This gives
$$\int d^3xe^{ i\vec{k}\cdot \vec{x} }(LHS)=\int d^3xe^{ i\vec{k}\cdot \vec{x} }\int \frac{d^3q}{(2\pi)^32E_{q}}2E_{q}\hat{a}^{\dagger}(\vec{q})e^{ iq_{0}x^{0}-i\vec{q}\cdot \vec{x} }=\int d^3xe^{ i(\vec{k}-\vec{q})\cdot \vec{x} }\int \frac{d^3q}{(2\pi)^32E_{k}}2E_{q}\hat{a}^{\dagger}(\vec{q})e^{ iq_{0}x^{0} }\tag{4.10} $$
$$=\int \frac{d^3q}{\cancel{(2\pi)^32E_{q}}}\cancel{2E_{q}}\hat{a}^{\dagger}(\vec{q})e^{ iq_{0}x^{0} }\cancel{(2\pi)^3}\delta^{(3)}(\vec{k}-\vec{q})=\hat{a}^{\dagger}(\vec{k})e^{ ik_{0}x^{0} }.\tag{4.11} $$
Rearranging this gives
$$\hat{a}^{\dagger}(\vec{k})=\int d^3xe^{ -ik_{\mu}x^{\mu} }(k_{0}\hat{\phi}(x)-i\hat{\pi}(x)).\tag{4.12} $$To find $\hat{a}$ take the Hermitian conjugate,
$$\hat{a}(\vec{k})=\int d^3xe^{ ik_{\mu}x^{\mu} }(k_{0}\hat{\phi}(x)+i\hat{\pi}(x)).\tag{4.13} $$
These can be used to derive the commutation relation,
$$[\hat{a}(\vec{k}),\hat{a}^{\dagger}(\vec{q})]=\int d^3x\int d^3y e^{ ik_{\mu}x^{\mu} }e^{ -iq_{\mu}y^{\mu} }[(k_{0}\hat{\phi}(x)+i\hat{\pi}(x)),(q_{0}\hat{\phi}(y)-i\hat{\pi}(y))]\tag{4.14} $$
Expand commutator,
$$[(k_{0}\hat{\phi}(x)+i\hat{\pi}(x)),(q_{0}\hat{\phi}(y)-i\hat{\pi}(y))]=k_{0}q_{0}\cancelto{0}{[\hat{\phi}(x),\hat{\phi}(y)]}-ik_{0}[\hat{\phi}(x),\hat{\pi}(y)]+iq_{0}[\hat{\pi}(x),\hat{\phi}(y)]+\cancelto{0}{[\hat{\pi}(x),\hat{\pi}(y)]}\tag{4.15} $$
$$=k_{0}\delta^{(3)}(\vec{x}-\vec{y})+q_{0}\delta^{(3)}(\vec{x}-\vec{y})=(k_{0}+q_{0})\delta^{(3)}(\vec{x}-\vec{y}).\tag{4.16} $$
This gives the commutator
$$[\hat{a}(\vec{k}),\hat{a}^{\dagger}(\vec{q})]=\int d^3x \int d^3ye^{ ik_{\mu}x^{\mu} }e^{ -iq_{\mu}x^{\mu} }(k_{0}+q_{0})\delta^{(3)}(\vec{x}-\vec{y})=\int d^3x e^{ i(k_{\mu}-q_{\mu})x^{\mu} }(k_{0}+q_{0})=2E_{k}(2\pi)^3\delta^{(3)}(\vec{k}-\vec{q}).\square \tag{4.17} $$
This same method can be used to derive the Hamiltonian $(4.8)$. Using the commutator relation the Hamiltonian can be rewritten in terms of just $\hat{a}^{\dagger}\hat{a}$,
$$\hat{H}=\int \frac{d^3k}{(2\pi)^32E_{k}}E_{k} (\hat{a}^{\dagger}\hat{a}+E_{k}(2\pi)^3\delta^{(3)}(\vec{k}-\vec{k})),\tag{4.18} $$
however, $\delta^{(3)}(\vec{k}-\vec{k})$ is infinite so this Hamiltonian cannot be used.