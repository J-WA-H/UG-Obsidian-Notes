The universe contains different fluids which only interact via gravity, e.g. dark matter, [[Baryon-Photon Fluid]]. 

$\delta$ can be different in different components but all feel the same gravitational field.

After recombination, CDM behaves as a fluid with zero pressure,
$$\delta_{DM}=\frac{\delta \rho_{DM}}{\bar{\rho}_{DM}}\tag{16.1} .$$
Baryons are a non-relativistic fluid with pressure,
$$\delta_{b}=\frac{\delta \rho_{b}}{\bar{\rho}_{b}}.\tag{16.2} $$
This gives the master equations
$$\frac{\partial^2\delta_{DM}}{\partial t^2}+2H \frac{\partial\delta_{DM}}{\partial t}=\frac{1}{a^2}\nabla^2\phi \tag{16.3} $$$$\frac{\partial^2\delta_{b}}{\partial t^2}+2H \frac{\partial\delta_{b}}{\partial t}=\frac{c_{s}^2}{a^2} \nabla^2\delta_{b}+\frac{1}{a^2}\nabla^2\phi.\tag{16.4} $$This gives a pair of coupled equations as $\phi$ depends on both $\delta_{DM}$ and $\delta_{b}$.
The perturbation $\phi$ is related to the [[Poisson's Equations]],
$$\nabla^2\phi=4\pi Ga^2\delta \rho_{tot};\;\delta \rho_{tot}=\delta \rho_{DM}+\delta \rho_{b}=\bar{\rho}_{DM}\delta_{DM}+\bar{\rho}_{b}\delta_{b}.\tag{16.5} $$
Suppose the perturbation in both baryons and dark matter are plane waves with the same wavenumber,
$$\delta_{DM}\propto e^{ i\vec{k}\cdot \vec{x} },\;\delta_{b}\propto e^{ i\vec{k}\cdot \vec{x} }.\tag{16.6} $$
This gives
$$\frac{d^2\delta_{b}}{dt^2}+2H \frac{d\delta_{b}}{dt}=-\frac{c_{s}^2k^2}{a^2}\delta_{b}+4\pi G[\bar{\rho}_{DM}\delta_{DM}+\bar{\rho}_{b}\delta_{b}].\tag{16.7} $$
Consider the special case $\delta_{DM}=\delta_{b}$. Define $k=k_{J_{b}}$ so the RHS=0,
$$k_{J_{b}}=[4\pi G(\bar{\rho}_{DM}+\bar{\rho}_{b})]^{1/2} \frac{a}{c_{s}}.\tag{16.8} $$
The pressure of baryons exactly balance the combined gravity of baryons and dark matter.
$$\lambda_{J_{b}}=c_{s}\left( \frac{\pi}{G\bar{\rho}_{tot}} \right)^{1/2}.\tag{16.9} $$
Although derived for a special case, $\lambda_{J_{b}}$ remains useful more generally.

In general, $k_{J_{b}}$ depend on the ratio of perturbations.

Assume collisionless cold dark matter component together with radiation ($b\gamma$ fluid),
$$\Omega=\Omega_{DM}+\Omega_{r}=1,\;\rho_{b}\ll \rho_{\gamma}\text{ s.t. } \rho_{b\gamma}\equiv \rho_{r}.\tag{16.10} $$
Dark matter and radiation only interact via gravity.

Consider density perturbations with $\lambda\ll\lambda_{J_{b\gamma}}$. The Meszaros approximation - assume there are density perturbations in dark matter, but that radiation density remains perfectly uniform. This is a good approximation for evolution of density perturbations in CDM for wavelengths $\lambda_{J_{b\gamma}}$.

For $\lambda<\lambda_{J_{b\gamma}}$ when $a<a_{rec}$,
- Pressure of coupled photon-baryon fluid causes $\delta_{r}$ to oscillate
- Dark matter component feels no pressure (thus no oscillations) but tend to grow due to self gravity
The time-average gravitational effect of the oscillating radiation part on dark matter is almost zero.

![[Pasted image 20251107134110.png]]

Evolution of the DM perturbation is almost the same as within a uniform radiation background.

Hence assume $\bar{\rho}=\bar{\rho}_{DM}+\bar{\rho}_{b}$ but $\nabla^2\phi-4\pi Ga^2\delta \rho_{DM}$ for dark matter as the time-average for $\delta_{r}$ is almost zero for $\lambda\ll\lambda_{J_{b\gamma}}$. The master equation becomes
$$\frac{\partial^2\delta_{DM}}{\partial t^2}+2H \frac{\partial\delta_{DM}}{\partial t}-4\pi G\bar{\rho}_{DM}=0.\tag{16.11} $$
This looks identical to the single fluid master equation except that $\rho_{r}$ effects $H(t)$ are $\bar{\rho}_{DM}(t)$/

We need to solve this growing from radiation domination to matter domination.
Since $\rho_{m}=\rho_{DM}$ and $\rho_{m}=\rho_{r}$ at time $a=a_{eq}$, we can write,
$$\bar{\rho}=\bar{\rho}_{m}+\bar{\rho}_{r},\;\bar{\rho}_{m}=\bar{\rho}_{m,eq}\left( \frac{a_{eq}}{a} \right)^3,\;\bar{\rho}_{r}=\bar{\rho}_{m,eq}\left( \frac{a_{eq}}{a} \right)^{4}.\tag{16.12} $$
It is convenient to define a new time variable,
$$y\equiv \frac{a}{a_{eq}}\tag{16.13}. $$
This gives the Meszaros equation for dark matter,
$$\frac{\partial^2\delta_{DM}}{\partial y^2}+\frac{2+3y}{2y(1+y)} \frac{\partial\delta_{DM}}{\partial y}-\frac{2}{2y(1+y)}\delta_{DM}=0.\tag{16.14} $$
The growing mode solution is
$$D_{+}=1+\frac{3}{2}y=1+\frac{3}{2} \left( \frac{a}{a_{eq}} \right).\tag{16.15} $$
$D_{+}\to 1$ for early times and $D_{+}\propto a$ for late times.

$\delta_{DM}$ does not grow as long as the mean density of the universe is dominated by radiation.

The Meszaros effect is the suppression of growth of $\delta \rho$ in a collisionless cold dark matter component when $\rho_{tot}$ is dominated by a uniform radiation background. This applies to $\delta_{DM}$ with $\lambda<\lambda_{J_{b\gamma}}$ during the radiation-dominated era. The physical reason for suppression of perturbation growth is that radiation density dominates the expansion of the universe, so the growth time for dark matter perturbations due to self gravity is
$$\tau_{grav}=\frac{1}{\sqrt{ 4\pi G\bar{\rho}_{DM} }}=\left( \frac{\bar{\rho}_{r}}{\bar{\rho}_{DM}} \right)^{1/2} \frac{1}{\sqrt{ 4\pi G\bar{\rho}_{r} }}\sim \left( \frac{\bar{\rho}_{r}}{\bar{\rho}_{DM}} \right)^{1/2}\tag{16.16} $$so $\tau_{grav}\gg t$ as $\bar{\rho}_{r}\gg \bar{\rho}_{DM}$. The growth of $\delta_{DM}$ due to self gravity is effectively overwhelmed by the expansion of the universe.

