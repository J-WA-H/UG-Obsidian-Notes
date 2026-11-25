This interpretation comes from quantum field theory but is useful in relativistic quantum mechanics.

The main idea is that negative energy particles propagating backwards through time are equivalent to positive energy antiparticles moving forwards in time.

Example: $\pi^{+}$ scattering by a potential in 2nd order perturbation theory.
In normal quantum mechanics.
![[Pasted image 20250311154013.png]]
Feynman considered that in relativistic quantum mechanics, we should also consider scattered particles moving backwards in time
![[Pasted image 20250311154124.png]]
The middle $\pi^{+}$ appears to be moving backwards in time, but instead it is a positive energy $\pi^{-}$ moving forwards in time.

There are are additional trajectories in 2nd order relativistic QM.

This interpretation also helps thinking about currents.

For plane wave solutions of the Klein-Gordon equation,
$$j^{\mu}_{\ell m}(\pi^{+})=eP=2e|N|^2((p^2+m^2)^{1/2},\underline{p})$$
where $P$ is the probability current for negative energies.
For a $\pi^{-}$ with positive energy,
$$j^{\mu}_{\ell m}(\pi^{-})=e 2|N|^2(-(p^2+m^2)^{1/2},-\underline{p}).$$
This shows negative probabilities in the Klein-Gordon equation is the positive probabilities of having antiparticles.

The emission of an antiparticle with 4-momentum $p^{\mu}$ is equivalent to absorption of particle with 4-momentum $-p^{\mu}$.
![[Pasted image 20250311154959.png]]
For the negative energies of the Dirac equation, consider
$$i\hbar \frac{\partial \psi}{\partial t}=(-ic\underline{\alpha}\cdot \underline{\nabla}+\beta mc^2)\psi.$$
$$\psi=Ue^{-ip^{\mu}x_{\mu}/\hbar};\;U=\begin{bmatrix}
\phi \\
\chi
\end{bmatrix}.$$
This gives the Dirac equation in matrix notation is
$$p^{0}c \begin{bmatrix}
\phi \\
\chi
\end{bmatrix}=\begin{bmatrix}
mc^2\mathbb{I}_{2} & \underline{\sigma}\cdot \underline{p}c \\
\underline{\sigma}\cdot \underline{p}c & -mc^2\mathbb{I}_{2}
\end{bmatrix}\begin{bmatrix}
\phi \\
\chi
\end{bmatrix}.$$
$$p^{0}c\phi=mc^2\phi+c\underline{\sigma}\cdot \underline{p}\chi$$
$$p^{0}c\chi=c\underline{\sigma}\cdot \underline{p}\phi-mc^2\chi.$$
$$(p^{0}c-mc^2)\phi=c\underline{\sigma}\cdot \underline{p}\chi$$
$$(p^{0}+mc^2)\chi=c\underline{\sigma}\cdot \underline{p}\phi.$$
$$((p^{0}c)^2-m^2c^4)\phi=c^2|\underline{p}|\phi.$$
$$\therefore U_{1,2}=\begin{bmatrix}
\phi_{1,2} \\
\frac{c\underline{\sigma}\cdot\underline{p}}{E+mc^2}\phi_{1,2}
\end{bmatrix}$$
where
$$\phi^{1}=\begin{bmatrix}
1 \\
0 
\end{bmatrix};\;\phi^{2}=\begin{bmatrix}
0 \\
1
\end{bmatrix}.$$
Each $\phi$ represents the spin up / spin down respectively.

For the negative energy solutions,
$$p^{0}=-\frac{E}{c};\;U=\left[ -\frac{c\underline{\sigma}\cdot \underline{p}}{E+mc^2}\chi \right].$$
Using Feynman correspondence,
$$+\text{ve},\;e^{-ipx}$$
$$-\text{ve},\;e^{ipx}$$
which needs solutions $p^{\mu}\to-p^{\mu}$, i.e. $p^{\mu}=\left( -\frac{E}{c},-\underline{p} \right)$.
$$U^{3,4}=\begin{bmatrix}
\frac{c\underline{\sigma}\cdot \underline{p}}{E+mc^2}\chi_{1,2} \\
\chi_{1,2}
\end{bmatrix}.$$
Now negative energy solutions are spin down and positive energy solutions are spin up.
$$\chi^{1}=\begin{bmatrix}
0 \\
1
\end{bmatrix};\;\chi^{2}=\begin{bmatrix}
1 \\
0
\end{bmatrix}.$$
