We can describe metals for the free electron model.

![[Pasted image 20250117105635.png]]
This describes a metal as a lattice of positive core regions, consisting of the nucleus and innermost electrons, and a cloud of delocalised free electrons.

From statistical physics, classical systems are described by the [[Maxwell-Boltzmann Distribution]].
$$f_{MB}(E)\propto \exp\left( -\frac{E}{k_{B}T} \right)$$
![[Pasted image 20250117110117.png]]
However electrons are fermions so we use the [[Fermi-Dirac Distribution]]
$$f_{FD}(E)=\frac{1}{1+\exp\left( \frac{{E-\mu}}{k_{B}T} \right)}.$$
![[Pasted image 20250117110231.png]]
Quantum mechanics is essential for describing electronic structure.

For the free electron model, the space between nuclei are treated as a potential well, so $V(r)=0$, so to model electrons we have the Schrodinger equation
$$-\frac{\hbar^2}{2m}\nabla^2\psi(\underline{r})=E\psi(\underline{r})$$
which gives plane wave solutions, $\psi(\underline{r})=e^{i\underline{k}\cdot \underline{r}}$.
This wavefunction yields an energy of
$$E=\frac{\hbar^2k^2}{2m}.$$
The momentum is given by $p=\hbar k$, which can be used to define the de-Broglie wavelength
$$\lambda=\frac{h}{mv}.$$

To find the energy levels in a solid, we need to impose periodic boundary conditions. Consider a cubic solid of length $L$:
![[Pasted image 20250117111201.png]]
The wavefunction should be the same at both the shaded surfaces.
$$\psi(x,y,z)=\psi(x,y+L,z)$$
$$\cancel{e^{ik_{x}x}}e^{\cancel{ik_{y}y}}\cancel{e^{ik_{z}z}}=\cancel{e^{ik_{x}x}}e^{ik_{y}(\cancel{y}+L)}\cancel{e^{ik_{z}z}}$$
$$\implies e^{ik_{y}L}=1=e^{i(2\pi n)}$$
$$\implies k_{y}=\frac{2\pi n}{L},\;n\in \mathbb{Z}.$$
This shoes that the wavevector is quantised.

The distance between adjacent nuclei in k-space is hence given by $\frac{2\pi}{L}$, so the volume of a state is given by
$$V=\left( \frac{2\pi}{L} \right)^{3}.$$
The density of states fives the number of electronic states between $E$ and $E+dE$ per unit volume of the solid.
$$g(k)dk=\frac{4\pi k^2dk}{\left( \frac{2\pi}{L} \right)^{3}}\times 2.$$
The multiplication by 2 is due to the spin states of the electrons.
$$\implies g(k)dk=\left( \frac{k}{\pi} \right)^{2}dk.$$
Using $E=\frac{(\hbar k)^{2}}{2m}$ and $dE=\frac{\hbar^2}{m}kdk$ gives
$$g(E)dE=\frac{1}{2\pi^2}\left( \frac{2m}{\hbar^2} \right)^{3/2}\sqrt{ E }dE.$$
The Fermi surface is the surface in k-space that all states up to it are occupied.
![[Pasted image 20250117113434.png]]
All states up to the Fermi wavevector, $k_{F}$, are occupied. Consider $N$ electrons, 
$$N=\frac{\frac{4}{3}\pi k_{F}^{3}}{\left( \frac{2\pi}{L} \right)^3}\times 2$$
$$\implies \frac{N}{L^3}=\frac{1}{3\pi^2}k_{F}^{3}=n$$
This gives the relation between the Fermi-wavevector and electron density,
$$n=\frac{k_{F}^{3}}{3\pi^2}.$$
The Fermi wavevector can then give the Fermi energy and the Fermi velocity
$$E_{F}=\frac{(\hbar k_{F})^{2}}{2m}$$
$$v_{F}=\hbar \frac{k_{F}}{m}.$$
