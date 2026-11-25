The energy of a [spin wave](Spin%20Waves.md) is given by
$$\hbar \omega=4J_{ex}S[1-\cos(qa)].$$
Plotting this as a function of $q$ in the first Brillouin zone gives
![[Pasted image 20250205164324.png]]

For a given wavenumber $q$ the spin wave can only take a fixed value of energy $\hbar \omega$. This dispersion graph is similar to the phonon dispersion graph, and like phonons, spin waves have quantised energies, and can be thought of as quasi-particles called magnons.

Magnons represent a spin flip.

Insight can be gained from quantum mechanics.
Call the ground state $\ket{0}=\uparrow\uparrow\uparrow\uparrow\uparrow$ and the spin flip of the $j^{th}$ particle $\ket{j}=\uparrow\uparrow\downarrow\uparrow\uparrow$.
- $\ket{0}$ is an eigenstate of the [magnetic Hamiltonian](Angular%20Momentum%20in%20QM.md)
	$$\hat{H}_{mag}\ket{0}=E_{0}\ket{0}  $$
- $\ket{j}$ is not an eigenstate of $\hat{H}_{mag}$,
	$$\hat{H}_{mag}\ket{j}\neq E_{j}\ket{j}  $$
- The excited state $\ket{q}$ is given by
$$\ket{q}=\frac{1}{\sqrt{ N }}\sum_{j}e^{iqja}\ket{j}  $$
where $N$ is the number of atoms.

This tells us that a single spin flip is spread across all atoms, so the total spin change is from $-\frac{\hbar}{2}$ to $\frac{\hbar}{2}$,
$$-\frac{\hbar}{2}-\frac{\hbar}{2}=-\hbar.$$
This means that magnons have integer spin so magnons are bosons.
