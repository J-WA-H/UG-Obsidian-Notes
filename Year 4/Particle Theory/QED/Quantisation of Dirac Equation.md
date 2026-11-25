In the same way to [[Quantisation of Fields]] for the Klein-Gordon equation, define the conjugate momentum from the [Lagrangian](Dirac%20Equation.md)$$\mathcal{L}=\bar{\psi}(i\stackrel{\leftrightarrow}{\partial \!\!\!/}-m)\psi \tag{1.10} .$$The conjugate momentum is$$\pi=\frac{{\partial \mathcal{L}}}{\partial \dot{\psi}}=\frac{i}{2}\bar{\psi}\gamma^{0}=\frac{i}{2}\psi ^{\dagger}\tag{3.1} $$and
$$\pi ^{\dagger}=\frac{{\partial \mathcal{L}}}{\partial \dot{\psi}^{\dagger}}=-\frac{i}{2}\psi.\tag{3.2} $$
This gives the Hamiltonian density
$$\mathcal{H}=\pi \dot{\psi}-\pi ^{\dagger}\dot{\psi}^{\dagger}-\bar{\psi}(i\stackrel{\leftrightarrow}{\partial \!\!\!/}-m)\psi.\tag{3.3} $$
To quantise the spinor fields, instead of demanding commutator relations, we demand the anticommutator relations
$$\{ \hat{\psi}_{\alpha}(\vec{x}),\hat{\pi}_{\beta}(\vec{y}) \}=\frac{i}{2}\{ \hat{\psi}_{\alpha}(\vec{x}),\hat{\psi}^{\dagger}_{\beta}(\vec{y}) \}=i\delta_{\alpha\beta}\delta^{(3)}(\vec{x}-\vec{y}).\tag{3.4} $$
Every other anticommutator relation vanishes. This then gives the field,
$$\hat{\psi}(\vec{x},t)=\sum_{i=1}^{2}\int \frac{d^3p}{(2\pi)^32p_{0}}[e^{ -ip_{\mu}x^{\mu} }\hat{b}^{(i)}(\vec{p})u^{(i)}(\vec{p}) +e^{ ip_{\mu}x^{\mu} }\hat{d}^{{\dagger}(i)}(\vec{p})v^{(i)}(\vec{p})].\tag{3.5} $$
The only difference from the the scalar case is that we take into account the spinor nature of $\psi$.
$$\hat{\psi}^{\dagger}(\vec{x},t)=\sum_{i=1}^{2}\int \frac{d^3p}{(2\pi)^32p_{0}}[e^{ -ip_{\mu}x^{\mu} }\hat{d}^{(i)}(\vec{p})v^{\dagger(i)}(\vec{p})+e^{ ip_{\mu}x^{\mu} }\hat{b}^{\dagger(i)}(\vec{p})u^{\dagger(i)}(\vec{p})].\tag{3.6} $$
Plugging this into the anticommutator relation gives
$$\{ \hat{b}^{(i)}(\vec{p}),\hat{b}^{\dagger(i)}(\vec{q}) \}=2p_{0}(2\pi)^3\delta^{(3)}(\vec{p}-\vec{q})\delta^{ij}=\{ \hat{d}^{(i)}(\vec{p}),d^{\dagger(j)}(\vec{q}) \}.\tag{3.7} $$
$\hat{b}^{\dagger(i)}/\hat{b}^{(i)}$ are creation/annihilation operators. They create/annihilate positive energy with momentum $\vec{p}$ and spin $i$. $\hat{d}^{\dagger(i)}/\hat{d}^{(i)}$ create and annihilate negative energy.

Acting on the vacuum state,
$$\hat{b}^{\dagger(i)}(\vec{p})\ket{0} = \ket{E>0,\vec{p},\text{spin}-i}.\tag{3.8}  $$
Acting two creation operators on the vacuum gives
$$\hat{b}^{\dagger(i)}(\vec{p})\hat{b}^{\dagger(i)}(\vec{p})\ket{0} =0\tag{3.9} $$as $\{ \hat{b}^{\dagger(i)}(\vec{p}),\hat{b}^{\dagger(i)}(\vec{p}) \}=0$.
Applying the same creation operator twice to the same state will always annihilate it. This is from Pauli's exclusion principle, since we are working with fermions.

In terms of the creation an annihilation operators, the Hamiltonian is
$$\hat{H}=\int d^3x\;\mathcal{H}=\int d^3x \frac{d^3p}{(2\pi)^32p_{0}} \frac{d^3q}{(2\pi)^32q_{0}}\sum_{i,j=1}^{2}(e^{ -ip_{\mu}x^{\mu} }\hat{d}^{(i)}(\vec{p})\bar{v}^{(i)}(\vec{p})+e^{ ip_{\mu}x^{\mu} }\hat{b}^{\dagger(i)}(\vec{p})\bar{u}^{(i)}(\vec{p}))(-i\gamma \stackrel{\leftrightarrow}{\nabla}+m)$$$$(e^{ -iq_{\mu}x^{\mu} }\hat{b}^{(j)}(\vec{q})u^{(j)}(\vec{q})+e^{ iq_{\mu}x^{\mu} }\hat{d}^{\dagger(i)}(\vec{q})v^{(j)}(\vec{q}))\tag{3.10} $$The $u,v$'s combine and annihilate each other as $\hat{b},\hat{d}$ have vanishing anticommutators. From this all cross terms go to zero.

To expand this, make use of the equation of motion,
$$(q\!\!\!/-m)u(\vec{q})=0\tag{3.11} $$from the Dirac equation. This means we can replace the middle term $(\vec{q}\cdot \vec{\gamma}+m)u(\vec{q})=q_{0}\gamma_{0}u(\vec{q})=-i\gamma\stackrel{\leftrightarrow}{\nabla}+m$. This gives the Hamiltonian
$$\hat{H}=\int \frac{d^3q}{(2\pi)^32q_{0}}q_{0}\sum_{i=1}^{2}[\hat{b}^{\dagger(i)}(\vec{q})\hat{b}^{(i)}(\vec{q})-\hat{d}^{(i)}(\vec{q})\hat{d}^{\dagger(i)}(\vec{q})].\tag{3.12} $$This is equivalent to the difference in the number operators for positive and negative energy states.

The [[Feynman Propagator]] for fermions is defined by
$$(i\partial \!\!\!/-m)G_{0}(x',x)=i\delta^{(4)}(x'-x)\tag{3.13} .$$To solve for the Green's function, move to momentum space,
$$(p\!\!\!/-m)\tilde{G}_{0}(p)=i.\tag{3.14} $$
This can then be solved to get
$$\tilde{G}_{0}(p)=\frac{1}{p\!\!\!/-m}=\frac{i(p\!\!\!/-m)}{p^2-m^2}=iS_{F}\tag{3.15}. $$The Propagator $S_{F}$ is given by the time-ordered product
$$iS_{F}(y,x)=\bra{0} T(\hat{\psi}(y)\hat{\psi}^{\dagger}(x))\ket{0} \tag{3.16} .$$This can be rewritten as
$$iS_{F}(x,y)=\bra{0} \hat{\psi}(y)\psi ^{\dagger}(x)\ket{0} \Theta(y_{0}-x_{0})-\bra{0} \hat{\psi}^{\dagger}(x)\hat{\psi}(y)\ket{0} \Theta(x_{0}-y_{0}).\tag{3.17} $$
