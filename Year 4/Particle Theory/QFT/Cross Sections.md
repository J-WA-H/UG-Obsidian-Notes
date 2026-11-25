Cross sections are the physical observables obtained from the probabilities for each given scattering process to occur.

The [[Scattering Amplitudes]] $\mathcal{M}_{i\to f}$ give probability densities $|\mathcal{M}_{i\to f}|^2$. This gives the probability
$$P=\int d\phi_{n}|\mathcal{M}_{i\to f}|^2\tag{12.1} $$
where we are integrating over the Lorentz-invariant of the final state particles.
![[Pasted image 20251111165325.png]]
The cross section is the effective area of the particle which is given by the product of the flux and the probability.

$d\phi_{n}$ is the integrand of an n-particle Lorentz invariant phase space, given by, for $2\to n$ scattering
$$\int d\phi_{n}=\left( \int \prod_{f=1}^{n} \frac{d^3p_{f}}{(2\pi)^32E_{p_{f}}} \right)(2\pi)^4\delta^{(4)}\left( k_{1}+k_{2}-\sum_{f=1}^{n}p_{f} \right)\tag{12.2}. $$
The flux factor is given by
$$\text{flux}\equiv \sqrt{ (k_{1}^{\mu}k_{2\mu})^2-m_{1}^2m_{2}^2 }\tag{12.3} $$which is defined in this way as it has the dimensions of $\frac{1}{\text{Area}}$.
This gives the total cross section of
$$\sigma_{2\to n}=\frac{1}{\sqrt{ (k_{1}^{\mu}k_{2\mu})^2-m_{1}^2m_{2}^2 }}\int d\phi_{n}|\mathcal{M}_{2\to n}|^2\tag{12.4}. $$
Sometimes it is more convenient to write this as the differential cross section,
$$d\sigma_{2\to n}=\frac{1}{\sqrt{ (k_{1}^{\mu}k_{2\mu})^2-m_{1}^2m_{2}^2 }}d\phi_{n}|\mathcal{M}_{2\to n}|\tag{12.5} $$
Flux can also be written as
$$\frac{1}{\text{flux}}\equiv \frac{1}{E_{1}E_{2}|v_{1}-v_{2}|}\tag{12.6} $$where $E_{1},E_{2}$ are the energy of the incoming particles and $|v_{1}-v_{2}|$ is the magnitude of the relative velocity.

In the minimal case, $2\to 2$ scattering. In the centre of mass frame,
![[Pasted image 20251115152114.png]]
where $E_{i}=\sqrt{ |\vec{p}_{i}|^2+m_{i}^2 }$. In this frame the integrand simplifies to
$$\int d\phi_{2}=\int \frac{dp_{1}p_{1}^2d\Omega}{(2\pi)^32E_{1}2E_{2}}(2\pi)\delta(E_{COM}-E_{1}-E_{2}).\tag{12.7} $$
From azimuthal symmetry, this simplifies to
$$\int d\phi_{2}=\int d\cos \theta \frac{1}{16\pi} \frac{2|\vec{p}_{1}|}{E_{COM}}.\tag{12.8} $$
This gives
$$d\sigma_{2\to 2}= \frac{d\cos{\theta}}{16\pi} \frac{2|\vec{p}_{1}|}{E_{COM}} \frac{1}{\sqrt{ (k_{1}^{\mu}k_{2\mu})^2-m_{1}^2m_{2}^2 }}|\mathcal{M}_{2\to 2}|^2\tag{12.9} $$$$\implies \left( \frac{d\sigma}{d\Omega} \right)_{COM}= \frac{|\mathcal{M}_{2\to 2}|}{64\pi^2E_{COM}^2}\tag{12.10} $$
iff $\forall$ particles $i,m_{i}=0$.

For $m_{i}\neq 0$, 
$$\left( \frac{d\sigma}{d\Omega} \right)_{COM}= \frac{1}{2E_{1}E_{2}|v_{1}-v_{2}|} \frac{|\vec{p}_{1}|}{(2\pi)^24E_{COM}^2}|\mathcal{M}_{2\to 2}|^2\tag{12.11} .$$
For a $\frac{\lambda \phi^4}{4!}$ interacting field theory, to $\mathcal{O}(\lambda^{1})$, $\mathcal{M}_{2\to 2}=-i\lambda$ so $|\mathcal{M}_{2\to 2}|^2=\lambda^2$.