It has been shown that [[Spin Waves]] case the difference between experimental and theoretical values for the magnetisation.
As a [magnon](Magnons.md) represents a spin flip, this change in magnetisation is proportional to the number of magnons, $\Delta M\propto n_{m}(T)$.

From statistical mechanics the number of magnons can be calculated using
$$n_{m}=\int_{0}^{\infty}f_{BE}(E)g_{m}(E)dE.$$
The [[Bose-Einstein Distribution]] was used as magnons are bosons.

Consider the magnon energy
$$E=4J_{ex}S[1-\cos(qa)].$$
![[Pasted image 20250206113754.png]]
Near $T=0\text{ K}$, $E\to 0$ so $q\to 0$. Using the small angle approximation gives $\cos(qa)=1-\frac{(qa)^2}{2}$. This gives
$$E=2J_{ex}Sa^2q^2\propto q^2.$$
This is like [[Free-Electron Theory]], where $E\propto k^2$.

As this is analogous to free-electron theory, the density of states for magnons is $g_{m}(E)\propto \sqrt{ E }dE$.
This gives
$$n_{m}\propto \int_{0}^{\infty} \frac{1}{\exp\left( \frac{{E-\mu}}{k_{B}T} \right)-1}\sqrt{ E }dE=\int_{0}^{\infty} \frac{\sqrt{ E }}{\exp\left( \frac{E}{k_{B}T} \right)-1}dE.$$The chemical potential is 0 as the number of particles are not conserved.
Evaluating the integral gives
$$n_{m}\propto T^{3/2}.$$
This is Bloch's $T^{3/2}$ law.