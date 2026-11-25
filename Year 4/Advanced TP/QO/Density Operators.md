Consider a 2-state quantum system, $\ket{\psi}_{2}=a\ket{\varphi_{0}}+b\ket{\varphi_{1}}$,
$$\implies \rho_{2}=\begin{bmatrix}
b \\
a
\end{bmatrix}\otimes \begin{bmatrix}
b^{*} & a^{*}
\end{bmatrix}=\begin{bmatrix}
b(b^{*} & a^{*}) \\
a(b^{*} & a^{*})
\end{bmatrix}=\begin{bmatrix}
|b|^2 & ba^{*} \\
ab^{*} & |a|^2
\end{bmatrix}\tag{5.1} .$$This is the matrix representation of the density operator in the basis $\{ \ket{\varphi_{0}},\ket{\varphi_{1}} \}$. This two state system has a $2\times 2$ matrix for $\rho$.

The density operator must be Hermitian so the diagonal elements must be real.

Recall the [Von-Neumann equation](Quantum%20and%20Classical%20Dynamics),
$$i\hbar \frac{d\rho}{dt}=[\hat{H},\rho]\tag{1.8} .$$
Global phase has no measurable consequence on $\rho$.

Consider probabilities $P_{k}$ for a system to exist or be prepared in states $\ket{\psi_{k}}$. This corresponds to a mixed states density operator,
$$\rho=\sum_{k}P_{k}\ket{\psi_{k}} \bra{\psi_{k}} \tag{5.2} .$$
Mixed states cannot be described in a single wavefunction. 

Compare mixed and pure states:
For a pure (superposition) state,
$$\rho_{p}=\sum_{k}\sqrt{ P_{k} }\ket{\psi_{k}} \sum_{k'}\sqrt{ P_{k'} }\bra{\psi_{k'}} \tag{5.3} $$so a mixed state has a diagonal $\rho$ while a mixed state isn't in a basis of $\ket{\psi_{k}}$,
$$\rho_{m}=\begin{bmatrix}
P_{1} & 0 \\
0 & P_{0}
\end{bmatrix},\;\rho_{p}=\begin{bmatrix}
P_{1} & \sqrt{ P_{0}P_{1} } \\
\sqrt{ P_{0}P_{1} } & P_{0}
\end{bmatrix}.\tag{5.4} $$
Diagonal elements are populations (probabilities to measure system in a particular basis). Off-diagonal elements commonly  
referred to as coherences. These elements however are basis dependent.

Expectation values in general are defined by the trace
$$\langle \hat{O} \rangle =\mathrm{Tr}(\rho \hat{O})\tag{5.5}. $$If $\rho$ is Hermitian there is always one basis in which it is diagonal, $\ket{\chi_{k}}$. Probability weighted sum ($\rho_{k}$) of expectation values is
$$\bra{\chi_k}\hat{O}\ket{\chi_{k}} \tag{5.6} .$$
Probabilities must sum to 1 so $\mathrm{Tr}(\rho)=1$. Also $\mathrm{Tr}(\rho^2)\leq{1}$, with equality only for a pure state.

The Von-Neumann equation is linear in $\rho$ so extends easily to mixed states,
$$i\hbar \frac{d\rho}{dt}=i\hbar \frac{d}{dt}\left( \sum_{k}P_{k}\ket{\psi_{k}} \bra{\psi_{k}}  \right)=\sum_{k}P_{k}i\hbar \frac{d}{dt}\ket{\psi_{k}} \bra{\psi_{k}} =\sum_{k}P_{k}[\hat{H},\ket{\psi_{k}} \bra{\psi_{k}} ]=\left[ \hat{H},\sum_{k}P_{k}\ket{\psi_{k}}\bra{\psi_{k}}   \right]=[\hat{H},\rho].\tag{5.7} $$
The density operator can be expressed as an ensemble of [[Coherent States]],
$$\rho=\int d^2\alpha P(\alpha,\alpha ^{*})\ket{\alpha} \bra{\alpha}\tag{5.8}  .$$
Expectation values of normally ordered products $\hat{a}^{\dagger n}\hat{a}^{m}$ is given by
$$\langle \hat{a}^{\dagger n}\hat{a}^{m} \rangle =\int d^2\alpha P(\alpha,\alpha ^{*})\alpha ^{*n}\alpha^{m}.\tag{5.9} $$
This is the Glauber-Sudarshan P-representation.

The Husimi Q-representation is another way to look at the density operator.
Consider diagonal $\rho$ elements in an overcomplete coherent basis,
$$Q(\alpha,\alpha ^{*})=\frac{1}{\pi}\bra{\alpha} \rho \ket{\alpha}.\tag{5.10}  $$
Expectation values of antinormally ordered products $\hat{a}^{n}\hat{a}^{\dagger m}$ is given by
$$\langle \hat{a}^{n}\hat{a}^{\dagger m} \rangle=\int d^2\alpha Q(\alpha,\alpha ^{*})\alpha^{n}\alpha ^{*m} .\tag{5.11} $$
Recall the Wigner representation,
$$W=\frac{1}{\pi^2}\int d^2\lambda e^{ -\lambda ^{*}\alpha+\lambda\alpha ^{*} }\mathrm{Tr}(\rho e^{ \lambda ^{*}\hat{a}-\lambda \hat{a}^{\dagger} }).\tag{5.12} $$This yields the expectation values of symmetrically ordered products, for example
$$\frac{1}{2}\langle \hat{a}\hat{a}^{\dagger}+\hat{a}^{\dagger}\hat{a} \rangle =\int d^2\alpha W(\alpha,\alpha ^{*})\alpha\alpha ^{*}.\tag{5.13} $$
There is also a quadrature representation equivalent to Wigner's original function,
$$W(\alpha_{1},\alpha_{2})=\frac{1}{\pi^2}\iint d\lambda_{1}d\lambda_{2}\mathrm{Tr}(\rho e^{ i{2}[\lambda_{2}(\hat{X}_{1}-\alpha_{1})+\lambda_{1}(\hat{X}_{2}-\alpha_{2})] })\tag{5.14} .$$This yields expectation values of symmetrically ordered products of quadrature operators,
$$\frac{1}{2}\langle \hat{X}_{1}\hat{X}_{2}+\hat{X}_{2}\hat{X}_{1} \rangle =\iint d\alpha_{1}d\alpha_{2}W(\alpha_{1},\alpha_{2})\alpha_{1}\alpha_{2}\tag{5.15} .$$
$W(\alpha_{1},\alpha_{2})$ can be used to visualise the phase and number uncertainties
![[Pasted image 20251017133233.png]]
The annulus shows the number uncertainty and the triangle shows the phase uncertainty at the point $(\alpha_{1},\alpha_{2})$ since the point has an uncertainty radius.
Note $\alpha=|\alpha|e^{ i\theta }$ where $\theta$ is the phase angle.
The number variance is defined by
$$\langle \hat{N}^2 \rangle -\langle \hat{N} \rangle ^2=\langle \hat{N} \rangle =|\alpha|^2\tag{5.16}. $$
The standard deviation is then given by
$$\frac{\sqrt{ \langle \hat{N} \rangle  }}{\langle \hat{N} \rangle }=\frac{1}{|\alpha|}\tag{5.17} $$
which is negligible as $\langle \hat{N} \rangle\to \infty$.
There is always well defined mean number (centre circle of annulus) and mean phase (centre line of triangle) - both go through the centre of the point.
