We can use [hydrostatic equilibrium](Hydrostatic%20Equilibrium.md) to find a planets density profile. Differentiating hydrostatic equilibrium with respect to $r$, using $\frac{dM}{dr}=4\pi r^2\rho$, yields
$$\frac{d}{dr}\left( \frac{r^2}{G\rho} \frac{dP}{dr} \right)+4\pi r^2\rho=0.$$
To solve this equation we need the equation of state $P(\rho)$. 
The bulk modulus is given by$$\kappa=\rho\left( \frac{\partial P}{\partial \rho} \right)_{S}.$$
Empirically, $\kappa$ can be expressed as a Taylor series
$$\kappa=\kappa_{0}+BP+\mathcal{O}(P^2).$$
This gives a definition of the Murnaghan bulk modulus, $\kappa=\kappa_{0}+BP$, which fits well for pressures up to $10^{11}\text{ Pa}$.
Pressure only depends on density so
$$\frac{d\rho}{\rho}=\frac{dP}{\kappa_{0}+BP}.$$
Integrating this gives
$$P(\rho)=\frac{\kappa_{0}}{B}\left[ \left( \frac{\rho}{\rho_{0}} \right)^B-1 \right]$$
where $\rho_{0}$ is the density at $P=0$.

Plugging this into the ODE yields
$$\frac{1}{4\pi r^2\rho_{c}} \frac{d}{dr}\left( \frac{r^2}{G\rho} \frac{\kappa_{0}\rho^{B-1}}{\rho_{0}^B} \frac{d\rho}{dr} \right)+\frac{\rho}{\rho_{c}}=0.$$
We can rewrite $B=1+\frac{1}{n}$, $y^n=\frac{\rho}{\rho_{c}}$ and $x=\frac{r}{D}$ with $D=\left( \frac{n\rho_c^{1/(n-1)}\kappa_{0}}{4\pi G\rho_{0}^{1/(n+1)}} \right)$. This simplifies the ODE to
$$\frac{1}{x^2} \frac{d}{dx}\left( x^2 \frac{dy}{dx} \right)+y^n=0.$$
This is the Lame-Emden equation.
This equation can be solved with boundary conditions $y(0)=1$, $\frac{dy(0)}{dx}=0$.
![[Pasted image 20241105192620.png]]
The solutions show that for higher $n$, density decreases at a slower rate that for lower values of $n$.