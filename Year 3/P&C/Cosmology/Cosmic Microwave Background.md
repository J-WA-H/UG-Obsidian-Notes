The cosmic microwave background (CMB) is the surface of last scattering - the universe becomes transparent and photons free to stream across the universe once electrons and protons combine to form the first atoms.

The CMB is known as the epoch of recombination - where electrons and protons form neutral atoms - or decoupling (where photons decouple from electrons).

The CMB follows a perfect black body, where the intensity is given by
$$I(\nu,t)d\nu= \frac{8\pi \nu^2d\nu}{c^3} \frac{h\nu}{\exp\left[ \frac{h\nu}{k_{B}T} \right]-1}.$$
To calculate the energy density of the CMB, first consider the number density,
$$n(\nu,T)d\nu=\frac{I(\nu,T)d\nu}{h\nu}=\frac{8\pi \nu^2}{c^3} \frac{d\nu}{\exp\left[ \frac{h\nu}{k_{B}T} \right]-1}.$$
$$\varepsilon(T)=\int_{0}^{\infty} I(\nu,T)d\nu=\frac{8\pi h}{c^3}\int_{0}^{\infty} \frac{\nu^3d\nu}{\exp\left[ \frac{h\nu}{k_{B}T} \right]-1}.$$
Let $x=\frac{h\nu}{k_{B}T}$ so $dx=\frac{h}{k_{B}T}d\nu$
$$\therefore \varepsilon(T)=\frac{8\pi h}{c^3} \left( \frac{k_{B}T}{h} \right)^4 \int_{0}^{\infty} \frac{x^3dx}{e^{x}-1}.$$
Evaluating the integral gives
$$\int_{0}^{\infty} \frac{x^3dx}{e^{x}-1}=\Gamma(4)\zeta(4)$$
using the [gamma function](Common%20Laplace%20Transforms.md) and the Riemann-zeta function,
$$\zeta(s)=\sum_{n=1}^{\infty} \frac{1}{n^{s}}.$$
Evaluating these two functions analytically gives
$$\varepsilon(T)=\frac{8\pi^5}{15c^3h^3}(k_{B}T)^4.$$
For the number density
$$n(T)=\frac{8\pi}{c^3}\int_{0}^{\infty} \frac{\nu^2d\nu}{\exp\left[ \frac{h\nu}{k_{B}T} \right]-1}=\frac{16\pi}{h^3c^3}\zeta(3)(k_{B}T)^3.$$
This gives the mean photon energy is
$$\langle E_{\gamma} \rangle =\frac{\varepsilon(T)}{n(T)}=\frac{\pi^4}{3o\zeta(3)}k_{B}T\approx 2.7k_{B}T\approx 3k_{B}T.$$
This is approximately the expected energy.

It can be shown that
$$\varepsilon \propto a^{-4};\; n\propto a^{-3}\implies \langle E_{\gamma} \rangle \propto a^{-1}.$$
$$\therefore T_{CMB}\propto a^{-1}=T_{CMB_{0}}a^{-1}.$$
Where today, $T_{CMB_{0}}=2.725\text{ K}$.

Considering baryonic matter, 
$$n_{B}=\frac{\rho_{B_{0}}}{m_{p}}=\frac{3H_{0}^2\Omega_{B_{0}}}{8\pi Gm_{p}}.$$
$$\therefore \frac{n_{\gamma_{0}}}{n_{B_{0}}}\approx 1.5\times 10^{9}.$$
There are two methods to try to calculate the epoch of CMB production.
Attempt 1: equate hydrogen ionisation energy to mean photon energy:
$$13.6=3k_{B}T_{CMB_{0}}(1+z_{rec})\implies z_{rec}=19,300.$$
This is much higher than the true value of $z_{rec}=1,089$. 

This estimate is so wrong as the energy is on a black body spectrum.

We only need a few photons to ionise atoms as the exponential tail of the black body spectrum can allow for this.

To calculate a more accurate $z_{rec}$,
$$\frac{n_{B}}{n_{\gamma}}\equiv 10^{-9}=\frac{\int_{\nu_{min}}^{\infty}n(\nu,T)d\nu}{\int_{0}^{\infty}n(\nu,T)d\nu}$$
$$\int_{\nu_{min}}^{\infty}n(\nu,T)d\nu=\int_{v_{min}}^{\infty} \frac{8\pi \nu^2}{c^3} \frac{d\nu}{\exp\left( \frac{h\nu}{k_{B}T} \right)}.$$
The -1 is neglected as $h\nu_{min}\gg k_{B}T$.
$$=\frac{8\pi}{c^3} \left( \frac{k_{B}T}{h} \right)^3 \left( \frac{h\nu_{min}}{k_{B}T} \right)\exp\left[ \frac{h\nu}{k_{B}T} \right]$$
$$\therefore \frac{n_{B}}{n_{\gamma}}=\frac{1}{2\zeta(3)} \left( \frac{h\nu_{min}}{k_{B}T} \right)^2\exp\left[ -\frac{h\nu_{min}}{k_{B}T} \right]$$
$$\implies z_{rec}=3,000.$$
This is of the same order as the true value so this is a more accurate estimate.
