For uniform expansion, there must be a proper separation $r(t)$ of any pair of points,
$$r(t)=a(t)x\tag{3.1} $$where $x$ is the fixed comoving separation and $a(t)$ is the cosmological scale factor which is normalised such that $a(t_{0})=1$ today. For light emitted of wavelength $\lambda_{e}$ and observed at $\lambda_{o}$, the redshift is defined by
$$1+z=\frac{\lambda_{o}}{\lambda_{e}}\tag{3.2} .$$For light emitted at time $t$ and observed today at $t_{0}$, $\lambda \propto a$ so 
$$1+z=\frac{a(t_{0})}{a(t)}=\frac{1}{a(t)}.\tag{3.3} $$
For a pair of galaxies moving with cosmic flow, their relative velocity is
$$u=\frac{dr}{dt}=\dot{a}(t)x=H(t)r\tag{3.4} $$where
$$H(t)\equiv \frac{\dot{a}}{a}\tag{3.5} $$which denotes the Hubble expansion rate. $H_{0}=H(t_{0})$ is the current value of the Hubble expansion rate. This can also be expressed as the dimensionless Hubble constant
$$h\equiv \frac{H_{0}}{100\text{ km s}^{-1}\text{Mpc}^{-1}}.\tag{3.6} $$
Current observations give $H_{0}=70\text{ km s}^{-1}\text{Mpc}^{-1}$ with uncertainty $5-10\%$. For this model we will use the round number $H_{0}=70\text{ km s}^{-1}\text{Mpc}^{-1}$ with $h=0.7$ for numerical estimates.

In general relativity, space can be curved. Curvature is measured by the curvature constant $k$:
- Flat, Euclidean space corresponds to $k=0$
- Closed curvature $k>0$ (left)
- Open curvature $k<0$ (right)
![[Pasted image 20251017095955.png]]

Einstein's equations of general relativity leads to two independent equations for $a(t)$ - the Friedmann and acceleration equations
$$H^2\equiv\left( \frac{\dot{a}}{a} \right)^2=\frac{8\pi G\rho}{3}-\frac{kc^2}{a^2}\tag{3.7} $$
$$\frac{\ddot{a}}{a}=-\frac{4\pi G}{3}\left( \rho+\frac{3p}{c^2} \right)\tag{3.8} $$ where $\rho,p$ are the total density and pressure from all forms of matter and energy.

For normal matter, $\rho>0$ and $p\geq 0$ so the universe decelerates.
For dark energy, $\rho>0$ and $p<0$ so the universe accelerates.

From the first law of thermodynamics, total energy must be conserved,
$$dU+pdV=0.\tag{3.9} $$
In an expanding universe, $U=\rho c^2V$ and $V\propto a^{3}$ which gives the density equation
$$\frac{d\rho}{dt}+3 \frac{\dot{a}}{a}\left( \rho+\frac{p}{c^2} \right)=0.\tag{3.10} $$
This applies to each component of matter individually if these interact only with gravity.

Consider a simple equation of state, $p=w\rho c^2$ where $w$ is some constant. This simplifies the density equation to$$\frac{\dot{\rho}}{\rho}=-3(1+w) \frac{\dot{a}}{a}\tag{3.11} $$which has solutions
$$\rho(t)\propto a(t)^{-3(1+w)}.\tag{3.12} $$
For non-relativistic matter, $\rho_{m}\ll \rho_{m}c^2$ so we an approximate $\rho_{m}\approx 0$ so take $w=0$ so 
$$\rho_{m}=\rho_{m_{0}}a^{-3}=\rho_{m_{0}}(1+z)^3.\tag{3.13} $$
This is equivalent to the conservation of rest mass.

For radiation, photons and massless particles and extreme relativistic particles, $w=\frac{1}{3}$ so
$$\rho_{r}=\rho_{r_{0}}a^{-4}=\rho_{r_{0}}(1+z)^4.\tag{3.14} $$
The vacuum energy is given by a quantum field in its ground state with a constant non-zero density $\rho_{v}$. Since theses fields are Lorentz invariant, $p_{v}=-\rho_{v}c^2$ where $\rho_{v}=\rho_{v_{0}}$ is the present day vacuum density - which comes from energy conservation.

The vacuum energy behaves as a uniform density fluid with a negative pressure, so it is a type of dark energy. The vacuum energy is hence equivalent to the cosmological constant,$$\rho_{v}\equiv \frac{\Lambda c^2}{8\pi G}\tag{3.15} $$ and the Friedmann and acceleration equations become
$$\left( \frac{\dot{a}}{a} \right)^2=\frac{8\pi G(\rho_{m}+\rho_{r})}{3}+\frac{\Lambda c^2}{3}-\frac{kc^2}{a^2\tag{3.16} },$$
$$\frac{\ddot{a}}{a}=-\frac{4\pi G}{3}\left( \rho_{m}+\rho_{r}+\frac{3\rho_{r}}{c^2} \right)+\frac{\Lambda c^2}{3}\tag{3.17} $$
$\therefore \Lambda<0$.
From the acceleration equation, $\rho+\frac{3p}{c^2}<0$ so $p<-\frac{1}{3}\rho c^2$. A field with $p<0$ is dark energy.

In general, $\rho_{DE}$ can be time varying but observations tend to imply it is constant. Vacuum energy is a special case of dark energy.