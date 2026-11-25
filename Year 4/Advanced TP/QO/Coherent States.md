The [number states](Creation%20and%20Annihilation%20Operators.md) are defined as eigenstates of Hamiltonian $(3.6)$,
$$\hat{H}=\sum_{\vec{k},s}\hbar \omega_{k}\left( \hat{a}^{\dagger}_{\vec{k}s}\hat{a}_{\vec{k}s}+\frac{1}{2} \right).\tag{3.6} $$
In principle, this Hamiltonian can have an infinitely high energy eigenvalues. Consider the quantised electric-field
$$\hat{\vec{E}}(\vec{r},t)=i\sum_{\vec{k},s}\sqrt{  \hbar \frac{\omega_{\vec{k}}}{2\varepsilon_{0}V} }\vec{e}_{\vec{k}s}[\hat{a}_{\vec{k}s}e^{ i\vec{k}\cdot \vec{r} }-\text{H.c.}]\tag{3.10} .$$Applying this to the number operators show that the mean electric field is zero as all terms change the photon number which leaves $\braket{ n_{i} | n_{j} }=\delta_{ij}$.

The creation and annihilation operators can be used to define the first and second quadratures through $\hat{a}=\hat{X}_{1}+i\hat{X}_{2}$. The quadrature operators are defined by
$$\begin{matrix}
\hat{X}_{1}=\frac{1}{2}(\hat{a}+\hat{a}^{\dagger}), & \hat{X}_{2}=\frac{i}{2}(\hat{a}^{\dagger}-\hat{a}), & [\hat{X}_{1},\hat{X}_{2}]=\frac{i}{2}
\end{matrix}.\tag{4.1} $$
The quadrature uncertainties relate to initial values in a classical-like way. Uncertainties are equally distributed between quadratures. This can be used to give quasi-classical states.

Various quantities can be defined for the quadrature operators:
- Mean
$$\begin{matrix}
\alpha_{1}=\langle \hat{X}_{1} \rangle , & \alpha_{2}=\langle \hat{X}_{2} \rangle .
\end{matrix}\tag{4.2} $$
- Variance
$$\begin{matrix}
\Delta X_{1}^2=\langle (\hat{X}_{1}-\alpha_{1})^2 \rangle , & \Delta X_{2}^{2}=\langle (\hat{X}_{2}-\alpha_{2})^2 \rangle 
\end{matrix} .\tag{4.3} $$
- Covariance
$$\Delta X_{1}X_{2}=\frac{1}{2}\langle (\hat{X}_{1}-\alpha_{1})(\hat{X}_{2}-\alpha_{2})-(\hat{X}_{2}-\alpha_{2})(\hat{X}_{1}-\alpha_{1}) \rangle .\tag{4.4} $$
Also we get from the definition of quadrature operators,
$$\alpha=\alpha_{1}+i\alpha_{2}=\langle \hat{a} \rangle .\tag{4.5} $$
It is also useful to define shifted creation and annihilation operators:
$$\begin{matrix}
\hat{b}=\hat{a}-\alpha, & \hat{b}^{\dagger}=\hat{a}^{\dagger}-\alpha ^{*}
\end{matrix}\tag{4.6} $$
with the same commutator relation $[\hat{b},\hat{b}^{\dagger}]=1$. In the [Heisenberg Picture](Quantum%20and%20Classical%20Dynamics.md) it takes the form
$$\hat{b}(t)=\hat{b}(0)e^{ -i\omega t }.\tag{4.7} $$
From this we can get the time evolution of the variances,
$$\Delta X_{1}^2=\frac{1}{4}[\langle \hat{b}^{\dagger}(0)\hat{b}(0)+\text{H.c.} \rangle +(\langle \hat{b}^{\dagger}(0)^2 \rangle e^{ i{2}\omega t }-\text{H.c.})]\tag{4.8} ,$$
$$\Delta X_{2}^2=\frac{1}{4}[\langle \hat{b}^{\dagger}(0)\hat{b}(0)+\text{H.c.} \rangle -(\langle \hat{b}^{\dagger}(0)^2 \rangle e^{ i{2}\omega t }-\text{H.c.})]\tag{4.9} ,$$
$$\Delta X_{1}X_{2}=\frac{1}{4}[\langle \hat{b}^{\dagger}(0)^2 \rangle e^{ i{2}\omega t }-\text{H.c.}]\tag{4.10} .$$
Time independence requires $\langle \hat{b}^{\dagger}(0)^2 \rangle=\langle \hat{b}(0)^2 \rangle=0$ so we need to minimise $\langle \hat{b}^{\dagger}(0)\hat{b}(0)+\text{H.c.} \rangle$. This is equivalent to minimising $\langle \hat{b}^{\dagger}\hat{b} \rangle$ where $\hat{b}^{\dagger}\hat{b}$ is a form of number operator.
The minimum eigenvalue is 0, whose state is called the minimising state $\ket{\alpha}$.
In analogy to $\hat{a}\ket{0}=0$, $\hat{b}\ket{\alpha}=0\implies \hat{a}\ket{\alpha}=\alpha \ket{\alpha}$.

$\ket{\alpha}$ are coherent states, which are eigenstates of the annihilation operator.

Factorising property:
$$\bra{\alpha} \hat{a}^{\dagger n}\hat{a}^{m}\ket{\alpha} =\alpha ^{*n}\alpha^{m}=\bra{\alpha} \hat{a}^{\dagger}\ket{\alpha}^{n}\bra{\alpha} \hat{a}\ket{\alpha} ^{m}.\tag{4.11}  $$
The factorising property shows that the expectation value of the product equals the product of the expectation values, which is a classical property.

$\ket{\alpha}$ can be decomposed into number states
$$\ket{\alpha} =e^{ -|\alpha|^2/2 }\sum_{n=0}^{\infty} \frac{\alpha^{n}}{\sqrt{ \alpha! }}\ket{n} .\tag{4.12} $$
The inner product is then
$$\braket{ \alpha | \beta } =e^{ \alpha ^{*}\beta -|\alpha|^2/2-|\beta|^2/2}\implies |\braket{ \alpha | \beta } |^2=e^{ -|\alpha-\beta|^2 }.\tag{4.13} $$
This shows two coherent states are exactly orthogonal, but they are approximately orthogonal for large $|\alpha-\beta|$.

The identity operator in terms of coherent states is
$$\hat{\mathbb{1}}=\frac{1}{\pi}\int d^2\alpha \ket{\alpha} \bra{\alpha} .\tag{4.14} $$
The factor of $\frac{1}{\pi}$ is a signifier of over completeness.

A general operator $\hat{O}$ in terms of coherent states is then
$$\hat{O}=\frac{1}{\pi^2}\int d^2\alpha d^2\beta\;\ket{\alpha}\bra{\alpha} \hat{O}\ket{\beta}\bra{\beta} \tag{4.15}   =\frac{1}{\pi^2}\int d^2\alpha d^2\beta \;\ket{\alpha}\bra{\beta} O(\alpha ^{*},\beta)e^{ -|\alpha|^2/2-|\beta|^2/2 }. $$
From
$$\bra{\alpha} \hat{O}\ket{\alpha} =e^{ -|\alpha|^2 }\sum_{n,m}\bra{n} \hat{O}\ket{m} \frac{\alpha ^{*n}\alpha^{m}}{\sqrt{ n!m! }}\tag{4.16} $$we obtain the inverse expression
$$\bra{n} \hat{O}\ket{m} =\frac{1}{\sqrt{ n!m! }} \frac{\partial^n}{\partial\alpha ^{*n}} \frac{\partial^{m}}{\partial\alpha^{m}}(e^{ \alpha\alpha ^{*} }\bra{\alpha} \hat{O}\ket{\alpha} )|_{\alpha=0}.\tag{4.17} $$
All matrix elements in the number basis obtained from diagonal elements in the coherent states basis.

From number decomposition, we get a probability of observing $n$ photons,
$$P_{n}=\frac{{e^{ -|\alpha|^2/2 }|\alpha|^{2n}}}{n!}\tag{4.18} $$which is a Poisson distribution of mean $|\alpha|^2$.

To generate coherent states from the vacuum, it is relatively straightforward to show
$$\ket{\alpha} =e^{ \alpha \hat{a}^{\dagger}-\alpha ^{*}\hat{a} }\ket{0}.\tag{4.19}  $$
where $e^{ \alpha \hat{a}^{\dagger}-\alpha ^{*}\hat{a} }$ is the unitary displacement operator.

In quadratures the unitary displacement operator is given by $e^{ i 2(\alpha_{2}\hat{X}_{1}-\alpha_{1}\hat{X}_{2}) }$. Similarly,
$$\braket{ X_{1} | \alpha } =\bra{X_{1}} e^{ i 2(\alpha_{2}\hat{X}_{1}-\alpha_{1}\hat{X}_{2}) }\ket{0}=e^{ i\alpha_{1}\alpha_{2} }e^{ i{2}\alpha_{2}X_{1} }\left( \frac{2}{\pi} \right)^{1/4}e^{ -(X_{1}-\alpha_{1})^2 }.\tag{4.20}  $$
This is a Gaussian wave packet centred at position $X_{1}=\alpha_{1}$ with mean momentum $X_{2}=\alpha_{2}$.