In cosmology, fluid dynamics is used to simulate galaxy formation and evolution.

In a fluid, atoms/molecules are free to move past each other. Fluids can either be liquids or gases, depending on the size $r_{0}$ of the atoms/molecules compared to the mean separation $\lambda$ between them,
$$\lambda=\frac{1}{n^{1/3}}.\tag{5.1} $$
For a liquid, $\lambda\sim r_{0}$ so the molecules are touching but for a gas, $\lambda\gg r_{0}$ so there are empty space between them. For example, with water, $\frac{\lambda}{r_{0}}\sim 1$. Since $r_{0}^{H_{2}O}\sim 3\times 10^{-10}\text{ m}$, $\rho^{H_{2}O}\sim 10^{3}\text{ kg m}^{-3}\implies n^{H_{2}O}\sim 3\times 10^{28}\text{ m}^{-3}$ which gives $\lambda=(n^{H_{2}O})^{-1/3}\sim 3\times 10^{-10}\text{ m}$. For air $\frac{\lambda}{r_{0}}\approx 10$.

An atom/molecule has collision cross-section $\sigma=\pi r_{0}^2$. The mean free path $\ell$ is the distance an atom/molecule can travel in a straight line without colliding with another atom/molecule.
![[Pasted image 20251018102653.png]]
$$n\sigma \ell=1\implies \ell=\frac{1}{n\sigma}=\frac{1}{n\pi r_{0}^2}=\frac{1}{\pi}\left( \frac{\lambda}{r_{0}} \right)^3r_{0}.\tag{5.2} $$
Hence for liquids $\ell\sim r_{0}$ and for gases $\ell\gg r_{0}$. This is all for a microscopic description, which specifies motion of each particle individually.

A macroscopic description statistically obtains the motion of the system as a whole by averaging over volumes of spatial size $S$ and volume $S^3$. This requires $S\gg\lambda$ so the number of particles $N=nS^3=\left( \frac{S}{\lambda} \right)^{3}\gg 1$ as required for a statistical description to be valid.

Define the macroscopic mean mass density $\rho=\rho(\vec{r},t)$ and macroscopic mean velocity $\vec{u}=\vec{u}(\vec{r},t)$, which are both functions of space and time.

If macroscopic quantities vary on a spatial scale $L$, they require $S\ll L$ for a macroscopic description to be valid. The averaging scale $S$ must be in range
$$\lambda\ll S\ll L\tag{5.3} ,$$thus $L\gg\lambda$ for a macroscopic description to be valid.
![[Pasted image 20251018105109.png]]

The classification of fluids depends on $\ell$ compared to the length-scale $L$ on which macroscopic quantities vary.

Classification of fluids:
- Collisional if $\ell\ll L$
- Collisionless if $\ell\gtrsim L$

Liquids are always collisional since $\ell\sim\lambda\sim r_{0}$. Gases can be either collisional or collisionless.

Both types of gas can be described statistically by phase-space distribution function $f(\vec{r},\vec{v})$ defined s.t.
$$dN=f(\vec{r},\vec{v})d^3rd^3v\tag{5.4} $$is the number of molecules in spatial volume $d^3r$ and velocity range $d^3v$.

For collisional gas, collisions of atoms cause $v$ distribution to relax to a Maxwell distribution corresponding to thermal equilibrium at $T$,
$$f(\vec{r},\vec{v})=\frac{n(\vec{r})}{(2\pi)^{3/2}\sigma^2(\vec{r})}\exp\left[ -\frac{(\vec{v}-\vec{u}(\vec{r}))^2}{2\sigma^2(\vec{r})} \right].\tag{5.5} $$Collisional gases can be completely described by $\rho(\vec{r}),\vec{u}(\vec{r}),T(\vec{r})$. Collisional fluids can therefore be treated in a continuum approximation - ignoring atomic nature if the fluid.

In collisionless gases, the distribution function $f(\vec{r},\vec{v})$ is not locally relaxed as collisions are too infrequent so it needs to be defined in full.

In cosmology, baryons in the form of gas are always collisional, while dark matter is always collisionless.

Applying the basic physical laws of mass conservation, momentum balance, and gravity obtains a PDE to describe fluids that is obeyed by the relevant quantities.

- Assume Newtonian mechanics so ignore general relativity.
- Consider only ideal fluid (neglect viscosity and heat transport)

Consider the mass flow through the surface
![[Pasted image 20251018112633.png]]
Through the area $\Delta S$ in time $\Delta t$:
$$\Delta m=\rho\Delta Su_{n}\Delta t=\rho\Delta Su\cos \theta\Delta t=\rho \vec{u}\cdot\Delta \vec{S}\Delta t\tag{5.6} $$
where $\Delta \vec{S}=\hat{n}\Delta S$.
The rate of flow is then
$$\frac{\Delta m}{\Delta t}=\rho \vec{u}\cdot\Delta \vec{S}.\tag{5.7} $$
For a general surface, the mass flow through it is
$$\frac{dm}{dt}=\int \rho \vec{u}\cdot d\vec{s}\tag{5.8} .$$
For a closed surface $S$ enclosing a fixed volume $V$ and mass $m=\int \rho dV$,
$$\frac{dm}{dt}=\frac{d}{dt}\left( \int \rho dV \right)=\int \frac{{\partial \rho}}{\partial t}dV=-\oint \rho \vec{u}\cdot d\vec{s}.\tag{5.9} $$
The negative sign in front of the surface integral is due to the orientation of the surface.

Applying the divergence theorem gives
$$\oint \rho \vec{u}\cdot d\vec{S}=\int \vec{\nabla}\cdot(\rho \vec{u})dV\tag{5.10} $$which results in
$$\int \frac{{\partial \rho}}{\partial t}dV=-\int \vec{\nabla}\cdot(\rho \vec{u})dV\tag{5.11} $$which gives the continuity equation as the integrands must be equivalent
$$\frac{{\partial \rho}}{\partial t}+\vec{\nabla}\cdot(\rho \vec{u})=0\tag{5.12}. $$
For momentum balance, consider the acceleration of a fluid element moving with the fluid and the forces due to the gravity and pressure on it
![[Pasted image 20251018114113.png]]
$$\Delta \vec{u}=\vec{u}(\vec{r}+\Delta \vec{r},t+\Delta t)-\vec{u}(\vec{r},t)=\vec{u}(\vec{r}+\vec{u}\Delta t,t+\Delta t)-\vec{u}(\vec{r},t)\tag{5.13}. $$Taylor expand each component,
$$\Delta u_{x}=u_{x}(x+u_{x}\Delta t,y+u_{y}\Delta t,z+u_{z}\Delta t,t+\Delta t)-u_{x}(\vec{r},t)=u_{x}\Delta t \frac{{\partial u_{x}}}{\partial x}+u_{y}\Delta t \frac{{\partial u_{x}}}{\partial y}+u_{z}\Delta t \frac{{\partial u_{x}}}{\partial z}=\frac{\partial u_{x}}{\partial t}\Delta t+(u\cdot \vec{\nabla})u_{x}\Delta t.
\tag{5.14} $$
This gives the $x$ component of the acceleration, so overall the acceleration is
$$\vec{a}=\frac{\partial \vec{u}}{\partial t}+(\vec{u}\cdot \vec{\nabla})\vec{u}.\tag{5.15} $$
Note that fluid elements can be accelerated even in steady flow $\frac{\partial \vec{u}}{\partial t}=0$.

For gravity consider $\delta m=\rho\delta V$. As the fluid moves, $\rho,\delta V$ change but $\delta m$ is fixed. The gravitational force is
$$\delta \vec{f}_{g}=\delta m\vec{g}=(\rho\Delta V)\vec{g}.\tag{5.16} $$
Since gravity is a conservative force, it shall be written as
$$\vec{g}=-\vec{\nabla}\Phi \tag{5.17}. $$
![[Pasted image 20251018115239.png]]

To consider pressure, consider the difference of pressure forces acting on different sides of a fluid element.

Consider the $x$-component of pressure and Taylor expand it with respect to $\delta x$,
$$\delta f_{x}=p(x)\delta S-p(x+\delta x)\delta S=\left[ p(x)-p(x)-\delta x \frac{{\partial p}}{\partial x} \right]\delta S=-\frac{\partial p}{\partial x}\delta x\delta S\tag{5.18} $$and using $\delta S=\delta y\delta z$,
$$\delta \vec{f}_{p}=-(\vec{\nabla}p)\delta V\tag{5.19} .$$
Combining all results $(\delta m)\vec{a}=\delta \vec{f}_{g}+\delta \vec{f}_{p}$ and cancelling down gives the Euler equation,
$$\frac{\partial \vec{u}}{\partial t}+(\vec{u}\cdot \vec{\nabla})\vec{u}=-\vec{\nabla}\Phi-\frac{1}{\rho}\nabla p.\tag{5.20} $$
