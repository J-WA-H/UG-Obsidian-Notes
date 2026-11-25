Consider a dielectric material
![[Pasted image 20250305162819.png]]
At zero external electric field, the [electric dipoles](Electric%20Dipole.md) are randomly orientated so have no polarisation. When an external E-field is applied, the dipoles experience a torque which moves them into the lowest energy configuration where all the dipoles align with the E-field. This polarises the material.

Polarisation is the net dipole moment per unit volume.

Due to aligned dipoles, charges build up at the surface.
![[Pasted image 20250305163417.png]]
Theorem: For uniform polarisation, the surface charge density is given by
$$\sigma=\underline{P}\cdot \underline{\hat{n}}$$where $\underline{\hat{n}}$ is the surface vector normal.
For the right hand surface (RHS), $\underline{\hat{n}}\parallel\underline{P}$ which predicts a positive charge density, which is what's observed.
For the LHS, $\underline{\hat{n}}\parallel-\underline{P}$ which predicts a negative charge density as observed. 
For the top and bottom surfaces, $\underline{\hat{n}}\perp \underline{P}$ so the charge density is zero.

Using this gives the macro electric field,
$$\underline{E}_{macro}=\underline{E}_{ext}+\underline{E}_{1}$$where $\underline{E}_{1}$ is the internal field caused by the charges, which from Gauss' law is
$$E_{1}=-\frac{\sigma}{\varepsilon_{0}}.$$
$$\implies E_{macro}=E_{ext}-\frac{\sigma}{\varepsilon_{0}}.$$
There is also a micro electric field - the electric field one dipole experiences.
For a single dipole, the dipole moment is
$$\underline{\mu}=\alpha \underline{E}_{local}$$
where $\alpha$ is the polarisability and $\underline{E}_{local}$ is the local electric field.

Calculating the microscopic E-field requires an atomistic calculation.
![[Pasted image 20250305164450.png]]
The local E-field only effects it neighbouring atoms so there is a continuum where atoms don't experience the local E-field.
It is helpful to separate the two parts.
![[Pasted image 20250305164631.png]]
The E-field inside the continuum is $E_{1}=-\frac{\sigma}{\varepsilon_{0}}$, and the field experienced due to the charge build up at the surface of the local atoms is $E_{2}$ - the Lorentz field.
$$\underline{E}_{3}=\frac{\underline{P}}{3\varepsilon_{0}}.$$

For the atomistic calculation, consider the dipole,
![[Pasted image 20250305164836.png]]
For a single dipole,
$$\underline{E}(\underline{r})=\frac{{3(\underline{\mu}\cdot \underline{r})\underline{r}-r^2\underline{\mu}}}{4\pi\varepsilon_{0}r^5}.$$
This is the electric field experience by an atom due to a dipole, so for all the surrounding atoms the total field is
$$\underline{E}_{3}=\sum_{i} \frac{{3(\underline{\mu}\cdot \underline{r}_{i})\underline{r}_{i}-r_{i}^2\underline{\mu}}}{4\pi\varepsilon_{0}r_{i}^5}.$$
![[Pasted image 20250305165147.png]]
In the $x$ direction,
$$E_{3x}=\sum_{i} \frac{{3\mu x_{i}x_{i}-r_{i}^2\mu}}{4\pi\varepsilon_{0}r_{i}^5}=\frac{\mu}{4\pi\varepsilon_{0}}\sum_{i} \frac{{3x_{i}^2-r_{i}^2}}{r_{i}^5}.$$
For a cubic dielectric,
$$\sum_{i} \frac{x_{i}^2}{r_{i}^5}=\sum_{i} \frac{y_{i}^2}{r_{i}^5}=\sum_{i} \frac{z_{i}^2}{r_{i}^5}$$
and
$$r_{i}^2=x_{i}^2+y_{i}^2+z_{i}^2$$
$$\implies E_{3x}=0.$$
$$\implies E_{3y}=E_{3z}=0.$$
$$\therefore \underline{E}_{local}=\underline{E}_{ext}+\underline{E}_{1}+\underline{E}_{2}+\cancelto{0}{\underline{E}_{3}}$$
$$=\left( E_{ext}-\frac{\sigma}{\varepsilon_{0}} \right)+\frac{P}{3\varepsilon_{0}}$$
This is equivalent to
$$\underline{E}_{local}=\underline{E}_{macro}+\frac{\underline{P}}{3\varepsilon_{0}}.$$
As polarisation is given by
$$\underline{P}=N\underline{\mu}=N\alpha \underline{E}_{local}$$
Using the expression for $E_{local}$,
$$N\alpha=\frac{P}{E_{local}}=\frac{P/E_{macro}}{1+\frac{P/E_{macro}}{3\varepsilon_{0}}}.$$
Using the electric displacement field, $D=\varepsilon_{0}E_{macro}+P=\varepsilon_{0}\varepsilon_{r}E_{macro}$
$$\implies \frac{P}{E_{macro}}=\varepsilon_{0}(\varepsilon_{r}-1)$$
$$\implies \frac{{\varepsilon_{r}-1}}{\varepsilon_{r}+2}=\frac{N\alpha}{3\varepsilon_{0}}.$$
This is the Claussius-Messotti equation.
