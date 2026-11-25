Consider the magnitude of an object,
$$m(z)=5\log_{10}d_{L}(z)+b.$$
Taylor expand $d_{L}(z)=(1+z)S_{k}(r_{CM})$, assuming a flat universe
$$d_{L}=(1+z)r_{CM}(z).$$
Expand $r_{CM}(z)$,
$$r_{CM}(z)=r_{CM}(0)+z \frac{dr_{CM}(0)}{dz}+\frac{1}{2}z^2 \frac{d^2r_{CM}(0)}{dz^2}+\mathcal{O}(z^3).$$
$$r_{CM}(z)=c\int_{0}^{z} \frac{dz'}{H(z')}.$$
$$\therefore \frac{dr_{CM}}{dz}=\frac{c}{H(z)},\; \frac{d^2r_{CM}}{dz^2}=\frac{d}{dz}\left( \frac{c}{H(z)} \right)=-\frac{c}{H^2} \frac{dH}{dz}=-\frac{c}{H^2} \frac{{dH/dt}}{dz/dt}=-\frac{c}{H^2} \frac{{\left( \frac{\ddot{a}}{a} \right)-\left( \frac{\dot{a}}{a} \right)^2}}{-\frac{1}{a}H^2}$$
$$=\frac{ac}{H} \frac{{\left(\frac{\ddot{a}}{a}\right)-H^2}}{H^2}=-(1+q) \frac{ac}{H}.$$
Where $q$ is defined as the deceleration parameter,
$$q=-\frac{\ddot{a}/a}{(\dot{a}/a)^2}.$$
$$\implies r_{CM}=\frac{c}{H_{0}}z-\frac{1}{2}(1+q_{0}) \frac{c}{H_{0}}z^2+\mathcal{O}(z^3)$$
$$\therefore d_{L}=\frac{c}{H_{0}}\left[ z+\frac{1}{2}(1-q_{0})z^2 \right]+\mathcal{O}(z^3).$$
$q$ tells us if the expansion of the universe is accelerating or decelerating.

Substituting the [[Acceleration Equation]] into $q$ gives
$$q=-\frac{1}{H_{0}}\left[ -\frac{4\pi G}{3}\left( \rho_{M}+\frac{3P_{M}}{c^2} \right) +\frac{\Lambda c^2}{3}\right]=-\frac{1}{H^2}\left[ -\frac{4\pi G}{3}\rho_{M}+\frac{\Lambda c^2}{3} \right]=\frac{1}{2}\Omega_{M}(a)-\Omega_{\Lambda}(a).$$
