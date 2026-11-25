If the wave speed were constant throughout Earth, then the quickest and shortest routes would coincide and the travel time from source to observer would be
$$T=2 \frac{r_{0}}{V}\sin\left( \frac{\theta}{2} \right).$$
![[Pasted image 20241112202528.png]]

As S-waves cannot travel through liquid, we know the Earth's outer core is liquid.

We can find $\rho(r)$ from the [speeds](Material%20Properties.md) $v_p$ and $v_s$:
$$\frac{d\rho}{dr}=\frac{d\rho}{dP}\times \frac{dP}{dr}$$
The first term is $\rho/\kappa$ from the bulk modulus and the second term is [[Hydrostatic Equilibrium]].
$$\kappa=v_{p}^2-\frac{4}{3}v_{s}^2$$
$$\therefore \frac{d\rho}{dr}=-\frac{G\rho}{\left( v_{p}^2-\frac{4}{3}v_{s}^2 \right)r^2}\int_{0}^r 4\pi r'^2\rho dr'.$$
Extrapolating densities to zero and using the [Murnaghan bulk modulus](Finding%20Density%20Profile.md) we get
$$\frac{\rho}{\rho_{0}}=\left( 1+\frac{B}{\kappa}P \right)^{1/B}.$$
