Galaxy clusters are the most massive gravitationally bound objects in the universe, detached from the [[Hubble Flow]] as they are so massive.

There are hundreds to thousands of galaxies in a cluster in a radius of a few $Mpc$.

Evidence for dark matter can be given by measuring the mass of galaxy clusters.

Method 1: Virial theorem.
The virial theorem gives a relation between kinetic and potential energy that must be satisfied for a system to be stable.
$$2\langle T \rangle =\langle V \rangle .$$
First consider kinetic energy,
$$\langle T \rangle =\frac{1}{2}\sum_{i=1}^{N}m_{i}v_{i}^2$$
Assume all galaxies have the same mass
$$\langle T \rangle =\frac{1}{2}m\sum_{i=1}^{N}v_{i}^{2}=\frac{N}{2}m \frac{1}{N}\sum_{i=1}^{N}v_{i}^2.$$
Using the dispersion relation
$$\sigma_{disp}=\sqrt{ \frac{1}N\sum_{i=1}^{N}v_{i}^2 },$$
$$\langle T \rangle =\frac{1}{2}Nm\sigma_{disp}^2=\frac{1}{2}Nm 3\sigma_{los}^2.$$
This uses the line-of-sight velocity, which is multiplied by 3 as due to isotropy assume velocity disperses the same in all 3 dimensions - which means we only need to measure 1, the line of sight velocity.

Potential energy:
$$\langle V \rangle =\sum_{i=1}^{N}\sum_{j>i}^{N} \frac{Gm_{i}m_{j}}{|\underline{r}_{i}-\underline{r}_{j}|}.$$
Assume all galaxies have the same mass,
$$\langle V \rangle =Gm^2N_{pair} \frac{1}{N_{pair}} \sum_{i=1}^{N}\sum_{j>i}^{N} \frac{1}{|\underline{r}_{i}-\underline{r}_{j}|}.$$
The number of pairs is given by
$$N_{pair} = \frac{N(N-1)}{2}.$$
The sum is the expectation of $\frac{1}{|\underline{r}_{i}-\underline{r}_{j}|}$.
$$\langle V \rangle =\frac{N(N-1)}{2}Gm^2\left\langle  \frac{1}{|\underline{r}_{i}-\underline{r}_{j}|}  \right\rangle \approx N(N-1) \frac{Gm^2}{R}\approx N^2 \frac{Gm^2}{R}$$
for large $N\gg 1$ where $R$ is the radius of the cluster.
Apply virial theorem,
$$3Nm\sigma^2_{los}=N^2 \frac{Gm^2}{R}\implies m=\frac{3R\sigma_{los}^2}{NG}.$$
This can give the mass as the radius of the cluster, dispersion velocity and the number of galaxies in the cluster can be observed. This gives a rough estimate of the mass of the cluster - it gives the correct order of magnitude.

Method 2: [[Hydrostatic Equilibrium]]
Consider the volume element in a shell of a sphere,
![[Pasted image 20250225151612.png]]
the mass of this element is $m=\rho_{gas}(r)\Delta S\Delta r$.
The force pulling the element in is the gravitational force,
$$F_{in}=\frac{GM(<r)m}{r^2}=\frac{GM(<r)}{r^2}\rho_{gas}(r)\Delta S\Delta r.$$
The force pushing it out is the the gas pressure,
$$F_{out}=-\Delta P_{gas}\Delta S.$$
Evaluate the two expressions,
$$\frac{GM(<r)}{r^2}\rho_{gas}(r)\cancel{\Delta S}\Delta r=-\Delta P_{gas}\cancel{\Delta S}$$
$$\implies \frac{1}{\rho_{gas}} \frac{\Delta P_{gas}}{\Delta r}=-\frac{GM(<r)}{r^2}$$
Take $\Delta P_{gas}, \Delta r\to 0$,
$$\frac{1}{\rho_{gas}} \frac{dP_{gas}}{dr} =-\frac{GM(<r)}{r^2}$$
For an ideal gas,
$$P_{gas}=nk_{B}T=\frac{\rho_{gas}}{\mu m_{p}}k_{B}T$$
Consider a hydrogen plasma,
$$\mu m_{p}=\frac{{Nm_{p}+N\cancelto{0}{m_{e}}}}{2}=\frac{1}{2}m_{p}.$$
This is an isothermal gas so
$$-\frac{GM(<r)}{r^1}=\frac{k_{B}T}{\mu m_{p}} \frac{{d\ln \rho_{gas}}}{d\ln r}$$
$$M(<r)=\frac{2k_{B}TR}{G\mu m_{p}}.$$
Method 3: Gravitational lensing
Dark matter strongly lenses light from distant galaxies. We observe several images of a galaxy - this is strong lensing.
![[Pasted image 20250225152949.png]]

Weak lensing only distorts the image of the target galaxy.
![[Pasted image 20250225153020.png]]

Consider one cluster with undetermined mass. We observe both strong and weak lensing. Mass reconstructed from lensing agrees well with other observations. 
Consider a bullet cluster - where two galaxy clusters collide. As dark matter doesn't interact with anything, it is unaffected by the collision. This is the most direct evidence for dark matter.
