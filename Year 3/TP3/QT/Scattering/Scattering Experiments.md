There are two main ways to measure microscopic properties - photon emission/absorption and scattering of particles.

The scattering of particles gives information on the potential/forces present.

In scattering experiments we observe the particles scattered into a small solid angle $d\Omega$ at an angle theta.
![[Pasted image 20250118142718.png]]
There are two basic types of scattering, elastic and inelastic scattering.
Elastic scattering conserves the type of particle - the incoming and outgoing particles are the same, like the [[Rutherford experiment]].

Inelastic scattering is where the incoming and outgoing particles are different, like nuclear [[Fission]]. 

Looking at non-relativistic elastic scattering, the likelihood of an incoming particle being scattered in a given direction is given by
$$\frac{d\sigma}{d\Omega}=\frac{N}{F}.$$
$N$ is the number of particles scattered into a direction $\theta,\phi$ per unit time per unit solid angle, and $F$ is the incident flux, the number of particles per unit area per unit time incoming.

The total cross-section is given by integrating over the solid angle.
$$\sigma=\int d\Omega  \frac{d\sigma}{d\Omega}=\int_{0}^{2\pi}d\phi \int_{0}^{\pi}\sin \theta d\theta  \frac{d\sigma}{d\Omega}.$$
Using $\sin \theta d\theta=-d\cos \theta$,
$$\sigma=-\int_{0}^{2\pi}d\phi \int_{1}^{-1}d\cos \theta  \frac{d\sigma}{d\Omega}=\int_{0}^{2\pi}d\phi \int_{-1}^{1}d\cos \theta  \frac{d\sigma}{d\Omega}.$$
The total number of scattering events is given by
$$N=\left( \int Fdt \right)\sigma.$$
From dimensional analysis we get that the cross section has units of area.

For a general potential, the cross section is the effective area related to the range $\Omega$ strength of the potential.
