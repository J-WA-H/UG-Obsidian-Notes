The Lagrangian of a scalar field can be decomposed into two parts,
$$\mathcal{L}=\mathcal{L}_{0}+\mathcal{L}_{int}\tag{7.1} $$where $\mathcal{L}_{0}$ is the free Lagrangian [(1.14)](Classical%20Field%20Theory.md) and the field interactions are given by $\mathcal{L}_{int}$, which is normally given as some polynomial in $\phi$,
$$\mathcal{L}_{int}=\sum_{n=3}^{N} \frac{\lambda_{n}}{n!}\phi^n.\tag{7.2} $$
$\lambda_{n}$ is a coupling constant which have dimensions. For $\lambda\ll{1}$, we have Feynman perturbation theory.

To calculate the mass dimensions, consider the quantity,
$$S=\exp\left[ -\int dtL \right]\tag{7.3} $$where the exponent must be dimensionless. As $[dt]=-1$, in natural units, this means $[L]=1$. From the definition of the Lagrangian density $(1.9)$, $[\mathcal{L}]=4$. Using the Lagrangian
$$\mathcal{L}=\frac{1}{2}(\partial_{\mu}\phi)(\partial^{\mu}\phi)-m^2\phi^2+\sum_{n\geq 3} \frac{\lambda_{n}}{n!}\phi^{n}.\tag{7.4} $$
From this since $[\partial_{\mu}]=1$, $[\phi]=1$ which gives from $\mathcal{L}_{int}$, $[\lambda_{3}]=1$ and $[\lambda_{4}]=0$.

In most interacting field theories, like the Higgs potential, $\mathcal{L}_{int}$ only goes up to $\lambda_{4}$. After [quantisation](Quantisation%20of%20Fields.md) The $\phi^4$ term includes the sum of the different products of 4 creation and annihilation operators, e.g. $\hat{a}^{\dagger}\hat{a}^{\dagger}\hat{a}^{\dagger}\hat{a}^{\dagger},\hat{a}^{\dagger}\hat{a}^{\dagger}\hat{a}^{\dagger}\hat{a},$ etc. 

The experimental way to describe interacting fields is through the cross-section,
$$\sigma_{i\to f}\propto |\mathcal{M}_{i\to f}|^2\tag{7.5} $$where the matrix element
$$\mathcal{M}_{i\to f}=\braket{ f | i } .\tag{7.6} $$
The transition for the states $i\to f$ is given by the S-matrix.

For interactions, the Lagrangian is no longer quadratic in $\phi$ so the solution is no longer a plane wave.

Assume that the field starts as free, then interacting, then free again at large distances and late times. We can't assume that the initial and final free fields are the same
$$\phi(\vec{x},t)\xrightarrow{t\to \pm\infty}\phi^{in}_{out}(\vec{x},t).\tag{7.7} $$Both in and out fields satisfy the Klein-Gordon equation. The in field takes the form
$$\hat{\phi}_{in}=\int \frac{d^3k}{(2\pi)^32E_{k}}[\hat{a}_{k,in}e^{ -ik_{\mu}x^{\mu} }+\hat{a}^{\dagger}_{k,in}e^{ ik_{\mu}x^{\mu} }]\tag{7.8} .$$
$\ket{f}$ and $\ket{i}$ are in different [Fock spaces](Normal%20Ordering.md) but with one-to-one correspondence.

Assume a vacuum $\ket{0}=\ket{0}_{in}=\ket{0}_{out}$. Due to the one-to-one correspondence,
$$\hat{\phi}_{in}(x)=S\hat{\phi}_{out}(x)S^{\dagger}\tag{7.9} $$where the S-matrix is a unitary matrix. The S-matrix is defined as
$$\braket{ f_{out} | i_{in} } = \bra{f_{out}} S_{f\rightarrow i}\ket{i_{out}} =S_{fi}=\bra{0} (\hat{a}_{out}(p_{1})\dots\hat{a}_{out}(p_{n}))\hat{a}^{\dagger}_{in}(k_{1})\hat{a}^{\dagger}_{in}(k_{2})\ket{0} .\tag{7.10} $$
![[Pasted image 20251102164408.png]]
The $S$-matrix transfers an out state to an in state,
$$\ket{in} =\hat{S}\ket{out}.\tag{7.11}  $$
