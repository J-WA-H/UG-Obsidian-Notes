Linear perturbations assume $|\delta|\ll 1$. This breaks down completely when $|\delta|\gtrsim 1$, when the structures become non-linear.

For overdense regions ($\delta>0$), with $\delta\gtrsim 1$, structures stop expanding with Hubble flow and collapse to form gravitationally bound structures in dynamical equilibrium.
For underdense regions ($\delta<0$), this forms expanding voids with $\delta \approx-1$. For dark matter, collapsed structures are dark matter halos. For baryons, galaxies form by further collapse (dissipating energy) relative to dark matter. There is no general analytical solutions for non-linear evolution. We need numerical simulations.

Non-linear evolution results in the collapse of overdense regions to form dark matter halos. Exact analytical solutions for the spherical density perturbation, this is a useful guide to what happens in more realistic cases:
- Time of collapse and its relation to the initial overdensity
- Final density of dark matter halos and its dependence on the collapse redshift.

Assume a spherical perturbation with a uniform overdensity consisting of collisionless dark matter with zero pressure. Also assume a flat matter dominated universe $(\Omega=\Omega_{m}=1)$ for simplicity.
![[Pasted image 20251204120527.png]]
Consider a sphere of mass $M$, proper radius $R$, with an initially uniform overdensity. There is no gravitational force on the sphere.
The proper radius $R(t)$ of the sphere contains a constant mass $M$ evolves as
$$\frac{d^2R}{dt^2}=-\frac{GM}{R^2}.\tag{25.1} $$
This integrates to$$\frac{1}{2}\left( \frac{dR}{dt} \right)^2-\frac{GM}{R}=E\tag{25.2} $$where $E$ is the energy per unit mass.
$$\implies \left( \frac{dR}{dt} \right)^2=2\left( \frac{GM}{R}+E \right)\tag{25.3} .$$Consider gravitationally bound case, $E<0$ which leads to collapse/ Setting $R=0$ at $t=0$ gives
$$t=\int_{0}^{R} \frac{dr}{\sqrt{ 2\left( \frac{GM}{r}+E \right) }}\tag{25.4}. $$This is solved by a change of variables $r=\frac{GM}{|E|}\sin^2\phi$, and the parametric solution for $R(t)$ in terms of $\theta=2\phi$ and
$$\begin{matrix}
R=A(1-\cos \theta), & t=B(\theta-\sin \theta)
\end{matrix}\tag{25.5}. $$
$$A=\frac{GM}{2|E|},\; B=\frac{GM}{(2|E|)^{3/2}}\tag{25.6} .$$
Plotting this gives
![[Pasted image 20251204122305.png]]
The evolution of the radius $R$ of a uniform density spherical density perturbation. The sphere expands to its maximum radius $R_{max}$ at $t=t_{max}(\theta=\pi)$ and then collapses to zero radius at $t=t_{coll}=2t_{max}(\theta=2\pi)$.

The sphere expands from $R=0$ at time $t=0$ for $\theta=0$. This expands to turn around the radius $R_{max}=2A$ at time $\pi B(\theta=\pi)$. This then collapses to $R=0$ at time $t_{coll}=2t_{max}=2\pi B$. Re-expansion is prevented by other physical mechanisms.
![[Pasted image 20251204122831.png]]
The mean density inside the sphere is
$$\rho=\frac{M}{\frac{4}{3}\pi R^3}=\frac{3M}{4\pi A^3} \frac{1}{(1-\cos \theta)^3}.\tag{25.7} $$
The mean density for a background $\Omega_{m}=1$ universe,
$$\bar{\rho}= \frac{1}{6\pi Gt^2}= \frac{1}{6\pi GB^2} \frac{1}{(\theta-\sin \theta)^2}.\tag{25.8} $$
The actual non-linear overdensity is (exact solution),
$$1+\delta=\frac{\rho}{\bar{\rho}}=\frac{9}{2} \frac{(\theta-\sin \theta)^2}{(1-\cos \theta)^3}.\tag{25.9} $$
Taylor expand this for $\theta\ll 1(t\ll t_{max})$ to find the initial expansion,
$$\sin \theta=\theta-\frac{\theta^3}{3!}+\frac{\theta^5}{5!},\;\cos \theta=1-\frac{\theta^2}{2!}+\frac{\theta^4}{4!}.\tag{25.10} $$This gives
$$\delta \approx \frac{3}{20} (6\pi)^{2/3}\left( \frac{t}{t_{max}} \right)^{2/3},\;t\approx \frac{B}{6}\theta^3.\tag{25.11} $$
This shows that this grows at the same rate as the [growing mode](Perturbations%20Outside%20Horizon.md) for linear perturbation theory for $\Omega=\Omega_{m}=1$. If $\delta=\delta_{i}\ll 1$ at $t_{i}\ll t_{max}$ the sphere collapses to $R=0$ at time
$$t_{coll}=2t_{max}=12\pi\left( \frac{3}{20} \right)^{3/2} \frac{t_{i}}{\delta_{i}^{3/2}}.\tag{25.12} $$
This implies perturbations with a large $\delta_{i}$ at $t_{i}$ collapses at earlier times.

According to linear perturbation theory in $\Omega_{m}=\Omega=1$ universe
$$\delta_{L}=\delta_{i}\left( \frac{t}{t_{i}} \right)^{2/3}\tag{25.13} $$so $\delta(t)\approx \delta_{L}(t)$ for $t\ll t_{max}$.
At $t=t_{max}$, overdensity is extrapolated according to linear theory,
$$\delta_{L}(t_{max})=\frac{3}{20}(6\pi)^{2/3}=1.062\tag{25.14} $$while the actual non-linear overdensity is ($\theta=\pi$ at $t=t_{max}$)
$$\delta(t_{max})=\left\lvert  \frac{9}{2} \frac{(\theta-\sin \theta)^2}{(1-\cos \theta)^4} \right\rvert_{\theta=\pi}-1=\frac{9\pi^2}{16}-1=4.55.\tag{25.15} $$
This implies overdensity is already appreciable non-linear when $\delta_{L}\approx 1$.
At $t=t_{coll}=2t_{max}$, the overdensity extrapolated according to linear theory is
$$\delta_{L,coll}=\delta_{L}(t_{coll})=\frac{3}{20}(6\pi)^{2/3}\left( \frac{t_{coll}}{t_{max}} \right)^{2/3}=\frac{3}{20}(12\pi)^{2/3}=1.686\tag{25.16}. $$
The collapse of density perturbations happens when $\delta_{L}\simeq 1$. Collapse happens in terms of the initial overdensity $\delta_{i}$ at time
$$t_{coll}=2t_{max}=t_{i}\left( \frac{\delta_{L,coll}}{\delta_{i}} \right)^{3/2}\propto\delta_{i}^{-3/2}.\tag{25.17} $$
Hence initially more overdense perturbations collapse earlier. This is a very similar result even for $\Omega_{m}\neq 1$, $\delta_{L,coll}=\delta_{L,coll}(\Omega_{m},\Omega_{v})$, with a weak dependence on $\Omega_{m},\Omega_{v}$.
![[Pasted image 20251204173952.png]]
A collapse down to $R=0$ is not physically realistic. Instead, collapsing sphere relaxes to an equilibrium radius $R_{f}$. $R_{f}$ is calculated using energy conservation and the virial theorem.
The total kinetic energy $E=K+U$. At turnaround, the total energy is (since $K=0$)
$$E_{max}=U_{max}=-\frac{3}{5} \frac{GM^2}{R_{max}}\tag{25.18}. $$
Assume it collapses to a uniform spherical halo of radius $R_{f}$ in dynamical equilibrium. With the virial theorem $2K_{f}+U_{f}=0$, the total energy of the final halo is
$$E_{f}=K_{f}+U_{f}=\frac{1}{2}U_{f}=-\frac{3}{10} \frac{GM^2}{R_{f}}\tag{25.19}. $$The total energy of collisionless dark matter is conserved during collapse, so $E_{f}=E_{max}$, so
$$R_{f}=\frac{1}{2}R_{max}\tag{25.20}. $$
As mass is conserved, the final density $\rho_{f}$ is $2^{3}=8\times\text{density}$ at $t=t_{max}$. Using $\bar{\rho}_{m}=\bar{\rho}\propto t^{-2}$. the overdensity of the halo at time $t\approx t_{coll}$ when it virialises is
$$1+\delta_{vir}=\frac{\rho_{f}}{\bar{\rho}_{m}(t_{coll})}=\frac{\rho_{f}}{\bar{\rho}(t_{coll})}=\left( \frac{\rho_{f}}{\rho(t_{max})} \right)\left( \frac{\rho(t_{max})}{\bar{\rho}(t_{max})} \right)\left( \frac{\bar{\rho}(t_{max})}{\bar{\rho}(t_{coll})} \right)=8\times(1+\delta(t_{max}))\times\left( \frac{t_{max}}{t_{coll}} \right)^{-2}=8\times \frac{9\pi^2}{16}\times{4}\tag{25.21}. $$
Therefore $1+\delta_{vir}=18\pi^2=178$. We get similar results for $\frac{\rho_{f}}{\bar{\rho}_{m}}$ for $\Omega_{m}\neq 1$.

For a dark matter halo which forms at redshift $z_{coll}$, the mean density after it has reached virial equilibrium is 
$$\rho_{vir}=(1+\delta_{vir})\bar{\rho}_{m}(z_{coll})=(1+\delta_{vir})\bar{\rho}_{m_{0}}(1+z_{coll})^3\tag{25.22} $$where $\rho_{vir}=\rho_{f}$ as halo density remains constant and equal to $\rho_{vir}$ for $t>t_{coll}$. Ignoring any variation in $\delta_{vir}$ (true for $\Omega_{m}=1$), $\rho_{vir}\propto (1+z_{coll})^3$. The radius of a virialised halo is
$$R_{vir}=\left( \frac{M}{\frac{4\pi}{3}\rho_{vir}} \right)^{1/3}\propto \frac{M^{1/3}}{1+z_{coll}}\tag{25.23}. $$This shows the radius of the halo depends on formation redshift, with earlier formed halos of the same mass having smaller radii.

The circular velocity at the halo edge is$$V_{c}=\left( \frac{GM}{R_{vir}} \right)^{1/2}\tag{25.24}. $$Using virial theorem and modelling the halo as a uniform density sphere, the 3D velocity dispersion $\sigma$ of dark matter particles in the halo is
$$\sigma=\left( \frac{3}{5} \frac{GM}{R_{vir}} \right)^{1/2}\tag{25.25}. $$Thus a key relation for spherical dark matter halos:
$$\sigma \propto V_{c}\propto\left( \frac{M}{R_{vir}} \right)^{1/2}\propto M^{1/3}(1+z_{coll})^{1/2}\tag{25.26} $$
using $(25.23)$. This implies halos of the same mass formed at higher redshifts have a larger $\sigma$ or $V_{c}$.
The Milky Way halo has $M\approx 10^{12}M_{\odot}$, $z_{coll}\approx 1$, and using $1+\delta_{vir}=18\pi^2$, we get $R_{vir}=160\text{ kpc}$ and $V_{c}\approx 170\text{ km s}^{-1}$ - similar to observed.