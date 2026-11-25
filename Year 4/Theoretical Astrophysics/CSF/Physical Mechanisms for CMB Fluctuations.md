There are three main physical mechanisms for generating $\frac{\Delta T}{\bar{T}}$ on the last scattering surface:
- Intrinsic temperature fluctuations in the [[Baryon-Photon Fluid]]
- Gravitational potential perturbations
- Doppler shifts due to velocity perturbations in the baryon-photon fluid.

The same density fluctuations produces temperature fluctuations $\frac{\Delta T}{\bar{T}}$ via all three mechanisms, referred to as primary anisotropies. Normally this requires solving the Boltzmann equation for photons.

Outside the horizon, $\lambda>R_{H},\theta\gtrsim \theta_{H}$. Dark matter, baryons, and photons are still related by adiabatic relations,
$$\tag{24.1} \frac{\delta \rho_{DM}}{\bar{\rho}_{DM}}=\frac{\delta \rho_{b}}{\bar{\rho}_{b}}=\frac{3}{4} \frac{\delta \rho_{\gamma}}{\bar{\rho}_{\gamma}}. $$
They all grow at the same rate, $\delta \propto D_{+}\propto a$ and all are moving with the same velocity $\vec{v}$.

Inside the horizon, $\lambda<R_{H},\theta\lesssim\theta_{H}$. Baryons and photons coupled in the baryon-photon fluid for $a<a_{rec}$ and $c_{s}\simeq \frac{c}{\sqrt{ 3 }}$. $\delta_{b}$ and $\delta_{\gamma}$ oscillate, maintaining the adiabatic relation. Dark matter does not feel photon pressure, so $\delta_{DM}$ grows: $\delta_{DM}\propto a$. $\frac{\delta \rho}{\bar{\rho}}$ and $\vec{v}$ are different for dark matter and baryons/photons.
![[Pasted image 20251128184339.png]]
For $\delta \rho_{b}>0$, this implies compression so $\delta T>0$. For $\delta \rho_{b}<0$, this implies expansion or rarefracted so $\delta T<0$.

As photons have a blackbody spectrum, $\rho_{\gamma}\propto T^{4}$. Hence, temperature fluctuations in the baryon-photon fluid at recombination is
$$\frac{\delta T}{\bar{T}}=\frac{1}{4} \frac{\delta \rho_{\gamma}}{\bar{\rho}_{\gamma}}=\frac{1}{4}\left( \frac{4}{3} \frac{\delta \rho_{b}}{\bar{\rho}_{b}} \right).\tag{24.2} $$
Photons travelling to us from recombination have frequency $\nu \propto \frac{1}{a}$. But $\nu_{peak}\propto T$ for a blackbody spectrum from Wien's law which gives
$$T\propto \frac{1}{a}.\tag{24.3} $$This gives the CMB temperature fluctuations $\frac{\Delta T}{\bar{T}}$ measured on Earth is
$$\left( \frac{\Delta T}{\bar{T}} \right)_{intrinsic}=\left( \frac{\delta T}{\bar{T}} \right)_{rec}=\frac{1}{3}\left( \frac{\delta \rho_{b}}{\bar{\rho}_{b}} \right)_{rec}.\tag{24.4} $$
For $\lambda>R_{H}$, $\delta_{b}=\delta_{DM}$ so
$$\left( \frac{\Delta T}{\bar{T}} \right)_{intrinsic}=\frac{1}{3}\left( \frac{\delta \rho_{m}}{\bar{\rho}_{m}} \right)_{rec}.\tag{24.5} $$For $\lambda<R_{H}$, $\delta_{b}\neq \delta_{DM}$ which implies there is no simple relation of $\frac{\Delta T}{\bar{T}}$ to $\frac{\delta \rho_{m}}{\bar{\rho}_{m}}$.
![[Pasted image 20251129140827.png]]
The blackbody, has the dependence $T\propto \nu_{peak}$. The dependence on $a$ is then
$$\nu \propto \frac{1}{a},\;T\propto \frac{1}{a}\implies \frac{\Delta T}{\bar{T}}=\frac{\delta \nu}{\nu}.\tag{24.6} $$
For gravitational and Doppler effects, the fractional frequency shift $\frac{\delta \nu}{\nu}$ is independent of frequency $\nu$.

Consider the Sachs-Wolfe effect. $\frac{\delta \rho}{\bar{\rho}}$ generate fluctuations in the gravitational potential $\phi$.
![[Pasted image 20251129141255.png]]
The gravitational potential perturbations $\phi$ produces two effects:
- gravitational redshift
- Time dilation
Derivations assume matter domination ($a_{eq}\ll a_{rec}$), which is reasonable for most typical universes.

Gravitational redshift causes a change in photon frequency $\nu$ proportional to $\phi$,
$$\left( \frac{\Delta T}{\bar{T}} \right)_{grav.\,redshift}=\left( \frac{\delta \nu}{\nu} \right)_{grav.\,redshift}=\left( \frac{\phi}{c^2} \right)_{rec}.\tag{24.7} $$
For an overdense region, $\phi<0\implies\Delta T<0$ i.e. a drop in temperature.

Time dilation causes clocks to run slower in gravitational potential wells,
$$\frac{\delta t_{rec}}{t_{rec}}=-\left( \frac{\phi}{c^2} \right)_{rec}.\tag{24.8} $$
As $T\propto \frac{1}{a}$, the CMB temperature measured on Earth is $T=T_{rec}a_{rec}\propto a_{rec}\propto t_{rec}^{2/3}$ so
$$\left( \frac{\Delta T}{\bar{T}} \right)_{time\,dilation}=\frac{2}{3} \frac{\delta t_{rec}}{t_{rec}}=-\frac{2}{3}\left( \frac{\phi}{c^2} \right)_{rec}\tag{24.9}. $$
Combining gravitational redshift and time-dilation gives the Sachs-Wolfe effect.
$$\left( \frac{\Delta T}{\bar{T}} \right)_{SW}=\frac{1}{3} \frac{\phi}{c^2}.\tag{24.10} $$
To calculate this from the density perturbations, we need to solve [[Poisson's Equations]] for $\phi$ at recombination,
$$\nabla^2_{\vec{x}}\phi=4\pi Ga^2\delta \rho \tag{24.11} .$$
Since $\bar{\rho}_{m}\gg \bar{\rho}_{r}$ as $a_{eq}\ll a_{rec}$,
$$\nabla^2_{\vec{x}}\phi=4\pi Ga^2\bar{\rho}_{m}\delta_{m}\tag{24.12} .$$
For a single plane wave, $\delta_{m}=\delta_{m,k}e^{ i\vec{k}\cdot \vec{x} }$ then $\phi=\phi_{k}e^{ i\vec{k}\cdot \vec{x} }$ implies
$$\nabla^2_{\vec{x}}\phi=-k^2\phi \tag{24.13} $$
with
$$\phi_{k}=-\frac{4\pi Ga^2\bar{\rho}_{m}\delta_{m,k}}{k^2}=-\frac{3}{8\pi^2}H^2\lambda^2\delta_{m,k}.\tag{24.14} $$
The amplitude of the Sachs-Wolfe effect due to a single plane wave perturbation is
$$\left\lvert  \frac{\Delta T}{\bar{T}}  \right\rvert_{SW,k}=\left\lvert  \frac{1}{3} \frac{\phi}{c^2}  \right\rvert  =\frac{1}{8\pi^2}\left( \frac{\lambda(a_{rec})}{R_{H}(a_{rec})} \right)^2\left( \frac{\delta \rho_{m}(a_{rec})}{\bar{\rho}_{m}(a_{rec})} \right)_{k}\tag{24.15} $$
using $R_{H}=\frac{c}{H}$ and with all values on the right hand side taken at recombination.
$$\implies \frac{\Delta T}{\bar{T}}\propto e^{ i\vec{k}\cdot \vec{x} }.\tag{24.16} $$
The comoving wavenumber $k$ is related to the proper wavelength $\lambda$ at $a=a_{rec}$ by $k=\frac{2\pi a_{rec}}{\lambda(a_{rec})}$. $$\frac{\delta \rho_{m}}{\bar{\rho}_{m}}\approx \frac{\delta \rho_{DM}}{\bar{\rho}_{DM}}\tag{24.17} $$on all scales since $\bar{\rho}_{b}\ll \bar{\rho}_{m}$. The same relation for the Sachs-Wolfe effects for $\lambda>R_{H}$ and $\lambda<R_{H}$, $\delta_{m,k}>0$ (i.e. $(\delta \rho_{m})_{k}>0$) $\implies (\Delta T)_{SW,k}<0$. 
![[Pasted image 20251129144639.png]]
Velocity perturbations $\vec{v}_{b}$ in the baryon-photon fluid at recombination cause a Doppler shift in the frequency of emitted photons. $\vec{v}_{b}$ is perpendicular to the wave front $\vec{v}_{b}\parallel \vec{k}$.
$$\left( \frac{\Delta T}{\bar{T}} \right)_{Doppler}=\frac{\delta \nu}{\nu}=\left( \frac{v_{b}}{c} \right)_{rec}\cos \beta \tag{24.18} $$where $\beta$ is the angle between the baryon-photon fluid velocity $\vec{v}_{b}$ and the line of sight to the observer.

We need to solve the [perturbed continuity equation](Exact%20Perturbation%20Equations.md) for $\vec{v}_{b}$
$$\left. \frac{\partial\delta}{\partial t}\right|_{\vec{x}}+\frac{1}{a}\vec{\nabla}_{\vec{x}}\cdot \vec{v}_{b}=0\tag{24.19} .$$
For a single plane-wave ($\delta_{b}\propto e^{ i\vec{k}\cdot \vec{x} }$) gives $\vec{v}_{b}=\vec{v}_{b,k}e^{ i\vec{k}\cdot \vec{x} }$ and $\vec{v}_{b}\parallel \vec{k}$ so $\vec{\nabla}_{\vec{x}}\cdot \vec{v}_{b}=i\vec{k}\cdot \vec{v}_{b}=ikv_{b,k}$.

The time dependence is given by the growth factor $\delta_{b}\propto D_{+}(t,k)\implies \frac{\partial\delta_{b}}{\partial t}=\left( \frac{\dot{D}_{+}}{D_{+}} \right)\delta_{b}$.

The perturbation in fluid velocity, associated with $k$ becomes
$$\frac{\dot{D}_{+}}{D_{+}}\delta_{b}+\frac{ikv_{b,k}}{a}=0\implies v_{b,k}=i \frac{a}{k} \frac{\dot{D}_{+}}{D_{+}}\delta_{b,k}\tag{24.20} $$
where $i=e^{ i\pi/2 }$ implies $\vec{v}$ is out of phase by $90^{\circ}$ with respect to $\delta_{b}$. The amplitude of the Doppler effect due to a single plane wave perturbation,
$$\left\lvert  \frac{\Delta T}{\bar{T}}  \right\rvert _{Doppler,k}=\frac{|v_{b,k}|}{c}\cos \beta_{k}=\frac{1}{c}\left( \frac{\lambda(a_{rec})}{2\pi} \right)\left\lvert  \frac{\dot{D}_{+}(a_{rec})}{D_{+}(a_{rec})}  \right\rvert \left( \frac{\delta \rho_{b}(a_{rec})}{\bar{\rho}_{b}(a_{rec})} \right)_{k}\cos \beta_{k}.\tag{24.21} $$
For $\lambda>R_{H}$: $\delta_{b}=\delta_{DM}$ and $D_{+}\propto a\propto t^{2/3}=2 \frac{\dot{D}_{+}}{D_{+}}=\frac{2}{3t}=H=\frac{c}{R_{H}}$ so
$$\left\lvert  \frac{\Delta T}{\bar{T}}  \right\rvert _{Doppler,k}=\frac{1}{2\pi}\left( \frac{\lambda(a_{rec})}{R_{H}(a_{rec})} \right)\left( \frac{\delta \rho_{m}(a_{rec})}{\bar{\rho}_{m}(a_{rec})} \right)_{k}\cos \beta_{k}\tag{24.22} .$$For $\lambda<R_{H}$: $\delta_{b}\neq\delta_{DM}$ so the baryon-photon fluid oscillates $\implies D_{+}\propto e^{ i\omega_{k}t }\implies \frac{\dot{D}_{+}}{D_{+}}=i\omega_{k}\approx \frac{ic_{s}k}{a}= \frac{ic_{s}2\pi}{\lambda}$ so
$$\left\lvert  \frac{\Delta T}{\bar{T}}  \right\rvert _{Doppler,k}=\left( \frac{c_{s}(a_{rec})}{c} \right)\left( \frac{\delta \rho_{b}(a_{rec})}{\bar{\rho}_{b}(a_{rec})} \right)\cos \beta_{k}.\tag{24.23} $$
The importance of the contribution of different mechanisms depends on how the proper wavelength $\lambda$ compares to the horizon scale $R_{H}$ at recombination.
$\lambda\gtrsim R_{H}$ ($\theta\gtrsim \theta_{H}$): Superhorizon scales
$$\left( \frac{\Delta T}{\bar{T}} \right)_{intrinsic}:\left( \frac{\Delta T}{\bar{T}} \right)_{Doppler}:\left( \frac{\Delta T}{\bar{T}} \right)_{SW}\sim 1:\left( \frac{\lambda}{R_{H}} \right):\left( \frac{\lambda}{R_{H}} \right)^2\tag{24.24} $$which shows the gravitational Sachs-Wolfe term dominated for $\lambda\gtrsim R_{H}$.

For $\lambda\lesssim R_{H}$: Subhorizon scales
$$\left( \frac{\Delta T}{\bar{T}} \right)_{SW}\ll \left( \frac{\Delta T}{\bar{T}} \right)_{intrinsic}\sim \left( \frac{\Delta T}{\bar{T}} \right)_{Doppler}\tag{24.25} $$assuming $\delta_{b}\approx\delta_{DM}$ at $a=a_{enter}$ and $\delta_{b}$ oscillating with constant amplitude. This shows that intrinsic and Doppler dominate for $\lambda\lesssim R_{H}$.#![[Pasted image 20251129151755.png]]
For low $\ell$ $(\ell\lesssim 100)$ (large angular scales):
	$\ell(\ell+1)C_{\ell}$ is approximately constant due to gravitational perturbations arising from the spectrum of density perturbations with $P(k)\propto k$.
For intermediate $\ell$ $(100\lesssim \ell\lesssim 1000)$:
	$\ell(\ell+1)C_{\ell}$ peaks at $\ell \approx 200$ then oscillates with $\ell$ due to intrinsic and Doppler perturbations $(\lambda\lesssim R_{H})$ due to sound waves (acoustic oscillations)
For high $\ell$ ($\ell\gtrsim{1}000$) (small angular scales):
	$\ell(\ell+1)C_{\ell}$ declines with increasing $\ell$ that results from damping of acoustic oscillations by photon diffusion around recombination.
![[Pasted image 20251129152334.png]]

$\frac{\delta \rho_{b}}{\bar{\rho}_{b}}$ vs $t$ for plane waves with 3 different comoving wavelengths.
![[Pasted image 20251129152451.png]]
- Outside horizon: $\delta_{b}$ grows due to gravity
- Inside horizon: $\delta_{b}$ oscillates as sound waves due to pressure in the baryon-photon fluid starting at a maximum at $a_{enter}\to \cos(\psi(t,k))$.
- Depending on $\lambda$, and hence $k$, $\delta_{b}$ arrives with different phases at recombination $\psi(t_{rec},k)$.

The density perturbations in the baryon-photon fluid oscillate as sound waves for $\lambda<R_{H}$,
$$\omega(k,t)\approx \frac{c_{s}(t)k}{a(t)}\tag{24.26} .$$
The total phase change of the sound wave at $t=t_{rec}$
$$\psi(t_{rec},k)\approx \int_{0}^{t_{rec}}\omega(k,t')dt'=k\int_{0}^{t_{rec}} \frac{c_{s}(t')dt'}{a(t')}=kr_{s}(t_{rec})\tag{24.27} $$where $r_{s}$ is the comoving sound horizon, the distance a sound wave could have travelled since the big bang,
$$r_{s}(t)\equiv \int_{0}^{t} \frac{c_{s}(t')dt'}{a(t')}\tag{24.28} .$$
Then $\frac{\delta \rho_{b}}{\bar{\rho}_{b}}\propto \cos(\psi(t,k))=\cos(kr_{s}(t))$.

The intrinsic contribution to $\frac{\Delta T}{\bar{T}}$ is
$$\left( \frac{\Delta T}{\bar{T}} \right)^2_{intrinsic}\propto \left( \frac{\delta \rho_{b}}{\bar{\rho}_{b}} \right)^2_{rec}\propto \cos^2(kr_{s}(t_{rec})) \tag{24.29} $$so has peaks for $\cos(kr_{s}(t_{rec}))=\pm 1$ so for comoving wavenumbers $k$:
$$k=\frac{m\pi}{r_{s}(t_{rec})},\;m\in \mathbb{N}.\tag{24.30} $$
![[Pasted image 20251129153527.png]]
For density perturbations at recombination,
$$\ell \approx 2\pi\frac{d_{A}(a_{rec})}{\lambda}=k \frac{d_{A}(a_{rec})}{a_{rec}}\tag{24.31} .$$The angular power spectrum $C_{\ell}$ therefore has peaks at $$\ell_{m}\approx m\pi  \frac{d_{A}(a_{rec})}{a(t_{rec})r_{s}(t_{rec})}.\tag{24.32} $$
![[Pasted image 20251204111918.png]]
This diagram shows the effect of variations in cosmological parameters $(\Omega_{tot},\Omega_{\Lambda},\Omega_{b}h^2,\Omega_{m}h^2)$or the angular power spectrum of the CMB for $\Delta T$ for the $\Lambda CDM$ model. In each panel, only the parameter shown varies - all others are fixed.

Different features in the angular power spectrum $C_{\ell}$ is sensitive to different cosmological parameters. The position of the first peak corresponds to an angular size of the horizon at recombination. It depends mainly on curvature.
The observed $\ell_{1}=200$ is for a flat universe. The form at low $\ell$ sensitive to initial density fluctuation spectrum $P(k)=Ak^{n}$. The observed shape of $C_{\ell}\implies n\approx 1$. The relative heights of different peaks are sensitive to $\Omega_{m}$ and $\Omega_{b}$.