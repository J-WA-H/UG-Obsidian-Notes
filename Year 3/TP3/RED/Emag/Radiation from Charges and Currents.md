The energy transported by the fields per unit of time and area is called the Poynting vector
$$\underline{S}=\frac{1}{\mu_{0}}(\underline{E}\times \underline{B}).$$
Total power emitted is obtained by computing the integral of the flux of $\underline{B}$ through a sphere surrounding the source:
$$P(\underline{r})=\oint \underline{S}\cdot d\underline{a}=\frac{1}{\mu_{0}}\oint \underline{S}\cdot d\underline{a}.$$
The total power radiated to infinity is given by
$$P_{rad}=\lim_{ r \to \infty } P(\underline{r}).$$
For the static case, $\underline{E}$, $\underline{B}$ decreases as $\frac{1}{r^2}$, so $\underline{S}$ decreases with $1/r^4$, so static sources do not radiate.

![[Pasted image 20241109122831.png]]
Consider a dipole where charge is driven back and fourth given by $q(t)=q_{0}\cos(\omega t)$. This gives a dipole moment of $p(t)=p_{0}\cos(\omega t)$ where $p_{0}=q_{0}d$.
Scalar potential:
$$\phi(\underline{r},t)=\frac{1}{4\pi\varepsilon_{0}}\int_{V} \frac{\rho(\underline{r}',t_{r})}{R}dV'$$
$$=\frac{1}{4\pi\varepsilon_{0}}\left[ \frac{q_{0}\cos\left[ \omega\left( t-\frac{R_{+}}{c} \right) \right]}{R_{+}}-\frac{q_{0}\cos\left[ \omega\left( t-\frac{R_{-}}{c} \right) \right]}{R_{-}}\right]$$
$$\underline{R}_{+}=\underline{r}-\left( \frac{d}{z} \right)\underline{\hat{z}}\implies \lvert R_{+} \rvert =\sqrt{ r^2+\left( \frac{d}{2} \right)^2-dr\cos \theta }$$
$$\underline{R}_{-}=\underline{r}+\left( \frac{d}{z} \right)\underline{\hat{z}}\implies \lvert R_{-} \rvert=\sqrt{ r^2-\left( \frac{d}{2} \right)^2+dr\cos \theta } $$This can be simplified using some approximations:
1. $d\ll r$
	$$R_{\pm}=\sqrt{ r^2+\left( \frac{d}{2} \right)^2\mp dr\cos \theta }=r\sqrt{ 1+\left( \frac{d}{2r} \right)^2 \mp \frac{d}{r}\cos \theta}$$
	$$\approx r\left( 1\mp \frac{d}{2r}\cos \theta+\mathcal{O}\left( \left( \frac{d}{r} \right)^2 \right) \right).$$
	$$\frac{1}{R_{\pm}}\approx \frac{1}{r}\left( 1\pm \frac{d}{2r}+\mathcal{O}\left( \left( \frac{d}{2r}\cos \theta \right)^2 \right) \right).$$
	Rewrite some terms
	$$\cos \left[ \omega\left( t-\frac{R_{\pm}}{c} \right) \right]=\cos\left[ \omega\left( t-\frac{r}{c}\left( 1\mp \frac{d}{2r}\cos \theta \right) \right) \right]=\cos\left[ \omega\left( t-\frac{r}{c} \right)\pm \frac{\omega d}{2c}\cos \theta \right]$$
	$$=\cos\left[ \omega\left( t-\frac{r}{c} \right) \right]\cos\left[ \frac{\omega d}{2c}\cos \theta \right]\mp \sin\left[ \omega\left( t-\frac{r}{c} \right) \right]\sin \left[ \frac{\omega d}{2c}\cos \theta \right].$$
2. Perfect dipole limit: $d\ll \frac{c}{\omega}$.
	The oscillation length $\lambda=\frac{2\pi c}{\omega}\implies \frac{\omega}{c}d=d \frac{2\pi}{\lambda}\ll{1}$.
	$$\cos x\approx 1$$
		$$\sin x\approx x$$
	This gives
	$$\cos\left( \frac{\omega d}{2c}\cos \theta \right)\approx 1$$
	$$\sin\left( \frac{\omega d}{2c}\cos \theta \right)\approx \frac{\omega d}{2c}\cos \theta$$
	so we get
	$$\cos\left[ \omega\left( t-\frac{R_{\pm}}{c} \right) \right]\approx \cos\left[ \omega\left( t-\frac{r}{c} \right) \right]\mp \sin\left[ \omega \left( t-\frac{r}{c} \right) \right] \frac{\omega d}{2c}\cos \theta.$$
This gives a scalar potential
$$\phi=\frac{1}{4\pi\varepsilon_{0}}\left( \frac{q_{0}}{r}\left[ \cos\left[ \omega\left( t-\frac{r}{c} \right) \right]+\frac{\omega d}{2c}\cos \theta \sin\left[ \omega \left( t-\frac{r}{c} \right) \right] \right] \right)\left( 1-\frac{d}{r}\cos \theta \right)-\text{other stuff}$$
which simplifies to
$$\phi=\frac{1}{4\pi\varepsilon_{0}}\left[ \frac{q_{0}}{r}d\cos \theta \cos\left( \omega\left( t-\frac{r}{c} \right) \right)-\frac{\omega d}{c}\cos \theta \frac{q_{0}}{r}\sin\left( \omega\left( t-\frac{r}{c} \right) \right) \right].$$
$$=\left( \frac{p_{0}}{4\pi \varepsilon_{0}} \right)\left( \frac{\cos\theta}{r} \right)\left( \frac{\cos\left( \omega\left( t-\frac{r}{c} \right) \right)}{r} -\frac{\omega}{c}\sin\left( \omega\left( t-\frac{r}{c} \right) \right)\right).$$
3. Radiation limit: As $r\to\infty$, $\frac{1}{r^2}$ terms disappear
This gives the scalar potential
$$\phi \approx -\frac{p_{0}\omega}{4\pi\varepsilon_{0}c}\left( \frac{\cos \theta}{r} \right)\sin\left( \omega\left( t-\frac{r}{c} \right) \right).$$
Using the same process for the vector potential, where
$$\underline{j}=\frac{dq}{dt}\underline{\hat{z}}=-q_{0}\omega \sin(\omega t)\underline{\hat{z}}$$
with the same 3 approximations we get
$$\underline{A}(\underline{r},t)=-\frac{q_{0}\omega \mu_{0}}{4\pi r}\sin\left( \omega\left( t-\frac{r}{c} \right) \right)d\underline{\hat{z}}.$$
We can use these potentials to find the [E and B fields](Vector%20and%20Scalar%20Potentials.md), which gives
$$\underline{E}=-\frac{p_{0}\omega^2\mu_{0}}{4\pi r}\sin \theta \cos\left( \omega\left( t-\frac{r}{c} \right) \right)\underline{\hat{\theta}}$$
$$\underline{B}=-\frac{p_{0}\omega \mu_{0}}{4\pi r}\sin \theta\left( \frac{\omega}{c} \right)\cos\left( \omega\left( t-\frac{r}{c} \right) \right)\underline{\hat{\phi}}.$$
We can now find the Poynting vector
$$\underline{S}=\frac{1}{\mu_{0}}(\underline{E}\times \underline{B})=\frac{\mu_{0}}{c}\left( \frac{p_{0}\omega^2}{4\pi r}\sin \theta \cos\left( \omega\left( t-\frac{r}{c} \right) \right) \right)^2\underline{\hat{r}}$$
and the energy emitted over time is
$$\langle S\rangle=\frac{\mu_{0}}{c}\left( \frac{p_{0}\omega^2}{4\pi} \right)^2 \frac{\sin^2\theta}{2r^2}\underline{\hat{r}}.$$
![[Pasted image 20241112193336.png]]
Power radiated is given by
$$\langle P\rangle=\int\langle S\rangle da=\int \frac{\mu_{0}p_{0}^2\omega^4}{32\pi^2c} \frac{\sin^2\theta}{r^2}r^2\sin \theta d\theta d\phi$$
$$=\frac{\mu_{0}p_{0}^2\omega^4}{32\pi^2c}\int \sin^3\theta d\theta d\phi$$
$$\langle P\rangle=\frac{\mu_{0}p_{0}^2\omega^4}{12\pi c}.$$
