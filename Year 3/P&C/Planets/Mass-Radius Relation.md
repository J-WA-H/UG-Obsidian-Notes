Simplifications:
- Ignore thermal effects on equations of states. Decent approximation for solids but not gases.
- Ignore energy stored in magnetic field, which is dwarfed by gravitational energy.

The viral theorem states that $2T+V=0$, given that both attractive forces obey the inverse square law. $T$ is the degeneracy (kinetic) energy and $V$ is the sum of the two attractive potential energies. 

For a cold material with $n_{e}$ electrons per unit volume, momentum space will be filled up to $p_{0}$ where
$$n_{e}=\frac{2}{h^3} \frac{4\pi}{3}p_{0}^3$$
where $p_{0}$ is the outer momentum.
$$\implies p_{0}=h\left( \frac{3}{8\pi}n_{e} \right)^{1/3}$$
The phase space density of states satisfies
$$\frac{dn_{e}}{dp}=\frac{2}{h^3}4\pi p^2=\frac{8\pi}{h^3}p^2.$$
Assume non-relativistic electrons so $T=\frac{p^2}{2m}$.
We can ignore the kinetic energy of the nuclei and integrate over momenta to give the kinetic energy per unit volume
$$\int_{0}^{p_{0}} \frac{dn_{e}(p)}{dp} \frac{p^2}{2m_{e}}dp=\frac{8\pi}{10h^3m_{e}}p_{0}^5=\frac{3h^2n_{e}}{10m_{e}}\left( \frac{3n_{e}}{8\pi} \right)^{2/3}.$$
A planet contains a mean number of electrons per unit volume
$$n_{e}=\frac{Zm_{p}}{Am_{H}}\left( \frac{4}{3}\pi R_{p}^3 \right)^{-1}.$$
Eliminating $n_e$ gives degeneracy energy:
$$T_{d}=\beta\left( \frac{Zm_{p}}{A} \right)^{5/3} \frac{1}{R_{p}^2}.$$
$$\beta=\frac{9}{40\pi}\left( \frac{3}{16\pi} \right)^{4/3} \frac{h^2}{m_{e}m_{H}^{5/3}}.$$
Consider an atom with nucleus having charge $Ze$ surrounded by a uniform number density of electrons out to a distance $a$ s.t.
$$n_{e}=\frac{Z}{\frac{4}{3}\pi a^3}.$$
We aim to find the potential energy of this single atom by bringing successive shells of charge in from infinity to give
$$V_{e}=\int_{0}^a \frac{{Ze-\frac{4}{3}\pi r^3n_{e}e}}{4\pi \varepsilon_{0}r}(-4\pi r^2n_{e}e)dr=-\frac{9}{10} \frac{Z^2e^2}{4\pi \varepsilon_{0}a}.$$
The planets total electrostatic energy is this value multiplied by the number of atoms in the planet.
$$V_{e}=-\frac{M_{p}}{Am_{H}} \frac{9}{10} \frac{Z^2e^2}{4\pi \varepsilon_{0}a}.$$
We can rewrite $a$, the scale of the individual electron cloud, in terms of the planet's radius.
$$a^3\approx \frac{4}{3}\pi R_{p}^3 \frac{Am_{H}}{M_{p}}$$
$$\therefore V=-\alpha\frac{M_{p}^{4/3}Z^2}{R_{p}A^{4/3}}.$$
We have the gravitational energy as well:
$$V_{G}=-\frac{\gamma M_{p}^2}{P_{p}}.$$
The mass-radius relation is given by
$$2\beta\left( \frac{M_{p}Z^5}{A^5} \right)^{1/3}=R_{p}\left( \frac{\alpha Z^2}{A^{4/3}}+\gamma M_{p}^{2/3} \right).$$
For small masses:
$$\frac{\alpha^2Z^2}{A^{4/3}}\gg \gamma M_{p}^{2/3}\therefore R_{p}\propto M_{p}^{1/3}$$
For large masses:
$$\frac{\alpha^2Z^2}{A^{4/3}}\ll \gamma M_{p}^{2/3}\therefore R_{p}\propto M_{p}^{-1/3}.$$
Maximum planet size is when $\frac{dR_{p}}{dM_{p}}=0$:
$$\therefore R_{max}=\frac{\rho}{\sqrt{ \alpha \gamma }} \frac{Z^{2/3}}{A}.$$
