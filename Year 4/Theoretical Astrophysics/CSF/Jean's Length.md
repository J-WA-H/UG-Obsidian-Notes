Consider the equation for the linear growth [(12.7)](Perturbations%20with%20Pressure.md),
$$\ddot{D}+2H(t)\dot{D}=\left( 4\pi G\rho-\frac{c_{s}^2k^2}{a^2} \right)D=0.\tag{12.7} $$
Consider the static medium $a=1,H=0, \bar{\rho}=\text{const}, c_{s}=\text{const}$. This simplifies the linear growth equation to
$$\ddot{D}=(4\pi G\bar{\rho}-c_{s}^2k^2)D\tag{13.1}. $$Since $k,\bar{\rho},c_{s}$ are all constant in this medium, define $\omega=4\pi G\bar{\rho}-c_{s}^2k^2$ which gives the solution
$$D(t)\propto e^{ i\omega t }.\tag{13.2} $$
The nature of this solution depends on whether $\omega^2>0$ or $\omega^2<0$. This is equivalent to whether $k>k_{J}$ or $k<k_{J}$ where
$$k_{J}\equiv \frac{(4\pi G\bar{\rho})^{1/2}}{c_{s}}\tag{13.3} $$
is the Jeans wavenumber in a static medium, defined where $\omega=0$.

$\lambda_{J}$ is the Jeans length defined by
$$\lambda_{J}=\frac{2\pi}{k_{J}}=c_{s}\left( \frac{\pi}{G\bar{\rho}} \right)^{1/2}.\tag{13.4} $$
![[Pasted image 20251101114851.png]]
There are two distinct cases: 
- $k>k_{J}\to$ $\delta$ oscillates
- $k<k_{J}\to$ $\delta$ grows/decays exponentially.

For $k>k_{J}$, $\omega^2>0\implies \omega \in \mathbb{R}$ so $\delta$ oscillates in time due to pressure so
$$\delta(\vec{x},t)\propto e^{ i(\omega t+\vec{k}\cdot \vec{x}) }\tag{13.5}. $$
This is a sound wave moving at speed $v=\frac{\omega}{k}$. For $k\gg k_{J}$, $\omega \approx\pm c_{s}k\implies v\approx c_{s}$ like normal sound waves.

For $k<k_{J}$, $\omega^2<0$, so $\omega\in \mathbb{C}$ which gives $\omega=\pm i\gamma$, where $\gamma=(4\pi G\bar{\rho}-c_{s}^2k^2)^{1/2}\in \mathbb{R}$. This yields two solutions
$$D_{+}\propto e^{ \gamma t },\;D_{-}\propto e^{ -\gamma t }\tag{13.6} .$$
This shows that $\delta$ either grows or decays exponentially due to self gravity. The full solution is then
$$\delta(\vec{x},t)\propto e^{ \pm i\gamma }e^{ i\vec{k}\cdot \vec{x} }.\tag{13.7} $$
The timescale $\delta$ grows or decays on timescale $\frac{1}{\gamma}$. For $k\ll k_{J}$, $\gamma \approx \sqrt{ 4\pi G\bar{\rho} }=\frac{1}{\tau_{grav}}$ so this is the same exponential solution for [[Density Perturbations Without Pressure]] in a static universe.

Jean's length $\lambda_{J}$ separates perturbations,
- $\lambda<\lambda_{J}$ which oscillates due to pressure
- $\lambda>\lambda_{J}$ which grows or decays due to self-gravity.

Consider a spherical region of radius $R$ with overdensity $\delta \rho>0$ in a static background medium with a uniform density $\bar{\rho}$ and a uniform pressure $\bar{p}$.
$$\begin{matrix}
\rho=\bar{\rho}+\delta \rho, & p=\bar{p}+\delta p
\end{matrix}\tag{13.8}. $$
![[Pasted image 20251101125935.png]]

Pressure per unit mass at the edge of the sphere to first order is
$$-\frac{\vec{\nabla}p}{\rho}=-\frac{\vec{\nabla}(\bar{p}+\delta p)}{(\bar{\rho}+\delta \rho)}\approx-\frac{\frac{d(\delta p)}{dR}}{\bar{\rho}}\sim \frac{\delta p}{R\bar{\rho}}=\frac{c_{s}^2\delta \rho}{R\bar{\rho}}\tag{13.9}$$using $\delta p=c_{s}^2\delta \rho$.

The perturbation in gravitational acceleration at the edge of the sphere to first order is
$$\delta g=-\frac{G\delta M}{R^2}\sim GR\delta \rho \tag{13.10} $$where the excess mass is
$$\delta M=\frac{4\pi}{3}R^3\delta \rho.\tag{13.11} $$
The sphere will collapse if the gravity dominates over pressure,
$$GR\delta \rho\gtrsim \frac{c_{s}^2\delta \rho}{R\bar{\rho}}\implies R\gtrsim \frac{c_{s}}{(G\bar{\rho})^{1/2}}\sim\lambda_{J}.\tag{13.12} $$
This shows the Jean's length is the scale where pressure and gravity balance.

The equation for linear growth rate $D(t)$ becomes
$$\ddot{D}(t)+2H(t)\dot{D}(t)=\omega^2(t)D(t)\tag{13.13} $$
where 
$$\omega^2(t)=\frac{c_{s}^2(t)k^2}{a^2(t)}-4\pi G\bar{\rho}(t).\tag{13.14} $$
The differences compared to the static case are:
- $\omega$ depends on time
- Hubble drag term $2H \frac{\partial\delta}{\partial t}$ damps any growing or oscillatory solutions.

Solutions for $D(t)$ in an expanding universe is analogous to those for a damped harmonic oscillator except
- $\omega^2$ can be negative
- Both coefficients for $D,\dot{D}$ depend on time.

The Jean's length defined by $\omega=0$ still effectively separates oscillatory and growing/decaying solutions.

The comoving Jeans wavelength is 
$$k_{J}\equiv \frac{(4\pi G\bar{\rho})^{1/2}a}{c_{s}}\tag{13.15} $$and the proper Jeans length is
$$\lambda_{J}=\frac{2\pi}{k_{J}}a=c_{s}\left( \frac{\pi}{G\bar{\rho}} \right)^{1/2}.\tag{13.16} $$
In general, $k_{J},\lambda_{J}$ depends on time.
![[Pasted image 20251101131640.png]]

Plane wave perturbations with $\lambda_{J}$, overdense regions have a size $\frac{\lambda_{J}}{2}$. Gravitational collapse happens on sizes $\sim\lambda_{J}$.

The Jeans mass is the mass inside the sphere of the radius $\frac{\lambda_{J}}{2}$,
$$M_{J}\equiv \frac{4\pi}{3}\left( \frac{\lambda_{J}}{2} \right)^{3}\bar{\rho}\tag{13.17} .$$ With $\lambda_{J}$ defined in $(13.16)$, this gives
$$M_{J}= \frac{\pi^{5/2}}{6} \frac{c_{s}^{3}}{G^{3/2}\bar{\rho}^{1/2}}.\tag{13.18} $$
Density perturbations with $M<M_{J}$ oscillate and $M>M_{J}$ grows/decays.

Define the mass in matter (baryonic + dark) associated with perturbations of proper wavelength $\lambda$ as
$$M_{m}=\frac{4\pi}{3}\left( \frac{\lambda}{2} \right)^{3}\bar{\rho}_{m}\tag{13.19}. $$
Recall $\lambda \propto a$ and $\bar{\rho}_{m}\propto a^{-3}$ shows $M_{m}$ remains constant as the perturbation evolves so we can use this to relate the sane density perturbations at different times.

The comoving wavelength is given by
$$\lambda_{com}=\left( \frac{6M_{m}}{\pi \bar{\rho}_{m_{0}}} \right)=3.6\text{ Mpc}\left( \frac{\Omega_{m_{0}}}{0.3} \right)^{-1/3}\left( \frac{M_{m}}{10^{12}M_{\odot}} \right)^{1/3}.\tag{13.20} $$For the milky way, $M\sim 10^{12}M_{\odot}\implies\lambda_{com}\sim 4\text{ Mpc}$. For massive galaxy clusters, $M\sim 10^{15}M_{\odot}\implies\lambda_{com}\sim 40\text{ Mpc}$.

