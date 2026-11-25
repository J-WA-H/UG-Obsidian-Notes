Consider a capacitor connected to an AC source.
![[Pasted image 20250306111438.png]]
The capacitance of the capacitor is then a function of frequency
$$C(\omega)=\varepsilon_{0}\varepsilon _{r}(\omega)\left( \frac{A}{d} \right).$$
where $\varepsilon_{r}(\omega)$ is shown by
![[Pasted image 20250306111627.png]]
There are three regions that describe different polarisabilities, dipolar, ionic and electronic.

For electronic polarisability, consider a neutral atom.
![[Pasted image 20250306112257.png]]
The electron cloud is shifted by the electric field which creates an [[Electric Dipole]].

This can be achieved at high frequencies shown in the plot as electrons are light so can be easily moved, even by a rapidly oscillating E-field.

For ionic polarisability, consider a sodium chloride crystal.
![[Pasted image 20250306112626.png]]
The ions are moved by the external field that creates a dipole. This is only present at low and medium frequencies as ions are heavy compared to electrons so they are harder to move.

For dipolar polarisability, consider a water molecule
![[Pasted image 20250306112832.png]]
This molecule contains a permanent dipole. This is only present at low frequencies as the external field moves the whole molecule, which is harder to do.

Consider electronic polarisability,
Assume the nucleus is heavy so it doesn't move due to the electric field and that the electron-nucleus interaction is modelled as a spring with spring constant $k=m\omega_{0}^2$.
![[Pasted image 20250306113729.png]]
The E-field can be modelled as $\underline{E}_{local}=\underline{E}_{0}e^{i\omega t}$ and the electron position $\underline{r}=\underline{r}_{0}e^{i\omega t}$.
The dipole moment is $\underline{\mu}=-e\underline{r}=-e\underline{r}_{0}e^{i\omega t}$.
The equation of motion of the electron cloud is given by
$$\underline{F}=m \frac{d^2\underline{r}}{dt^2}=-k\underline{r}-e\underline{E}_{local}$$
$$=-m\omega^2\underline{r}=-k\underline{r}-e\underline{E}_{local}$$
$$\implies \underline{r}=-\frac{e\underline{E}_{local}}{k-m\omega^2}=-\frac{e\underline{E}_{local}}{m(\omega_{0}^2-\omega^2)}.$$
This gives the dipole
$$\underline{\mu}=\frac{e^2\underline{E}_{local}}{m(\omega_{0}^2-\omega^2)}=\alpha \underline{E}_{local}.$$
This gives [[Polarisation]] $$\alpha=\frac{e^2}{m(\omega_{0}^2-\omega^2)}.$$
Using the Claussius-Missotti equation:
$$\frac{{\varepsilon_{r}-1}}{\varepsilon_{r}+2}=\frac{N\alpha}{3\varepsilon_{0}}\implies\varepsilon_{r}=1+\frac{Ne^2}{m\varepsilon_{0}(\omega_{0}^2-\omega^2)-\left( \frac{Ne^2}{3} \right)}.$$
![[Pasted image 20250306114414.png]]
