[P and S-waves](Seismology.md) are low frequency waves with wavelengths of a few kilometres and speed up to about $10\text{ km s}^{-1}$.
The speed can be written as
$$v=\sqrt{ \frac{{\text{Elastic Modulus}}}{\text{density}} }.$$
Young's Modulus
$$q=\frac{{\text{Longitudinal stress}}}{\text{Longitudinal strain}}.$$
Poisson's ratio
$$\nu=-\frac{{\text{Lateral strain}}}{\text{Longitudinal strain}}.$$
Longitudinal strain is the strain in the longitudinal direction and lateral strain is the strain the the transverse direction.

Shear modulus
$$\mu=\frac{{\text{Shear stress}}}{\text{Shear strain}}=\frac{q}{2(1+\nu)}.$$
[Bulk modulus](Finding%20Density%20Profile.md) 
$$\kappa=\rho  \frac{dP}{d\rho}=\frac{q}{3(1-2\nu)}$$
These four properties can be used to describe the elastic properties of materials.

S-waves involve pure shear of the medium so the elastic modulus is the shear modulus which gives a speed
$$v=\sqrt{ \frac{\mu}{\rho} }.$$
For P-waves, we cannot just use Young's modulus as there is a constraint that there is no transverse displacement so there is some transverse stress.
Longitudinal strain:
$$\varepsilon_{i}=\frac{\sigma_{i}}{q}$$
Lateral strain:
$$\varepsilon_{j}=-\frac{\nu\sigma_{i}}{q}$$
Using these set of axes:
![[Pasted image 20241112201804.png]]
$$\varepsilon_{1}=\frac{1}{q}[\sigma_{1}-\nu(\sigma_{1}+\sigma_{2})]$$
$$\varepsilon_{2}=\frac{1}{q}[\sigma_{2}-\nu(\sigma_{3}+\sigma_{1})]$$
$$\varepsilon_{3}=\frac{1}{q}[\sigma_{3}-\nu(\sigma_{1}+\sigma_{2})].$$

Given the constraint of no transverse displacement, $\varepsilon_{2}=\varepsilon_{3}=0$ so
$$\sigma_{2}=\nu(\sigma_{1}+\sigma_{3});\;\sigma_{3}=\nu(\sigma_{1}+\sigma_{2})$$
This gives
$$(\sigma_{2}+\sigma_{3})(1-\nu)=2\nu\sigma_{1}$$
$$\implies \frac{\sigma_{1}}{\varepsilon_{1}}=\frac{q(1-\nu)}{(1-2\nu)(1+\nu)}=\kappa+\frac{4}{3}\mu.$$
This gives the speed of P-waves to be
$$v_{p}=\sqrt{ \frac{{\kappa+\frac{4}{3}\mu}}{\rho}}.$$
