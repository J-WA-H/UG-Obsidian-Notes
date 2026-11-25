Consider a slab of material with density $\rho$, cross-sectional area $A$ and depth $dr$ a distance $r$ from the centre of the body.
![[Pasted image 20241105183623.png]]
The net outwards force is 
$$\lim_{ dr \to 0 } [P(r)-P(r+dr)]A=-Adp.$$
The inwards gravitational force is given by
$$\frac{GM(<r)\rho Adr}{r^2}.$$
Equating these terms give the condition for hydrostatic equilibrium
$$\frac{dP}{dr}=-\frac{GM(<r)\rho}{r^2}.$$
Taking the boundary conditions that at the centre of the planet, $P(0)=P_{c}$ and at the surface $P(R_{p})=0$.
Using $M=\frac{4}{3}\pi r^3\rho$, we can integrate hydrostatic equilibrium to find the central pressure.
$$\int_{P_{c}}^0dP=-\frac{4}{3}\pi G\rho^2\int_{0}^{R_{p}}rdr$$
$$\implies P_{c}=\frac{2}{3}\pi G\rho^2R_{p}^2.$$
