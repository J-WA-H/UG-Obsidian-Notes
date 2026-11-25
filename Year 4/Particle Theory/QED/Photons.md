From Maxwell's equations, we have a vector $\vec{E}$ and an axial vector $\vec{B}$.

| Equation                                         | type          | $J^{P}$ | Constant                    |
| ------------------------------------------------ | ------------- | ------- | --------------------------- |
| $\vec{\nabla}\cdot \vec{E}$                      | Scalar        | $0^{+}$ | $\rho$                      |
| $\vec{\nabla}\cdot \vec{B}$                      | Pseudo-Scalar | $0^{-}$ | $\cancelto{0}{\rho_{M}}$    |
| $\partial_{t}\vec{E},\vec{\nabla}\times \vec{B}$ | Vector        | $1^{-}$ | $\vec{j}$                   |
| $\partial_{t}\vec{B},\vec{\nabla}\times \vec{E}$ | Axial-vector  | $1^{+}$ | $\cancelto{0}{\vec{j}_{M}}$ |
$\rho_{M}, \vec{j}_{M}$ go to zero as magnetic monopoles have not been detected.

These fields can be expressed in terms of potentials,
$$\vec{E}=-\vec{\nabla}A^{0}-\partial_{t}\vec{A},\;\vec{B}=\vec{\nabla}\times \vec{A}.\tag{4.1} $$
This gives the gauge field $A^{\mu}=(A^{0},\vec{A})$.

The physical fields are gauge invariant.
$$A^{\mu}\to A'^{\mu}=A^{\mu}-\partial_{\mu}\Lambda(x).\tag{4.2} $$
From this we can always find a gauge $\Lambda$ such that $A^{0}=0$. I can always gauge away one degree of freedom.

The field strength tensor is defined by
$$F^{\mu \nu}=\partial^{\mu}A^{\nu}-\partial^{\nu}A^{\mu}=F'^{\mu \nu}\tag{4.3} $$
Modifying the Lagrangian with this photon field gives
$$\mathcal{L}=-\frac{1}{4}F^{\mu \nu}F_{\mu \nu}+\lambda j^{\mu}A_{\mu}\tag{4.4} $$
where $\lambda$ is some proportionality constant.
We can also define
$$\tilde{F}^{\mu \nu}=\epsilon^{\mu \nu \rho \sigma}F_{\rho\sigma}\tag{4.5} .$$Using these the equations of motion are
$$\partial_{\mu}F^{\mu \nu}=j^{\nu},\;\partial_{\mu}\tilde{F}^{\mu \nu}=0\tag{4.6} .$$
It is also worth noting that $F^{\mu \nu}F_{\mu \nu}=\frac{1}{2}(E^2-B^2)$.

Looking at the zero component, $$F^{00}=\partial^{0}A^{0}-\partial^{0}A^{0}\tag{4.7}=0 ,$$this implies the conjugate momentum for the zeroth component vanishes
$$\pi^{0}=\frac{\partial \mathcal{L}}{\partial (\partial_{t}A^{0})}=0\tag{4.8} $$as there is no time derivative for $A^{0}$. $\pi^{i}$ for all other components exists. From this, we cannot quantise $A^{0}$ as all commutator relations vanish.

We can also gauge out one $A^{i}$ component which decreases the field from four degrees of freedom to two - the polarisation.

The Coulomb gauge is not Lorentz invariant as $A^{0}=0$ so there is no temporal component. The Lorenz gauge adds a term to the Lagrangian that keeps $A^{0}$ then kills it at the end.

Consider the wavevector $\vec{k}=k\vec{e}_{z}$. The polarisation vectors are$$\vec{\varepsilon}_{1,2}=\vec{e}_{x}, \vec{e}_{y}\tag{4.9} .$$In column vector form, these are
$$\vec{\varepsilon}_{x}=\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix},\;\vec{\varepsilon}_{y}=\begin{bmatrix}
0 \\
1 \\
0
\end{bmatrix} \tag{4.10} .$$
Light is normally circular polarised so
$$\vec{\varepsilon}_{1,2}=\frac{{\vec{e}_{x}\pm \vec{e}_{y}}}{\sqrt{ 2 }}\tag{4.11} $$We normally have the conditions
$$\vec{k}\cdot\vec{\varepsilon}=0,\;k_{\mu}\varepsilon^{\mu}=0\tag{4.12} $$
which gives
$$k_{\mu}=k\begin{bmatrix}
1 \\
0 \\
0 \\
1
\end{bmatrix},\;\varepsilon^{\mu}=\frac{1}{\sqrt{ 2 }}\begin{bmatrix}
0 \\
1 \\
\pm i \\
0
\end{bmatrix}.\tag{4.13} $$
This is the orthogonality condition, and the two polarisation vectors are also orthonormal, $\vec{\varepsilon}_{i}\cdot\vec{\varepsilon}_{j}=\delta_{ij}$.




