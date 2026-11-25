Consider a set of $N$ spins
![[Pasted image 20250206123526.png]]
There are two contributions to the [[Domain Walls]] energy:
- [Exchange energy](Exchange%20Interaction.md) trying to align the spins
- [[Magnetocrystalline anisotropy]] energy density trying to keeps the spins aligned with the easy axis.

For the exchange energy, $E=-2J_{ij}\underline{S}_{i}\cdot \underline{S}_{j}$.
The energy due to perfect spin alignment is $E_{0}=-2NJ_{ex}S^2$.
Due to a misalignment of $\Delta\theta$, $E_{1}=-2NJ_{ex}S^2\cos\Delta\theta$.
Difference in these energies is given by
$$\Delta E=E_{1}-E_{0}=2NJ_{ex}S^2[1-\cos\Delta\theta].$$
Assuming a small $\Delta\theta$, $\cos\Delta\theta=1-\frac{\Delta\theta^2}{2}$
$$\therefore \Delta E=NJ_{ex}S^2\Delta\theta^2.$$
As $N\Delta\theta=\pi$,
$$\Delta E=\frac{J_{ex}}{N}(\pi S)^2.$$
As the domain wall is a 2D plane, the energy per unit area, $\sigma_{1}$, needs to be considered.
![[Pasted image 20250206124037.png]]
The number of spins per unit area is $\frac{1}{a^2}$, as each spin in the corner contributes $\frac{1}{4}$ of itself to the unit cell.
$$\sigma_{1}=\frac{\Delta E}{a^2}=\frac{J_{ex}}{N}\left( \frac{\pi S}{a} \right)^2.$$
The exchange energy tries to keep spins aligned so it tries to increase $N$ to minimise $\sigma_{1}$.

For the magnetocrystalline anisotropy energy density, the energy per unit volume is given by
$$\Delta\varepsilon=\sum_{i-0}^{n}k\sin^2(i\Delta\theta).$$
For small $\Delta\theta$, $\Delta\theta\to d\theta$
$$\implies\Delta\varepsilon=\frac{1}{\Delta\theta}\int_{0}^{\pi}k\sin^2\theta d\theta=\frac{Nk}{\pi}\int_{0}^{\pi}\sin^2\theta d\theta=\frac{Nk}{2}.$$
For the energy per unit area, $\sigma_{2}$,
$$\sigma_{2}=\frac{Nka}{2}.$$
Here the domain wall energy increases with $N$ so it tries to keep the domain small.

This shows $\sigma_{1},\sigma_{2}$ work against each other.
The total domain energy is hence given by
$$\sigma=\sigma_{1}+\sigma_{2}=\frac{J_{ex}}{N}\left( \frac{\pi S}{a} \right)^2+\frac{Nka}{2}.$$
To minimise energy, $\frac{d\sigma}{dN}=0$, solving for which gives
$$N=\pi S\sqrt{ \frac{2J_{ex}}{ka^3} };\;\sigma=\pi S\sqrt{ \frac{2J_{ex}k}{a} }.$$
Domains give rise to a hysteresis loop which describes magnetisation in terms of $M$ and $H$:
![[Pasted image 20250206144332.png]]
At point 1, the material is described by the domains
![[Pasted image 20250206145259.png]]
Applying an $H$ field increases the magnetisation to the saturation magnetisation at point 2, where the material has one uniform $M$,
![[Pasted image 20250206145557.png]]
Taking the $H$ field back to zero, the magnetisation doesn't drop straight to zero, but to $M_{r}$, the remnant magnetisation. This is not a reversible process.

Applying the an $H$ field in the opposite direction magnetises the material to $-M_{s}$, between which $M=0$ at the coercive field $H_{c}$. At $-M_{s}$, removing the $H$ field brings $M$ to $-M_{r}$, then applying an $H$ field in the original direction takes $M$ back to $M_{s}$, where the cycle continues. 

This is a hysteresis loop.