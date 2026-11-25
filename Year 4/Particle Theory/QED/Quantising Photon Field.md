Consider the Coulomb gauge,
$$\vec{\nabla}\cdot \vec{A}=0\tag{5.1}. $$
Without a source, the Lagrangian for [[Photons]] is
$$\mathcal{L}=-\frac{1}{4}F^{\mu \nu}F_{\mu \nu}\tag{5.2}. $$
Using the definition of the field strength tensor from the gauge field $A^{\mu}$, we can find the conjugate momenta,
$$\pi_{\nu}=\frac{{\partial \mathcal{L}}}{\partial \dot{A}_{\nu}}=\frac{{\partial \mathcal{L}}}{\partial(\partial_{0}A_{\nu})}=\begin{cases}
0 & \nu=0 \\
-E_{i} & \nu=i\neq 0
\end{cases}.\tag{5.3} $$
To quantise the gauge field, we demand the commutator
$$[\hat{A}_{i}(t,\vec{x}),\hat{\pi}_{j}(t,\vec{y})]=i\delta_{ij}\delta^{(3)}(\vec{x}-\vec{y}).\tag{5.4} $$
This cannot exist for the temporal component, $i=j=0$ as you cannot take the commutator of two zero-valued operators. 

To derive Gauss' law, consider the Lagrangian
$$\mathcal{L}^{(source)}=-\frac{1}{4}F^{\mu \nu}F_{\mu \nu}+j^{\mu}A_{\mu}\tag{5.6} .$$
The derivative
$$\frac{\partial \mathcal{L}}{\partial A^{0}}=0\implies \vec{\nabla}\cdot \vec{E}=0 \iff j^{\mu}=0.\tag{5.7} $$
Implement this in view of the commutator,
$$[\hat{A}_{i}(t,\vec{x}),\hat{E}_{j}(t,\vec{y})]=-i\delta_{ij}\delta^{(3)}(\vec{x}-\vec{y})\tag{5.8}. $$
To get Gauss' law,
$$\frac{\partial}{\partial y_{j}}[\hat{A}_{i}(t,\vec{x}),\hat{E}_{j}(t,\vec{y})]=\frac{\partial}{\partial y_{i}}i\delta_{ij}\delta^{(3)}(\vec{x}-\vec{y}).\tag{5.9} $$
Combing $\frac{\partial}{\partial y_{j}}$ and $\hat{E}_{j}$ gives $\vec{\nabla}\cdot \hat{\vec{E}}(t,\vec{y})=0$.

The right hand side of $(5.9)$ is not zero as the $\delta$-function has a non-zero derivative.

To try to solve this, demand the physical state $\ket{\psi}$ such that $\bra{\psi}\vec{\nabla}\cdot \vec{E}\ket{\psi}=0$. Maxwell's equations are only quantum mechanical averages.

To fix this we update the demand. Define the transverse delta-function as
$$\delta_{ij}\delta^{(3)}(\vec{x}-\vec{y})=\delta^{(3)}_{tr(ij)}(\vec{x}-\vec{y})=\int \frac{d^3k}{(2\pi)^3}e^{ i\vec{k}\cdot(\vec{x}-\vec{y}) }\left( \delta_{ij}-\frac{k_{i}k_{j}}{|\vec{k}|^2} \right)\tag{5.10}. $$
It is easy to show that the transverse delta-function's derivative vanishes. Differentiating with respect to position is equivalent to multiplying by $k_i$,
$$k_{i}\left( \delta_{ij}-\frac{k_{i}k_{j}}{|\vec{k}|^2} \right)=k_{j}-\frac{k^2k_{j}}{|k^2|}=k_{j}-k_{j}=0.\tag{5.11} $$
This can also be used to recover both Gauss' law and the gauge condition,
$$\left\{  \frac{\partial}{\partial x_{i}}, \frac{\partial}{\partial y_{j}} \right\}[\hat{A}_{i}(t,\vec{x}),\hat{E}_{j}(t,\vec{y})]=\left\{  \frac{\partial}{\partial x_{i}}, \frac{\partial}{\partial y_{j}}  \right\}i\delta^{(3)}_{tr(ij)}(\vec{x}-\vec{y})=0=[\vec{\nabla}\cdot \hat{\vec{A}}(t,\vec{x}),\hat{E}_{j}(t,\vec{y})]=[\hat{A}_{i}(t,\vec{x}),\vec{\nabla}\cdot \hat{\vec{E}}(t,\vec{y})].\tag{5.12} $$
This gives both Gauss' law, $\vec{\nabla}\cdot \vec{E}=0$, and the gauge condition $\vec{\nabla}\cdot \vec{A}=0$.

The field operator in this gauge is
$$\hat{\vec{A}}(x)=\sum_{k=1,2}\int \frac{d^3k}{(2\pi)^3}[\vec{\varepsilon}^{(\lambda)}(\vec{k})\hat{a}(\vec{k},\lambda)e^{ -ik_{\mu}x^{\mu} }+\vec{\varepsilon}^{(\lambda){\dagger}}\hat{a}^{\dagger}(\vec{k},\lambda)e^{ ik_{\mu}x^{\mu} }].\tag{5.13} $$
The commutator relation for the [creation and annihilation operators](Quantisation%20of%20Fields.md) is
$$[\hat{a}_{\lambda}(\vec{k}),\hat{a}^{\dagger}_{\kappa}(\vec{k})]=i\delta_{\lambda\kappa}\delta^{(3)}(\vec{k}-\vec{q})(2\pi)^32k_{0}\tag{5.14}. $$
Now consider the Lorenz gauge, with
$$\partial_{\mu}A^{\mu}=0\tag{5.15}. $$
In this gauge we can use the method of Lagrange multipliers,
$$\mathcal{L}=-\frac{1}{4}F^{\mu \nu}F_{\mu \nu}-\frac{\alpha}{2}(\partial_{\mu}A^{\mu})^2\tag{5.16} .$$The equation of motion of this Lagrangian is then
$$\partial_{\mu}\partial^{\mu}A^{\nu}-(1-\alpha)\partial^{\nu}(\partial_{\mu}A^{\mu})=4\pi j^{\nu}\tag{5.17} .$$
The middle term is not in Maxwell's equations so $\alpha$ has to be such that it drops out, $\alpha=1$. This is the Feynman gauge.

Now the conjugate momentum is
$$\pi_{\nu}=\begin{cases}
-\alpha g_{\nu 0}(\partial_{\mu}A^{\mu}) & \nu=0 \\
-E_{i} & \nu= i\neq 0
\end{cases}.\tag{5.18} $$
Now $\pi^{0}$ no longer vanishes. The commutator relation becomes
$$[\hat{A}_{\mu}(t,\vec{x}),\hat{\pi}_{\nu}(t,\vec{y})]=ig_{\mu \nu}\delta^{(3)}(\vec{x}-\vec{y})\tag{5.19} .$$
Imposing the Lorenz gauge on the commutator gives
$$\partial^{\mu}[\hat{A}_{\mu}(t,\vec{x}),\hat{\pi}_{\nu}(t,\vec{y})]=\partial^{\mu}(ig_{\mu \nu}\delta^{(3)}(\vec{x}-\vec{y}))\neq 0\tag{5.20} $$which violates the gauge condition. Quantising the gauge field gives $\partial_{\mu} \hat{A}^\mu=0$, which we do not want. We also cannot have $\partial_{\mu}\hat{A}^\mu \ket{\psi}=0$.

To solve this we demand the physical states satisfy $\bra{\psi}\partial_{\mu}A^{\mu}\ket{\psi}=0$.
For positive energies we demand, $\partial_{\mu}\hat{A}^\mu_{+}\ket{\psi}=0$ as $$\tag{5.21} \partial_{\mu}\hat{A}^\mu=\partial_{\mu}\hat{A}^\mu_{+}+\partial_{\mu}\hat{A}^\mu_{-}.$$
This gives $\bra{\psi}\partial_{\mu}\hat{A}^\mu_{-}=[\partial_{\mu}\hat{A}^\mu_{+}\ket{\psi}]^{\dagger}$. This can be used to obtain the field operator,
$$\tag{5.22} \hat{A}_{\mu}(x)=\int \frac{d^3k}{(2\pi)^32k_{0}}\sum_{\lambda=0}^3[\varepsilon_{\mu}^{(\lambda)}(\vec{k})\hat{a}_{\lambda}(\vec{k})e^{ -ik_{\mu}x^\mu }+\varepsilon_{\mu}^{(\lambda)*}(\vec{k})\hat{a}_{\lambda}^{\dagger}(\vec{k})e^{ ik_{\mu}x^\mu }]$$
where 4 linearly independent polarisation vectors are chosen,
$$\tag{5.23} \varepsilon_{\mu}^{(0)}=\begin{bmatrix}
1 \\
0 \\
0 \\
0
\end{bmatrix},\;\varepsilon_{\mu}^{(1)}=\begin{bmatrix}
0 \\
1 \\
0 \\
0
\end{bmatrix},\; \varepsilon^{(2)}_{\mu}=\begin{bmatrix}
0 \\
0 \\
1 \\
0
\end{bmatrix},\;\varepsilon_{\mu}^{(3)}=\begin{bmatrix}
0 \\
0 \\
0 \\
1
\end{bmatrix}.$$
We set $\vec{k}=k\vec{e}_{z}\implies k_{\mu}=k\begin{bmatrix}1 & 0 & 0 & 0\end{bmatrix}$. Check$$\tag{5.24} \varepsilon^{(\lambda)}(\vec{k})\cdot \varepsilon^{(\kappa)*}(\vec{k})=\varepsilon^{(\lambda)\mu}(\vec{k})\varepsilon_{\mu}^{(\kappa)*}(\vec{k})g_{\lambda \kappa}.$$
Finally check
$$\tag{5.25} [\hat{a}_{\lambda}(\vec{k}),\hat{a}^{\dagger}_{\kappa}(\vec{q})]=-(2\pi)^32k_{0}g_{\lambda\kappa}\delta^{(3)}(\vec{k}-\vec{q}).$$
This gives the [[Normal Ordering]] Hamiltonian
$$\tag{5.26} :\hat{H}:\;=\int \frac{d^3k}{(2\pi)^32k_{0}}k_{0}\left[ \sum_{\lambda=1}^3\left(\hat{a}^{\dagger}_{\lambda}(\vec{k})\hat{a}_{\lambda}(\vec{k})\right)-\hat{a}^{\dagger}_{0}(\vec{k})\hat{a}_{0}(\vec{k}) \right]$$where the sum is the space-like contribution to the energy and the last term is the time-like contribution, which reduces energy.

Since photons have 2 degrees of freedom, there is a dodgy space-like term, which perfectly cancels with the time-like term. Consider a single photon
$$\ket{1}_{s}=\int \frac{d^3k}{(2\pi)^32k_{0}}f(\vec{k})\hat{a}_{0}^{\dagger}(\vec{k})\ket{0},\;\; _{s}\braket{ 1 | 1 }_{s} = -_{s}\braket{ 0 | 0 }_{s} \int \frac{d^3k}{(2\pi)^32k_{0}}|f(\vec{k})|^2\leq 0.\tag{5.27} $$
The state has a negative norm which is pretty shit so it is non-physical. To find a physical state, consider $\partial_{\mu}\hat{A}^\mu_{+}\ket{\psi}=0$$$=-i\int \frac{d^3k}{(2\pi)^32}[k^\mu\varepsilon_{\mu}^{(0)}(\vec{k})\hat{a}_{0}(\vec{k})-k^\mu \varepsilon_{\mu}^{(3)}(\vec{k})\hat{a}_{3}(\vec{k})]e^{ -ik_{\mu}x^\mu }.\tag{5.28} $$Since $\vec{k}=k\vec{e}_{z}$, $\lambda=1,2$ terms vanish.

By definition, $k^\mu\varepsilon_{\mu}=0$
$$\therefore -i \int \frac{d^3k}{(2\pi)^3}[\hat{a}_{0}(\vec{k})-\hat{a}_{3}(\vec{k})]\ket{\psi}=0\tag{5.29}  $$for all physical states.
