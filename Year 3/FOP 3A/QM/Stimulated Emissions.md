Spontaneous emission occurs when an electron deexcites from one energy level to a lower one. 
![[Pasted image 20241108142931.png]]
Einstein's solution for the probability amplitudes of this emission puts atoms in thermal equilibrium with a photon gas of temperature $T$ (Blackbody radiation).

The [stimulated emission probability](Electrons%20In%20Atoms%20in%20an%20EM%20field.md) is given by
$$P_{b\to a}(\omega,t)=\frac{\lvert p_{z}\rvert^{2}E_{0}^{2}}{\hbar^2} \frac{{\sin ^{2}\left[\frac{(\omega-\omega_{0})t}{2}\right]}}{(\omega-\omega_{0})^{2}}.$$
From electrodynamics we have the energy density of a time varying E-field
$$\frac{U}{V}=\frac{\varepsilon_{0}}{2}E_{0}^{2}\implies E_{0}^{2}=\frac{2}{\varepsilon_{0}} \left( \frac{U}{V} \right).$$
For black body radiation, 
$$\frac{U}{V}=\rho(\omega)=\frac{\hbar\omega^3}{\pi c^{3}} \frac{1}{\exp\left( \frac{\hbar\omega}{k_{B}T} \right)-1}$$
so
$$E_{0}^{2}=\frac{2}{\varepsilon_{0}}\rho(\omega)=\frac{2}{\varepsilon_{0}} \frac{\hbar\omega^{3}}{\pi c^{3}} \frac{1}{\exp\left( \frac{\hbar\omega}{k_{B}T} \right)-1}.$$
This can be used to find the time dependent probability of stimulated emission:
$$P_{b\to a}(t)=\int_{0}^{\infty} d\omega\frac{\lvert p_{z}\rvert^2}{\hbar^2} \frac{2}{\varepsilon_{0}}\rho (\omega)  \frac{{\sin ^{2}\left[\frac{(\omega-\omega_{0})t}{2}\right]}}{(\omega-\omega_{0})^{2}}$$
At the high time limit, the sinc function becomes a delta function, giving
$$P_{b\to a}(t)=\int_{0}^{\infty}d\omega  \frac{{\lvert p_{z} \rvert^2 }}{\hbar^2} \frac{2}{\varepsilon_{0}}\rho(\omega) \frac{\pi t}{2}\delta(\omega-\omega_{0})$$
$$=\frac{{\lvert p_{z} \rvert^2\pi t }}{\varepsilon_{0}\hbar^2}\rho(\omega_{0}).$$
We call $\omega_{0}$ the natural frequency.

The rate of this emission is given by
$$R_{b\to a}=\frac{dP_{b\to a}}{dt}=\frac{{\lvert p_{z} \rvert^2\pi }}{\varepsilon_{0}\hbar^2}\rho(\omega_{0}).$$
Since E can have many polarisations, we have to consider the electric dipole in all 3 dimensions
$$(p)_{ba}=\bra{\psi_{b}}qx\ket{\psi_{a}}\underline{\hat{x}}+\bra{\psi_{b}}qy\ket{\psi_{a}}\underline{\hat{y}}+\bra{\psi_{b}}qz\ket{\psi_{a}}\underline{\hat{z}}.$$
On average photon gas is polarised equally in $x,y,z$:
$$\langle\lvert p_{x} \rvert^2\rangle=\langle\lvert p_{y} \rvert^2\rangle=\langle\lvert p_{z} \rvert^2\rangle=\frac{1}{3}\langle\lvert p \rvert\rangle^2$$
so
$$R_{b\to a}=\frac{{\pi \lvert p_{ba} \rvert^2}}{3\varepsilon_{0}\hbar^2}\rho(\omega_{0})=B_{ab}\rho (\omega_{0}).$$
