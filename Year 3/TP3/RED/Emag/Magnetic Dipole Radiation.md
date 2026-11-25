Now consider radiation emitted from a magnetic dipole![[Pasted image 20241116175931.png]]
As this is a current loop, there is no net charge so $\rho=0$ so $\phi=0$ in the [[Lorenz Gauge]].

A wire loop with alternating current $I(t)=I_{0}\cos(\omega t)$ produces a magnetic dipole
$$\underline{m}(t)=\pi b^2I(t)\underline{\hat{z}}=\pi b^2I_{0}\cos(\omega t)\underline{\hat{z}}.$$
This yields a current density of $$\underline{j}=I_{0}\cos (\omega t)\underline{\hat{z}}.$$
We can use this to calculate the vector potential
$$\underline{A}(\underline{r},t)=\frac{\mu_{0}}{4\pi}\int_{V} \frac{\underline{j}(\underline{r}',t_{r})}{R}dV=\frac{\mu_{0}}{4\pi}\int \frac{I_{0}\cos(\omega t)}{R}d\underline{l}'.$$
The length element $d\underline{l}'$ can be expressed in polar coordinates as
$$d\underline{l}'=dl'\underline{\hat{l}}+rd\theta'\underline{\hat{\theta}}+r\sin \theta d\phi'\underline{\hat{\phi}}.$$
$\underline{\hat{l}}$ points in the radial direction, orthogonal to $d\underline{l'}$ so the radial component is zero. The current loop is also in a constant plane so $d\theta'=0$, leaving the only azimuthal component.
$$\underline{A}(\underline{r},t)=\frac{\mu_{0}}{4\pi}b^2I_{0}\underline{\hat{\phi}}\int \frac{\cos\left( \omega\left( t-\frac{R}{c} \right) \right)}{R}\cos \phi'd\phi'.$$
The $\sin \theta$ term goes to one as we set $\theta=\frac{\pi}{2}$ and the $\cos \phi'$ term comes from the projection of $\phi'$ onto $\phi$.
$$R=\lvert \underline{r}-\underline{b} \rvert=\sqrt{ r^2+b^2+2rb\sin \theta \cos \phi' }.$$
1. $b\ll r$
	$$R\approx r\left( 1-\frac{b}{r}\sin\theta \cos \phi'+\mathcal{O}\left( \frac{b^2}{r^2} \right)\right).$$
	$$\frac{1}{R}\approx \frac{1}{r}\left( 1+\frac{b}{r}\sin \theta \cos \phi' +\mathcal{O}\left( \frac{b^2}{r^2} \right)\right).$$
	$$\cos\left( \omega\left( t-\frac{R}{c} \right) \right)=\cos\left( \omega\left( t-\frac{r}{c} \right)+\frac{\omega b}{c}\sin \theta \cos \phi' \right)$$
	$$=\cos\left( \omega\left( t-\frac{r}{c} \right) \right)\cos\left( \frac{\omega b}{c}\sin \theta \cos \phi' \right)-\sin\left( \omega\left( t-\frac{r}{c} \right) \right)\sin\left( \frac{\omega b}{c}\sin \theta \cos \phi' \right).$$
2. $b\ll \frac{c}{\omega}$
	$$\cos\left( \omega\left( t-\frac{R}{c} \right) \right)\approx \cos\left( \omega\left( t-\frac{r}{c} \right) \right)-\sin\left( \omega\left( t-\frac{r}{c} \right) \right) \frac{\omega b}{c}\sin \theta \cos \phi'$$
	$$\underline{A}=\frac{\mu_{0}bI_{0}}{4\pi}\underline{\hat{\phi}}\int_{0}^{2\pi} d\phi'\left[ \cos\left( \omega\left( t-\frac{r}{c} \right) \right)-\frac{\omega b}{c}\sin \theta \cos \phi'\sin\left( \omega\left( t-\frac{r}{c} \right) \right) \right] \frac{1}{r}\left[ 1+\frac{b}{r}\sin \theta \cos \phi' \right]\cos \phi'.$$
	Using $$\int_{0}^{\pi}\cos \phi d\phi=0;\;\int_{0}^{2\pi}\cos^2\phi d\phi=\pi$$
	$$\underline{A}(\underline{r},t)=\frac{\mu_{0}bI_{0}}{4r}\left[ \frac{b}{r}\sin \theta \cos\left( \omega\left( t-\frac{r}{c} \right) \right)-\frac{\omega b}{c}\sin \theta \sin\left( \omega\left( t-\frac{r}{c} \right) \right) \right]\underline{\hat{\phi}}.$$
3. Radiation limit (ignore $r^2$ terms):
	$$\underline{A}(\underline{r},t)=-\frac{\mu_{0}b^2I_{0}\omega}{4rc}\sin \theta \sin\left( \omega\left( t-\frac{r}{c} \right) \right)\underline{\hat{\phi}}.$$
We can now use the vector potential to find the $\underline{E}$ and $\underline{B}$ fields in the radiation limit.
$$\underline{B}=\underline{\nabla}\times \underline{A}=-\frac{\mu_{0}m_{0}\omega^2}{4\pi rc^2}\sin \theta \cos\left( \omega\left( t-\frac{r}{c} \right) \right)\underline{\hat{\theta}}.$$
$$\underline{E}=-\frac{\partial\underline{A}}{\partial t}=-\frac{\mu_{0}m_{0}}{4\pi c}\omega^2\left( \frac{\sin\theta}{r} \right)\cos\left( \omega\left( t-\frac{r}{c} \right) \right)\underline{\hat{\phi}}.$$
We can now calculate the Poynting vector:
$$\underline{S}=\frac{1}{\mu_{0}}(\underline{E}\times \underline{B})=\frac{\mu_{0}m_{0}^2}{(4\pi)^2} \frac{\omega^4}{c^3}\left( \frac{\sin\theta}{r} \right)^2\cos^2\left( \omega\left( t-\frac{r}{c} \right) \right)\underline{\hat{r}}.$$
Averaged over time, we get
$$\langle S\rangle=\frac{\mu_{0}m_{0}^2\omega^4}{32\pi^2c^3}\left( \frac{\sin\theta}{r} \right)^2\underline{\hat{r}}.$$
The radiation emitted is given by
$$P^{mag}_{rad}=\int\langle S\rangle da=\frac{\mu_{0}m_{0}^2\omega^4}{32\pi^2c^3}\int \frac{\sin^2\theta}{r^2}r^2\sin \theta d\theta d\phi$$
$$=\frac{\mu_{0}m_{0}^2\omega^4}{12\pi c^3}.$$
Comparing this to the radiation emitted by an [electric dipole](Radiation%20from%20Charges%20and%20Currents.md)
$$P_{rad}^{elec}=\frac{\mu_{0}p_{0}^2\omega^4}{12\pi c}.$$
$$\frac{P_{rad}^{mag}}{P_{rad}^{elec}}=\frac{m_{0}^2}{p_{0}^2c_{6}2}=\left( \frac{q_{0}\omega \pi b^2}{q_{0}\pi bc} \right)^2=\left( \frac{\omega b}{c} \right)^2\ll 1$$
This shows that the radiation emitted by an electric dipole is far larger than the radiation emitted by a magnetic dipole.