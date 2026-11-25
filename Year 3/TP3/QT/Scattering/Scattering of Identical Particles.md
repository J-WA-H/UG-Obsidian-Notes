For identical particles we need to consider what happens when we exchange identical particles.
For bosons, $\psi\to_{swap}\psi$ and for fermions $\psi\to_{swap}-\psi$.
In the centre of mass frame, $\underline{r}\to-\underline{r}$
![[Pasted image 20250131162750.png]]
Consider the symmetry with respect to $\theta,\phi\to(\pi-\theta,\pi+\phi)$.

Starting with the symmetric solution
$$\psi(\underline{r})+\psi(-\underline{r})=e^{i\underline{k}\cdot \underline{r}}+e^{-i\underline{k}\cdot \underline{r}}+(f(k,\theta,\phi)+f(k,\pi-\theta,\pi+\phi)) \frac{e^{ikr}}{r}.$$
Let $f_{T}(\theta,\phi)=f(\theta,\phi)+f(\pi-\theta,\pi+\phi)$.
For a central potential $f(\theta,\phi)=f(\theta)$.
This gives the [cross section](Scattering%20Amplitude.md) 
$$\frac{d\sigma}{d\Omega}=|f(\theta)+f(\pi-\theta)|^2.$$
The simplest case is Coulomb scattering where
$$f_{c}=-\frac{\gamma}{2k\sin^2\left( \frac{\theta}{2} \right)} \frac{\Gamma(1+i\gamma)}{\Gamma(1-i)}\exp\left[ -i\gamma \ln\left( \sin^2\left( \frac{\theta}{2} \right) \right) \right]$$
where $\Gamma$ is the gamma function
$$\Gamma(x)=\int_{0}^{\infty}t^{x-1}e^{-t}dt$$
and
$$\gamma=\frac{q_{1}q_{2}}{4\pi\varepsilon_{0}\hbar v}=\frac{U_{0}}{2k}.$$
The gamma function and the exponential are complex phases so they don't contribute anything to the cross section.
$$\frac{d\sigma}{d\Omega}=\left( \frac{\gamma}{2k} \right)^2\left[ \csc^4\left( \frac{\theta}{2} \right) +\sec^4\left( \frac{\theta}{2} \right)+2\csc^2\left( \frac{\theta}{2} \right)\sec^2\left( \frac{\theta}{2} \right)\cos\left( 2\gamma \ln\left( \tan\left( \frac{\theta}{2} \right) \right) \right)\right].$$
The $\csc^4$ and $\sec^4$ terms are the classical scattering case and the cross term is the quantum interference observed in experiment.

For identical spin-$\frac{1}{2}$ particles the wavefunctions have a spatial and spin part, $\psi=\psi_{spatial}\psi_{spin}$.
The spin is either antisymmetric, $S=0$ (singlet) or symmetric, $S=1$ (triplet).

The overall wavefunction must be antisymmetric, so the scattering amplitude for the singlet is symmetric and for the triplet is antisymmetric.
$$f_{s^{+}}(\theta)=f_{s}(\theta)+f_{s}(\pi-\theta)$$
$$f_{t^{-}}(\theta)=f_{t}(\theta)-f_{t}(\pi-\theta).$$
This gives the cross section
$$\frac{d\sigma_{s}}{d\Omega}=|f_{s}(\theta)+f_{s}(\pi-\theta)|^2$$
$$\frac{d\sigma_{t}}{d\Omega}=|f_{t}(\theta)-f_{t}(\pi-\theta)|^2.$$
In an unpolarised beam and target, there are 4 possible states, 1 singlet and 3 triplet, so the total cross section becomes
$$\frac{d\sigma}{d\Omega}=\frac{1}{4} \frac{d\sigma_{s}}{d\Omega}+\frac{3}{4} \frac{d\sigma_{t}}{d\Omega}.$$
For a spin independent interaction, $f_{s}(\theta)=f_{t}(\theta)$ so
$$\frac{d\sigma}{d\Omega}=|f(\theta)|^2+|f(\pi-\theta)|^2-\mathrm{Re}[f(\theta)f(\pi-\theta)].$$
The first two terms are the classical terms and the Real cross term is the interference part.
