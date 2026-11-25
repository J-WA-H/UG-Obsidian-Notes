As the [[Rutherford experiment]] shows most of the atom is concentrated into a small nucleus, it can be treated as a point mass - with the potential generated being Coulomb's potential.
![[Pasted image 20241123104607.png]]
From the [[Coulomb Gauge]], the potential can be found by solving Laplace's equation which gives
$$H_{int}=\frac{Z_{1}Z_{2}e^2}{4\pi\varepsilon_{0}}\int d^3y \frac{f(y)}{\lvert \underline{x}-\underline{y} \rvert }$$
where $f(y)$ is the probability density of the proton.
Propagating this change to the cross section we have the square of a more complicated Fourier Transform. One can still factorise this change as
$$\int d^3xd^3y \frac{e^{i\underline{q}\cdot \underline{x}}f(y)}{\lvert \underline{x}-\underline{y} \rvert }=\int d^3z\int d^3y \frac{e^{iq(z+y)}f(y)}{\lvert \underline{z} \rvert }=\left[ \int d^3z \frac{e^{iqz}}{\lvert \underline{z} \rvert } \right]\left[ \int d^3y e^{iqy}f(y) \right]$$
which allows us to write 
$$\bra{p'}H_{int}\ket{p}=\frac{Z_{He}Z_{Au}e^2}{2\varepsilon_{0}} \frac{\mathcal{F}(q^2)}{q^2}$$
Hence we get a cross-section of
$$\frac{d\sigma}{d\Omega}=\lvert \mathcal{F}(q^2) \rvert^2\left( \frac{d\sigma}{d\Omega} \right)_{Ruth}$$
where $\mathcal{F}(q^2)$ is the form factor, given by
$$\mathcal{F}(q^2)=\int d^3x e^{i\underline{q}\cdot \underline{x}}f(\underline{x}).$$
To consider what a nucleus could be like, consider a spherical uniform distribution that ends at $r=R$
$$f_{Sph}(y)=\frac{3}{4\pi R^3}\begin{cases}
1 & r<R \\
0 & r>R
\end{cases}$$

which gives
$$\mathcal{F}(q^2)=\frac{3}{4\pi R^3}\int_{0}^R r^2dr(2\pi) \frac{{e^{iqr}-e^{-iqr}}}{iqr}=\frac{3}{(qR)^2}\left( \frac{\sin(qR)}{qR}-\cos(qR) \right).$$
This form factor can be analysed to give the features of finite size targets.
- In the low energy limit, $qR\ll{1}$, we do not have enough energy to resolve the size of the nucleus and it is effectively point-like, as $\mathcal{F}(q^2)\to 1$, which recovers Rutherford's cross section.
- In the high momentum regime, there will be an angle $\theta$ where interference causes the cross-section to approximately cancel, we can find the first of these values numerically
	$$\frac{\sin(q_{0}R)}{q_{0}R}-\cos(q_{0}R)\to 0;\; q_{0}R=2p \sin\left( \frac{\theta_{0}}{2} \right)R\approx{4}.493.$$
	Given that the momentum of the incoming particles and the first angle of cancellation $\theta_{9}$ we can determine $R$.

When we increase enough of the projectiles momentum, a diffraction like pattern will appear in our distribution in scattering angle. 