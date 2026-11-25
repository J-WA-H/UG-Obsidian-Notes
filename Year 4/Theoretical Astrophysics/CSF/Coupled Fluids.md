The main component of the universe are dark matter - collisionless, baryons - collisional, and photons - collisional before recombination, collisionless after.

Perturbations in collisional and cold collisionless fluids can be treated using the normal [[Fluid Equations]]. Other collisionless fluids like hot, warm dark matter can [free stream](Free%20Streaming%20of%20Dark%20Matter.md). Collisionless fluids only interact via gravity.

In inflation models, we assume:
- fluctuations/perturbations in a scalar field driving inflation are separated during inflation
- At the end of inflation, they are converted into adiabatic density fluctuations in the different components.
This gives, for a [[Baryon-Photon Fluid]],
$$\frac{\delta \rho_{b}}{\bar{\rho}_{b}}=-\frac{3}{4} \frac{\delta \rho_{\gamma}}{\bar{\rho}_{\gamma}}\iff\delta_{b}=\frac{3}{4}\delta_{\gamma}\tag{19.1} $$More generally, adiabatic means
$$\frac{\delta \rho_{m}}{\bar{\rho}_{m}}=\frac{3}{4} \frac{\delta \rho_{r}}{\bar{\rho}_{r}} \iff \delta_{m}=\frac{3}{4}\delta_{r}\tag{19.2} $$where $\rho_{m}$ is any non-relativistic component, and $\rho_{r}$ is any relativistic component.

The density fluctuations of different components are related to each other as
$$\delta_{b}=\delta_{DM}=\frac{3}{4}\delta_{\gamma}=\frac{3}{4}\delta_{\nu}\tag{19.3} .$$
Assume that all perturbations initially all have this form. Subsequent evolution can cause deviations from these adiabatic ratios.

Outside the [horizon](Perturbations%20Outside%20Horizon.md) $\lambda>R_{H}$ evolution of $\delta$ for dark matter, baryons, and photons is characterised by,
- Only gravity is important for perturbation growth, all components evolve in the same way, $\delta_{\gamma}\propto\delta_{b}\propto\delta_{DM}$, maintaining the adiabatic ratios.
$$\delta_{b}=\delta_{DM}=\frac{3}{4}\delta_{\gamma} \tag{19.6}.$$
- The growing mode evolves as
$$\delta \propto \begin{cases}
a^2 & a_{inf}<a<a_{eq} & \text{radiation} \\
a & a_{eq}<a<a_{DE} & \text{matter} \\
\text{const} & a>a_{DE} & \text{dark energy}
\end{cases}\tag{19.7} .$$
Before recombination, $c_{s}\approx \frac{c}{\sqrt{ 3 }}$ in a baryon-photon fluid hence
$$\lambda_{J_{b\gamma}}=\sqrt{ \frac{8}{3} }\pi\left( \frac{c_{s}}{c} \right)R_{H}\sim R_{H}\tag{19.8} .$$
For $\lambda\ll R_{H}$, perturbations in the baryon-photon fluid also have $\lambda\ll\lambda_{J_{b\gamma}}$. This implies the $\delta_{b\gamma}$ oscillates due to photon pressure.
The oscillation period is given by
$$T=\frac{\lambda}{c_{s}}\approx \frac{\lambda}{c}\ll \frac{R_{H}}{c}=\frac{1}{H}\approx t\tag{19.9} $$
which shows there are many oscillations in one expansion time, $T\ll t$.

Dark matter perturbations see rapidly oscillating gravitational fields due to the baryon-photon fluid.
From the [Meszaros equation](Gravitationally%20Coupled%20Fluids.md), cold dark matter perturbations with $\lambda\ll R_{H}$ do not grow while the universe is still dominated by radiation but start growing again one the universe is matter dominated.
![[Pasted image 20251120113638.png]]

With the adiabatic initial conditions, before recombination we have a baryon-photon fluid and between $a_{enter}\ll a\ll a_{rec}$, $\delta_{b\gamma}$ oscillates.

For $a_{enter}$ after matter-radiation equality,
![[Pasted image 20251120114651.png]]

Cold dark matter perturbations inside the horizon grow as
$$\delta_{CDM}\propto \begin{cases}
\text{const} & a<a_{eq} \\
a & a_{eq}<a<a_{DE} \\
\text{const} & a>a_{DE}
\end{cases}.\tag{19.10} $$
For $a<a_{eq}$, growth is supressed for perturbations inside the horizon.

For $a_{eq}<a$, $\delta_{DM}$ grows in the same way as if it is inside or outside the horizon. Dark matter is not affected by recombination. For warm dark matter and hot dark matter, particle random thermal velocities are not negligible so we get free streaming.

The comoving free streaming length is:
- $\ell_{FS}\sim \ell_{H}$ for $a<a_{nr}$ ($v_{*}\approx c$)
- $\ell_{FS}\sim\text{const}$ for $a>a_{nr}$ ($v_{*}<c$).

For $a<a_{nr}$, free streaming effectively starts to erase perturbations in dark matter as soon as $\delta$ enters the horizon.
There is a large effect on $\delta$ if dark matter particles are relativistic at horizon entry $(a_{enter}<a_{nr})$. There is only a small effect on $\delta$ if particles are non-relativistic at horizon entry $(a_{enter}>a_{nr})$.

Free streaming erases all $\delta_{DM}$ with comoving wavelength $\lambda_{com}\lesssim\ell_{FS}$ and cannot regrow later. Typically $a_{nr}<a_{eq}$ so free streaming effectively ceases for $a\gtrsim a_{eq}$.
![[Pasted image 20251120145609.png]]
After recombination, baryons decouple from photons so $c_{s}\ll c$ in baryons after recombination which gives $\lambda_{J_{b\gamma}}\ll R_{H}$. After recombination, all baryon perturbations with $\lambda>\lambda_{J_{b}}$ can grow due to gravity. Perturbations in baryons feel gravity from perturbations in dark matter so $\delta_{b}\approx\delta_{DM}$ after a few expansion times.

After recombination, photons can free stream. This erases all photon perturbations in the photon density on scales $\lambda\lesssim R_{H}$.
![[Pasted image 20251120150814.png]]
![[Pasted image 20251120151117.png]]
![[Pasted image 20251120151317.png]]
