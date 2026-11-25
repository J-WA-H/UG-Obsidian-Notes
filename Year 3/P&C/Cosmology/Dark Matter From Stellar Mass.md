From observations there are a higher number of low luminosity stars.
![[Pasted image 20250225140244.png]]
The luminosity is given by $L$ and $\phi$ gives the number density.
This is the Schechter function: a power law for low luminosity and an exponential cut off on the other.

Stellar luminosity can be used to calculate the mass, using the mass-to-light ratio,
$$\frac{M}{L}=0.8 \frac{M_{\odot}}{L_{\odot}}.$$
Massive stars produce more light per unit mass, so the mean value of $\frac{M}{L}$ will depend on what fraction of stars are more or less massive.

The total universe matter content from stars is
$$\Omega_{star}\approx 2.3\times 10^{-3}.$$
Calculations of the density are inaccurate as there is a 10% uncertainty from the luminosity function determination and 20% uncertainty from the assumptions about the stellar mass distributions.

The total mass of the galaxy can be obtained by measuring the galaxies rotation curve. This is measured using redshift.
![[Pasted image 20250225143853.png]]
At the observer $O'$ near the galaxy, only [Doppler shift](Redshift.md) is observed,
$$z_{D}=\frac{v}{c}=\frac{\Delta\lambda}{\lambda}$$
$$\lambda_{1}=\lambda_{0}\left( 1-\frac{v}{c} \right);\;\lambda_{2}=\lambda_{0}\left( 1+\frac{v}{c} \right).$$
$\lambda_{1}$ is blue shifted and $\lambda_{2}$ is redshifted. 

To observer $O$, [[Hubble Flow]] also needs to be taken into account so we need both cosmological and Doppler shifts.
$$\lambda_{1}=\lambda_{0}\left( 1-\frac{v}{c} \right)(1+z)$$
$$\lambda_{2}=\lambda_{0}\left( 1+\frac{v}{c} \right)(1+z).$$
This gives
$$\Delta\lambda=2\lambda_{0} \frac{v}{c}(1+z).$$
This can be used to calculate rotational velocity $v$, as $\lambda_{0}$ and $z$ are known and $\Delta\lambda$ is measurable.
Using Newtonian mechanics this can be used to determine the mass - by equating gravitational and centripetal acceleration,
$$\frac{GM(<r)}{r^2}=\frac{v_{rot}^2}{r}\implies v_{rot}=\sqrt{ \frac{GM(<r)}{r} }.$$
This predicts a $r^{-1/2}$ dependence on $v_{rot}$, when in reality the rotation curve is flat.

This implies the existence of dark matter, which has density $\rho(r)\propto r^{-2}$, which gives
$$M=\int 4\pi r^2\rho(r)dr\propto r.$$
![[Pasted image 20250225145748.png]]
