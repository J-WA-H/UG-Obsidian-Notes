An equation of state is the relation between pressure, density, and temperature, $p=p(\rho,T)$.

In general we need an equation for the energy balance of a fluid element to find how $T$ evolves. In cosmology, we usually consider adiabatic fluids - no heat flow in or out of the fluid element, so the entropy per unit mass $S(\rho,T)$ is constant with time.

Assume $S$ is uniform, in cosmology, $S$ is the same for all fluid elements for all $t$.

Since, $p=p(\rho,T)$, it can be written as $p=p(\rho,S)$. Since $S$ is constant, the pressure can be calculated if we know the density. e.g. for a monatomic ideal gas, $p=K(S)\rho^{5/3}\propto \rho^{5/3}$ if $S$ is constant.

Newton's laws of gravity can be used to yield Poisson equations. The gravitational acceleration for a point mass $M$ is
$$\vec{g}=-\frac{GM}{r^2}\hat{r}\tag{6.1} .$$Integrating over a closed surface gives Gauss' law,
$$\oint \vec{g}\cdot d\vec{s}=-4\pi G\sum m_{i}=-4\pi G\int \rho dV\tag{6.2} .$$From divergence theorem $\vec{\nabla}\cdot \vec{g}=-4\pi G\rho$ and using $\vec{g}=-\vec{\nabla}\Phi$, this yields Poisson's equations
$$\nabla^2\Phi=4\pi G\rho \tag{6.4} $$
Using the other [[Fluid Equations]] we get three coupled PDEs, the continuity equation, the Euler equation, and the Poisson equation,
$$\frac{\partial \rho}{\partial t}+\vec{\nabla}\cdot(\rho \vec{u})=0\tag{5.12} $$
$$\frac{\partial \vec{u}}{\partial t}+(\vec{u}\cdot \vec{\nabla})\vec{u}=-\frac{1}{\rho}\vec{\nabla}p-\vec{\nabla}\Phi \tag{5.20} $$
$$\nabla^2\Phi=4\pi G\rho.\tag{6.4} $$
