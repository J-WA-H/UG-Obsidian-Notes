If the potential decreases faster than $\frac{1}{r}$ as $r\to \infty$ then at large distances we can ignore the potential.
$$\lim_{ r \to \infty }\psi(\underline{r})=\psi_{inc}(\underline{r})+\psi_{scat}(\underline{r}) $$
where $\psi_{inc}$ is the incident wavefunction and $\psi_{scat}$ being the scattered wavefunction.

These wavefunctions obey the [[Potential Scattering]] Schrodinger equation,
$$[\nabla^2+k^2]\psi(\underline{r})=0.$$
This is the same as the potential well equation so the incident wavefunction is a plane wave, which we will [choose to align](Scattering%20Experiments.md) along the $z$ axis.
$$\psi_{inc}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}=e^{ikz}.$$
This is normalised so $|\psi_{inc}|^2=1$.

We describe the scatter wave as a spherical/radial wave,
$$\psi_{scat}(\underline{r})=f(k,\theta,\phi) \frac{e^{ikr}}{r}.$$where $f(k,\theta,\phi)$ is the scattering amplitude.

This gives the behaviour of $\psi(\underline{r})$ at large distances:
$$\lim_{ r \to \infty } \psi(\underline{r})=e^{i\underline{k}\cdot \underline{r}}+f(k,\theta,\phi) \frac{e^{ikr}}{r}.$$
Consider the probability density
$$\frac{{\partial \mathcal{P}(\underline{r},t)}}{\partial t}=\frac{\partial |\psi|^2}{\partial t}=\frac{\partial \psi^{*}}{\partial t}\psi+\psi^{*} \frac{\partial \psi}{\partial t}.$$Using the time dependent Schrodinger equation gives
$$\frac{\partial}{\partial t}\int_{V}\mathcal{P}(\underline{r},t)d^3r=\frac{i\hbar}{2m}\int_{V}\psi^{*}\nabla^2\psi-(\nabla^2\psi^{*})\psi d^3r=\frac{i\hbar}{2m}\int_{V}\underline{\nabla}\cdot(\psi^{*}\underline{\nabla}\psi-(\underline{\nabla}\psi^{*})\psi)d^3r$$
$$=-\int_{V}\underline{\nabla}\cdot \underline{j}d^3r.$$
This is used to define the current of the scattered wave, where $|\underline{j}|$ is the number of particles per unit time per unit area, given by
$$\underline{j}(\underline{r})=\frac{\hbar^2}{2m}(\psi^{*}\underline{\nabla}\psi-(\underline{\nabla}\psi^{*})\psi).$$
In spherical coordinates, the del operator is given by
$$\underline{\nabla}=\frac{\partial}{\partial r}\underline{\hat{r}}+\frac{1}{r} \frac{\partial}{\partial \theta} \underline{\hat{\theta}} +\frac{1}{r\sin \theta} \frac{\partial}{\partial \phi} \underline{\hat{\phi}}.$$
Since we are considering large distances, the angular part goes to zero so
$$\underline{\nabla}=\frac{\partial}{\partial r}\underline{\hat{r}}.$$
This gives
$$\underline{\nabla}\psi_{scat}=f(k,\theta,\phi)\left( \frac{ike^{ikr}}{r}-\cancelto{0\text{ as }r\to \infty}{\frac{e^{ikr}}{r^2} }\right)=f(k,\theta,\phi) \frac{ike^{ikr}}{r}$$
$$\therefore \underline{j}(\underline{r})=\frac{\hbar^2}{2mi} 2ik \frac{|f(k,\theta,\phi)|^2}{r^2}\underline{\hat{r}}=\frac{\hbar k}{m} \frac{|f(k,\theta,\phi)|^2}{r^2}\underline{\hat{r}}.$$
From the definition of the current, we get
$$Nd\Omega=|\underline{j}|A$$
where $A$ is the area of the solid angle.
$$Nd\Omega=|\underline{j}|r^2d\Omega=\frac{\hbar k}{m}|f(k,\theta,\phi)|^2d\Omega.$$The flux is equivalent to the velocity of the incoming particles, $v=\frac{\hbar k}{m}$.
$$\therefore \frac{d\sigma}{d\Omega}=|f(k,\theta,\phi)|^2.$$
The differential cross section can be measured experimentally, and $f(k,\theta,\phi)$ and be calculated. This links theory and experiment.
