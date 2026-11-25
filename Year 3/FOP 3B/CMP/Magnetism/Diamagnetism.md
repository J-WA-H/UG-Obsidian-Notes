Diamagnets are materials that repel a magnetic field

From [[Larmor Procession]] we get the magnetic dipole moment
$$|\underline{\mu}|=-\frac{e^2B}{6m}\langle r^2 \rangle .$$
This gives the magnetisation ([dipole moment](Magnetic%20Dipoles.md) per unit volume)
$$|\underline{M}|=-\frac{e^2BnZ}{6m}\langle r^2 \rangle. $$
For weak magnetic materials, we have $\underline{B}=\mu_{0}(\underline{H}+\underline{M})\approx \mu_{0}\underline{H}$; $\underline{M}=\chi \underline{H}$
$$\implies \chi=\frac{M}{H}=\frac{\mu_{0}M}{B}$$
So for a diamagnetic material
$$\chi_{d}=-\frac{e^2\mu_{0}nZ}{6m}\langle r^2 \rangle. $$
The mean square $\langle r^2 \rangle$ is used as atoms have numerous electrons, each having a different value of $r$.

Bohr-Van-Leeuwen theorem states that net magnetisation is zero, as the diagram shows.
![[Pasted image 20250123114824.png]]
Here all the loops cancel each other out so the net magnetisation is zero.

For a singe electron in a B field, $\underline{B}=\underline{\nabla}\times \underline{A}$, the Hamiltonian is given by
$$\hat{H}=\frac{(\underline{p}+e\underline{A})^2}{2m}+V+\hat{H}_{s}$$
where $\hat{H}_{s}$ is the spin Hamiltonian, given by the magnetic potential energy,
$$E_{s}=-\mu_{s}\cdot \underline{B};\;\underline{\mu}_{s}=-g_{s}\gamma \underline{S}$$
$$\implies E_{s}=g_{s}\gamma \underline{B}\cdot \underline{S}$$
$$\implies \hat{H}=\frac{(\underline{p}+e\underline{A})^2}{2m}+V+g_{s}\gamma \underline{B}\cdot \underline{S}.$$
Choose the symmetric gauge, $\underline{A}=\frac{1}{2}(\underline{B}\times \underline{r})$.
$$\frac{(\underline{p}+e\underline{A} )^2}{2m}=\frac{p^2}{2m}+\frac{e}{m}\underline{p}\cdot \underline{A}+\frac{e^2}{2m}A^2.$$
$$\frac{e}{m}\underline{p}\cdot \underline{A}=\frac{e}{2m}\underline{p}\cdot(\underline{B}\times \underline{r})=\frac{e}{2m}\underline{B}\cdot(\underline{r}\times \underline{p})=\gamma \underline{B}\cdot \underline{L}.$$
$$\hat{H}=\left( \frac{p^2}{2m}+V \right)+\gamma(\underline{L}+g_{s}\underline{S})\cdot \underline{B}+\frac{e^2}{8m}(\underline{B}\times \underline{r})^2$$
The first term is the normal Hamiltonian, the second term is the paramagnetic term, and the third term is the diamagnetic term.

Using perturbation theory, the energy shift by a diamagnetic material is
$$\Delta E=\bra{0}E_{d}\ket{0}  $$
where $\ket{0}$ is the ground state.
For a B field along the z-axis, $(\underline{B}\times \underline{r})^2=B^2(x^2+y^2)$ so
$$\Delta E= \frac{e^2}{8m}[\bra{0}x^2\ket{0}+\bra{0}y^2\ket{0}]$$
$$=\frac{e^2B^2}{8m} \frac{2}{3}\langle r^2 \rangle =\frac{e^2B^2}{12m}\langle r^2 \rangle. $$
Per unit volume:
$$\Delta\varepsilon=\frac{e^2B^2}{12m}nZ\langle r^2 \rangle. $$
$E=-\underline{\mu}\cdot \underline{B}\implies\varepsilon=-\underline{M}\cdot \underline{B}$
$$\therefore |\underline{M}|=-\frac{d(\Delta\varepsilon)}{dB}=-\frac{e^2B}{6m}nZ\langle r^2 \rangle. $$
For weak magnetic materials, 
$$\chi=\frac{\mu_{0}M}{B}$$
$$\implies \chi_{d}=-\frac{e^2\mu_{0}nZ}{6m}\langle r^2 \rangle. $$
This is identical to the result from classical mechanics.
