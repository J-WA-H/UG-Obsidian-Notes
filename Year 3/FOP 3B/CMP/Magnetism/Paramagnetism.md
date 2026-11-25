The paramagnetic term of the [magnetic Hamiltonian](Angular%20Momentum%20in%20QM.md) is
$$\hat{H}_{para}=\gamma g_{J}\underline{B}\cdot \underline{J}.$$
We have $|\underline{J}|=\sqrt{ J(J+1) }\hbar^2$, $J_{z}=m_{z}\hbar$.
This describes paramagnets - materials where the spins are randomly arranged.
![[Pasted image 20250129182751.png]]
Langevin theory is the classical theory for paramagnets, a $J=\infty$ solid.
Consider a [[Larmor Procession]]:
![[Pasted image 20250129182909.png]]
The energy of this dipole processing at a constant angle $\theta$ is
$$E=-\underline{\mu}\cdot \underline{B}=-\mu B\cos \theta.$$
As this is a classical system, apply the [[Maxwell-Boltzmann Distribution]]:
$$f_{MB}\propto \exp\left[ -\frac{E}{k_{B}T} \right]=\exp\left[ \frac{\mu B}{k_{B}T}\cos \theta \right].$$
The average dipole moment along the $z$ axis is
$$\langle \mu_{z} \rangle =\frac{\int_{0}^{\pi}\mu\cos\theta e^{\mu B\cos \theta/k_{B}T}(2\pi \sin \theta)d\theta}{\int_{0}^{\pi}e^{\mu B\cos \theta/k_{B}T}(2\pi \sin \theta)d\theta}.$$
Let $x=\cos \theta$ and $y=\frac{\mu B}{k_{B}T}$
$$\frac{{\langle \mu_{z} \rangle}}{\mu}=\frac{\int_{-1}^{1}xe^{yx}dx}{\int_{-1}^{1}e^{yx}dx}=\coth(y)-\frac{1}{y}.$$
This is the Langevin function
$$L(y)=\coth(y)-\frac{1}{y}.$$
![[Pasted image 20250129184101.png]]
For weak B-fields, $y\to 0$, $\coth(y)\to \frac{y}{3}+\frac{1}{y}$
$$\therefore L(y)=\frac{y}{3}=\frac{\mu B}{3k_{B}T}.$$
Per unit volume gives the magnetisation
$$\frac{{n\langle \mu_{z} \rangle}}n{\mu}=\frac{M}{M_{s}}=\frac{\mu B}{3k_{B}T}$$
where $M_{s}$ is the saturation magnetisation and $n$ is the number of atoms per unit volume.

For weak paramagnetic solids:
$$\underline{B}=\mu_{0}(\underline{H}+\underline{M})\approx \mu_{0}\underline{H};\;\underline{M}=\chi \underline{H}.$$
$$\chi=\frac{M}{H}=\frac{\mu_{0}M}{B}.$$
Using the above expression for magnetisation we get the paramagnetic susceptibility as
$$\chi_{p}=\frac{\mu_{0}M_{s}\mu_{0}}{3k_{B}T}=\frac{n\mu_{0}\mu^2}{3k_{B}T}.$$
It can be seen that susceptibility is proportional to $\frac{1}{T}$, this is Curie's law
![[Pasted image 20250129185939.png]]
As magnetism is a quantum mechanical phenomenon, the susceptibility should be derived from quantum mechanics.
Consider a $J=\frac{1}{2}$ solid:
$$\underline{\mu}=-g_{J}\gamma \underline{J};\;\mu_{z}=-g_{J}\gamma J_{z}=-g_{J}(\gamma \hbar)m_{J}$$
As the [Bohr magneton](Magnetic%20Dipoles.md) is given by $\mu_{B}=\gamma \hbar$, this simplifies to
$$\mu_{z}=-g_{J}\mu_{B}m_{J}.$$
For this $J=\frac{1}{2}$ solid, the possible values of $m_J$ are $\pm \frac{1}{2}$ so this cancels with $g_{J}=2$, leaving
$$\mu_{z}=\pm \mu_{B}.$$
Now consider energy, with $\underline{B}$ aligned parallel to the $z$ axis.
$$E=-\underline{\mu}\cdot \underline{B}=-\mu_{z}B.$$
As this is in the dilute limit, the Maxwell Boltzmann distribution can be used,
$$f_{MB}\propto \exp\left[ \frac{\mu_{Z}B}{k_{B}T} \right].$$
$$\langle \mu_{z} \rangle =\frac{{\mu_{B}\exp\left[ \frac{\mu_{B}B}{k_{B}T} \right]-\mu_{B}\exp\left[ -\frac{\mu_{B}B}{k_{B}T} \right]}}{\exp\left[ \frac{\mu_{B}B}{k_{B}T} \right]+\exp\left[ \frac{\mu_{B}B}{k_{B}T} \right]}.$$
Using $y=\frac{\mu_{B}B}{k_{B}T}$,
$$\frac{{\langle \mu_{z} \rangle}}{\mu_{B}}=\frac{{e^{y}-e^{-y}}}{e^{y}+e^{-y}}=\tanh(y).$$
For weak B fields $y\to 0$, $\tanh(y)\to y$
$$\frac{M}{M_{s}}=\frac{{n\langle \mu_{z} \rangle }}{n\mu}=\frac{\mu_{B}B}{k_{B}T}.$$
For weak magnetic solids,
$$\chi_{p}=\frac{\mu_{0}M}{B}=\frac{n\mu_{0}\mu_{B}^2}{k_{B}T}.$$
This is of the same form as the classical susceptibility but a factor of 3 larger.

For an arbitrary $J$ and $y=\frac{g_{J}\mu_{B}JB}{k_{B}T}$,
$$\frac{M}{M_{s}}=B_{J}(y)$$
where $B_{J}(y)$ is the Brillouin function
$$B_{J}(y)=\frac{{2J+1}}{2J}\coth\left( \frac{{2J+1}}{2J}y \right)=\frac{1}{2J}\coth\left( \frac{y}{2J} \right).$$
This can be used to determine thermodynamic properties
![[Pasted image 20250129192950.png]]
![[Pasted image 20250129193005.png]]
![[Pasted image 20250129193025.png]]
This can be used in magnetic cooling
![[Pasted image 20250129193115.png]]
The steps include an isothermal step, where the B field is turned on, and an adiabatic magnetisation where the B field is turned off.
![[Pasted image 20250129193225.png]]
Repeating these steps gets to temperatures around $T\approx 10^{-3} \text{ K}$.
