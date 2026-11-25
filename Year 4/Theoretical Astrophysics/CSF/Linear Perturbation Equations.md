The [[Exact Perturbation Equations]] are non-linear and can hold for large perturbations but in general, $\delta\ll 1$ for early times up to $z\sim 10$. Hence we can approximate the exact equations for perturbations by equations which are linear - first order in perturbed quantities, e.g. terms like $\delta,\vec{v}$ etc. are kept in but terms like $\delta^2,\vec{v}\delta$ are discarded.

Higher order terms should be much smaller than the first order times if the perturbations are sufficiently small.

Continuity equation:
$$\frac{\partial\delta}{\partial t}|_{\vec{x}} + \frac{1}{a}\vec{\nabla}_{\vec{x}}\cdot[(1+\cancelto{0}{\delta})\vec{v}]=0\tag{10.1} $$
$$\implies \frac{\partial\delta}{\partial t}|_{\vec{x}}+\frac{1}{a}\vec{\nabla}_{\vec{x}}\cdot \vec{v}=0.\tag{10.2} $$
Euler equation:
$$\frac{\partial \vec{v}}{\partial t}|_{\vec{x}}+\frac{\dot{a}}{a}\vec{v}+\frac{1}{a}\cancelto{0}{(\vec{v}\cdot \vec{\nabla}_{\vec{x}})\vec{v}}=-\frac{\vec{\nabla}_{\vec{x}}\delta p}{a\bar{\rho}(1+\delta)}-\frac{\vec{\nabla}_{\vec{x}}\phi}{a}\tag{10.3} .$$Expanding the first term in the RHS in terms of $\delta$ and discarding higher order terms gives
$$\frac{\partial \vec{v}}{\partial t}|_{\vec{x}}+\frac{\dot{a}}{a}\vec{v}=-\frac{\vec{\nabla}_{\vec{x}}\delta p}{a\bar{\rho}}-\frac{\vec{\nabla}_{\vec{x}}\phi}{a}.\tag{10.4} $$
There is no change for the Poisson equation,
$$\nabla^2_{\vec{x}}\phi=4\pi Ga^2\bar{\rho}a^2.\tag{10.5} $$
If interest is only with density perturbations, all three equations can be combined to give a master equation.
$$\frac{\partial^2\delta}{\partial t^2}|_{\vec{x}}+2 \frac{\dot{a}}{a} \frac{\partial\delta}{\partial t}|_{\vec{x}}=\frac{\nabla^2_{\vec{x}}\delta p}{a^2\bar{\rho}}+4\pi G\bar{\rho}\delta.\tag{10.6}$$
The $2 \frac{\dot{a}}{a} \frac{\partial\delta}{\partial t}|_{\vec{x}}$ term represents Hubble drag caused by the expansion of the universe. The $\frac{\nabla^2_{\vec{x}}\delta p}{a^2\bar{\rho}}$ term represents the effect of pressure forces on $\delta$, and the $4\pi G\bar{\rho}\delta$ represents the effect of self-gravity.

From gravity, $|\delta|$ typically grows in amplitude as the universe evolves. Linear perturbation theory is a very good approximation provided $|\delta|\ll {1}$, and roughly valid until $|\delta|\simeq 1$. Density perturbations with $|\delta|\gtrsim 1$ are non-linear.

For overdense regions ($\delta>0$), $\delta$ stops expanding with Hubble flow when $\delta \approx 1$. Then they undergo gravitational collapse to form gravitationally bound structures in dynamical equilibrium with $\delta\gg 1$, dark matter halos containing galaxies, groups, and clusters.

![[Pasted image 20251026114939.png]]

In underdense regions, $\delta<0$, $\delta$ evolves into cosmic voids with $\delta \approx -1$, essentially empty regions which expand with the universe.

![[Pasted image 20251026115051.png]]
