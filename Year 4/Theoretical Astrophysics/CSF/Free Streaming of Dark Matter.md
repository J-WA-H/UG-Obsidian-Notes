Fluids are characterised into [collisional and collisionless](Fluid%20Equations.md),
![[Pasted image 20251108160513.png]]
Collisional fluids have a short mean free path. The frequent collisions maintain local thermal equilibrium. Properties are completely specified by a few macroscopic variables: density, pressure (or temperature), and velocity. The evolution of these variables is described by the standard fluid equations. Examples are a baryonic gas after recombination and a [[Baryon-Photon Fluid]].

Collisionless fluids have a long mean free path. It is not in thermal equilibrium. Collisionless fluids are described by $f(\vec{r},\vec{v},t)$, the phase-space distribution function defined such that $f(\vec{r},\vec{v},t)d^3rd^3v$ gives the number of particles in the phase-space volume $d^3r d^3v$. The evolution of $f(\vec{r},\vec{v},t)$ is given by the collisionless Boltzmann equation. An example is dark matter that is thought to be an extremely weakly interacting elementary particle. Dark matter is effectively collisionless over most of the history of the universe (though probably in thermal equilibrium at very early times).
![[Pasted image 20251108164143.png]]
Random motions of particles unimpeded by any collisions transport particles from overdense regions to underdense regions. In the absence of gravity, free streaming erase density fluctuations of proper size $\lambda$ over timescale 
$$\tau_{FS}\sim \frac{\lambda}{v_{*}}\tag{17.1} $$
where $v_{*}$ is the random thermal speed.
![[Pasted image 20251108164959.png]]

Consider a static medium. Compare $\tau_{FS}$ with the gravitational growth time $\tau_{grav}$. Gravity wins over free streaming if
$$\tau_{grav}\lesssim\tau_{FS}\implies\lambda_{J}\lesssim \lambda\tag{17.2} $$with [[Jean's Length]] defined as
$$\lambda_{J}=v_{*}\left( \frac{\pi}{G\bar{\rho}} \right)^{1/2\tag{17.3} }$$i.e. the Jeans length in a collisionless fluid is the scale where free streaming balances self-gravity.

For $\lambda>\lambda_{J}$, self-gravity makes $\delta$ grow faster than free streaming can smooth it. 
For $\lambda<\lambda_{J}$, there is damping in a collisionless fluid as opposed to oscillations as in the collisional case.

Compare $\tau_{FS}$ with the age of the universe at time $t$. $\tau_{FS}=t$ gives the scale $\lambda_{FS}$, the free streaming length, up to which free streaming could erase density perturbations,
$$\lambda_{FS}\sim v_{*}t.\tag{17.4} $$
For $\lambda<\lambda_{J}$ (static case) or $\lambda<\lambda_{FS}$ (expanding case),
- $\delta$ is damped due to the free streaming of collisionless particles, which is completely different to a collisional fluid, where $\delta$ oscillates as a sound wave.

For $\lambda>\lambda_{J}$ or $\lambda>\lambda_{FS}$,
- Density perturbations grow due to self-gravity. $\delta$ grows like a collisional fluid with zero pressure.

For collisionless fluids in an expanding universe, the free streaming length is more useful than the Jeans length:
- $\lambda_{J}$ depends on $t$ and can increase/decrease with time
- Density perturbations on the comoving wavelength erased by free streaming are not recreated even if $\lambda_{J}$ falls.

The total comoving distance a collisionless particle moving at a typical thermal speed $v_{*}(t)$ can travel from the big bang, $t=0$, to time $t$.
Since $dx=\frac{dr}{a}=\frac{v_{*}dt}{a}$, we get
$$\ell_{FS}(t)=\int_{0}^{t} \frac{v_{*}(t')}{a(t')}dt'.\tag{17.5} $$
The proper free streaming length is given by
$$\lambda_{FS}(t)=\ell_{FS}(t)a(t).\tag{17.6} $$
The general picture for how $\delta$ in a collisionless dark matter evolves in an expanding universe is:
- $\delta$ with $\lambda\lesssim\lambda_{FS}$ gets erased by free-streaming by time $t$
- $\delta$ with $\lambda\gtrsim \lambda_{FS}$ grows by self-gravity in the same way up to $t$ as a collisional fluid with zero pressure.

If $v_{*}(t)=0\;\forall\;t$ then $\lambda_{FS}=0$ since $\ell_{FS}=0$.

The schematic picture is confirmed by full numerical calculations using the collisionless Boltzmann equation.

Analogous to the Jeans mass $M_{J}$, we define the free streaming mass $M_{FS}$,
$$M_{FS}=\frac{4\pi}{3}\left( \frac{\lambda_{FS}}{2} \right)^{3}\bar{\rho}_{m}.\tag{17.7} $$
Consider dark matter particles interactions are in thermal equilibrium at early times.

Dark matter particles decouple (i.e. interactions stop at $a=a_{dec}$), $\rho$ falls due to the expansion of the universe which reduces interactions. Dark matter is effectively collisionless for $a>a_{{dec}}$.

Assume dark matter particles are still relativistic at $a_{rec}$ so
$$T_{X}(t)\propto \frac{1}{a(t)}\tag{17.8} $$like photons.

Dark matter particles become non-relativistic at $a=a_{nr}\gg a_{dec}$ when the mean thermal energy equals the rest mass energy,
$$3k_{B}T_{X}(t_{nr})\approx m_{X}c^2\implies a_{nr}\propto \frac{1}{m_{*}}.\tag{17.9} $$
This shows more massive particles become more non-relativistic at earlier times.

The momentum for non-relativistic collisionless particles scale as $p\propto \frac{1}{a}$. This gives $v_{*}\propto \frac{1}{a}$ for $a>a_{nr}$ so
$$v_{*}(t)\approx \begin{cases}
c & a<a_{nr} \\
c\left( \frac{a_{nr}}{a} \right) & a>a_{nr}
\end{cases}.\tag{17.10} $$
The evolution of $a(t)$ in terms of $a_{eq},t_{eq}$ gives$$a(t)\approx \begin{cases}
a_{eq}\left( \frac{t}{t_{eq}} \right)^{1/2} & t<t_{eq} & \text{radiation domination} \\
a_{eq}\left( \frac{t}{t_{eq}} \right)^{2/3} & t>t_{eq} & \text{matter domination}
\end{cases}.\tag{17.11} $$
Assuming $a_{nr}<a_{eq}$, $\ell_{FS}$ for $t>t_{eq}$ is given by
$$\ell_{FS}(t)=\int_{0}^{t} \frac{v_{*}(t')}{a(t')}dt'=\int_{0}^{t_{nr}} \frac{cdt'}{a}+\int_{t_{nr}}^{t} c\left( \frac{a_{nr}}{a} \right) \frac{dt'}a =\int_{0}^{t_{nr}} \frac{cdt'}{a_{eq}\left( \frac{t'}{t_{eq}} \right)^{1/2}}+\int_{t_{nr}}^{t_{eq}} \frac{ca_{nr}}{a^2_{eq}\left( \frac{t'}{t_{eq}} \right)}dt'+\int_{t_{eq}}^{t} \frac{ca_{nr}}{a^2_{eq}\left( \frac{t'}{t_{eq}} \right)^{4/3}}\tag{17.12}. $$
Evaluating this gives the comoving free streaming length for dark matter,
$$\ell_{FS}(t)=\frac{2ct_{nr}}{a_{nr}}\left[ \frac{5}{2}+\ln\left( \frac{a_{eq}}{a_{nr}} \right)-\frac{3}{2}\left( \frac{a(t)}{a_{eq}} \right)^{-1/2} \right].\tag{17.13} $$For $a\gg a_{eq}$, the comoving free streaming length converges to
$$\ell_{FS}^{final}=\frac{2ct_{nr}}{a_{rn}}\left[ \frac{5}{2}+\ln\left( \frac{a_{eq}}{a_{nr}} \right) \right]\tag{17.14} $$
which depends mainly on the epoch $a_{nr}$.

Up to some logarithmic factor,
$$\ell_{FS}\propto a_{nr}\propto \frac{1}{m_{X}}.\tag{17.15} $$This implies lighter dark matter particles have larger free streaming lengths.

For very light dark matter particles with $a_{nr}=a_{eq}$, $\ell_{FS}^{final}=\frac{5ct_{eq}}{a_{eq}}\sim 300\text{ Mpc}$.

Free streaming potentially has a very large effect on structure formation.

For heavy dark matter particles, $a_{nr}\ll a_{eq}$ gives $\ell_{FS}^{final}\approx 0$.

We classify dark matter particles based on the particle mass and free streaming length:
- Hot dark matter (HDM), $a_{nr}\sim a_{eq}$. These are light dark matter particles with $m_{*}\sim \text{eV/c}^2$,
$$\ell_{FS}\sim \frac{ct_{eq}}{a_{eq}}.\tag{17.16} $$
	Free streaming is very important for HDM.
- Cold dark matter (CDM), $a_{nr}\lll a_{eq}$. These are heavy particles with $m_{X}\sim\text{GeV/c}^2$,
$$\ell_{FS}\lll \frac{ct_{eq}}{a_{eq}}\tag{17.17}  $$
	so free streaming is negligible on the scale of structures in the present day universe.
- Warm dark matter (WDM), the intermediate case with $m_{X}\sim\text{keV/c}^2$.
	Free streaming is not important for large-scale clustering, but could have effects on the scale of individual galaxies.

Free streaming suppresses density fluctuations on small scales for HDM but not CDM.

Observed galaxy clustering is on scale $1-100\text{ Mpc}$ which is much more than predicted by HDM so HDM has been ruled out.