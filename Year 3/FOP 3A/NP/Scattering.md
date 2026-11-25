After introducing [[Relativistic Kinematics]], we can now look at the case for scattering.

Experiment: 
We can measure scattering by firing particles at a screen.
$$N_{scatter}=\frac{\sigma N_{t}}{A}N_{in}.$$
We call $\frac{N_{t}N_{in}}{A\Delta t}$ the instantaneous luminosity
$$N_{scatter}=\mathcal{L}\Delta t\sigma$$
where $\sigma$ is the cross-sectional area of the particle, and $N_t$ is the number of particles.
![[Pasted image 20241121144254.png]]
This gives the probability of scattering to be
$$P_{i\to f}=\frac{\sigma}{A}=\frac{\sigma L}{AL}$$
which yields
$$P_{i\to f}=\frac{\sigma vt}{V}.$$

Theory:
[[Fermi's Golden Rule]] for an initial state $i$ to final state $f$:
$$P_{i\to f}=\sum_{f}2\pi t\delta(E_{i}-E_{f})\lvert \mathcal{M}_{if} \rvert^2 $$
where $\mathcal{M}_{if}=\bra{f}H_{int}\ket{i}=\frac{\mathcal{M}_{pp'}}{V}$
Consider the potential well where
$$n=\left( \frac{Lp}{2\pi \hbar} \right).$$
Convert the sum to an integral
$$\sum_{n_{x},n_{y},n_{z}}\to \int(dn)^3=\int\left( \frac{Ldp}{2\pi} \right)^3=\int \frac{V(dp)^3}{(2\pi)^3}.$$
This gives a probability of
$$P_{i\to f}=\int V \frac{d^3p'}{(2\pi)^3}2\pi t\delta(E_{p}-E_{p'}) \frac{{\lvert \mathcal{M}_{pp'}\rvert^2}}{V^2}. $$
Equating the theory and experimental probabilities gives an expression for the cross-sectional area.
$$\frac{\sigma v\cancel{t}}{\cancel{V}}=\int \cancel{V} \frac{d^3p'}{(2\pi)^3} 2\pi \cancel{t}\delta(E_{p}-E_{p'}) \frac{{\lvert \mathcal{M}_{pp'} \rvert^2 }}{\cancel{V^2}}$$$$\implies\sigma=\frac{1}{v(2\pi)^2}\int d^3p' \delta(E_{p}-E_{p'})\lvert \mathcal{M}_{pp'} \rvert^2. $$
Moving to spherical coordinates
$$\underline{p}'=\lvert \underline{p}' \rvert \begin{bmatrix}
\sin \theta \cos \phi \\
\sin \theta \sin \phi \\
\cos \theta
\end{bmatrix}.$$
$$d^3p'=\lvert \underline{p}' \rvert^2d\lvert \underline{p}' \rvert^2\sin \theta d\theta d\phi.$$
We call $\sin \theta d\theta d\phi=d\Omega$.
$$\int \lvert \underline{p}' \rvert d\lvert \underline{p}' \rvert\delta(E_{p}-E_{p'})=\int \lvert \underline{p}' \rvert \frac{{d\lvert \underline{p}' \rvert }}{dE_{p'}}dE_{p'}\delta(E_{p}-E_{p'}).$$
Given that $E_{p'}=\sqrt{ m^2+p'^2 }$, we get
$$\frac{dE_{p'}}{dp'}=\frac{1}{2} \frac{2p'}{E_{p'}}\implies \frac{dp'}{dE_{p'}}=\frac{E_{p'}}{p'}.$$
$$\therefore \int p'^2 \frac{E_{p'}}{p'} dE_{p'} \delta(E_{p}-E_{p'})=pE_{p}.$$
This gives a cross-sectional area of
$$\sigma=\frac{E_{p}}{p(2\pi)^2}\int d\Omega E_{p}p\lvert \mathcal{M}_{pp'} \rvert^2$$
$$=\int d\Omega \left\lvert  \frac{E_{p}\mathcal{M}_{pp'}}{2\pi}  \right\rvert^2. $$
