Consider a material with zero B field at $T=0\text{ K}$, and spin states $\uparrow\downarrow$. All spin states up to the Fermi level are occupied.
![[Pasted image 20250206151909.png]]
There are an equal number of $\uparrow$ and $\downarrow$ spins so $\underline{M}=\underline{0}$.
The energy is $E=-\underline{\mu} \cdot \underline{B}=-\mu_{z}B$.
For a $J=\frac{1}{2}$ solid,
$$\underline{\mu}=-\gamma g_{s}\underline{S}\therefore\mu_{z}=-\gamma g_{s}(S_{z})=-\gamma g_{s}(m\hbar).$$
Given that $J=\frac{1}{2}$, this implies that $S=\frac{1}{2}$ so $m_{s}=\pm \frac{1}{2}$
$$\mu_{z}=-(\gamma \hbar)g_{s}m_{z}=\mp \mu_{B}.$$
This give the absolute value of the energy as $|E|=\mu_{B}B$.
If we add a non-zero B field, the bands shift by $\pm \mu_{B}B$,
![[Pasted image 20250206152338.png]]
At equilibrium, we must have a constant Fermi level so some electrons move from the spin down to the spin up state.
![[Pasted image 20250206152514.png]]
As there is an imbalance in the number of spin up and spin down states, the net magnetisation is no longer zero, and is related to the number of electrons transferred to the up band and the number of electrons transferred from the down band.
$$M=\mu_{B}(\Delta n_{\uparrow}-\Delta n_{\downarrow}).$$
$$\Delta n_{\uparrow}=\frac{1}{2}g(E_{F})(\mu_{B} B)$$
$$\Delta n_{\uparrow}=-\Delta n_{\downarrow}\implies M=g(E_{F})\mu_{B}^{2}B.$$
For weak [magnetic materials](Paramagnetism.md), $\chi=\frac{\mu_{0}M}{B}$ so
$$\chi=g(E_{F})\mu_{0}\mu_{B}^2.$$
From [[Free-Electron Theory]], 
$$g(E)dE=\frac{mk}{\pi^2\hbar^2}dE;\;g(E_{F})=\frac{mk_{F}}{\pi^2\hbar^2}=\frac{mk_{F}^2}{\pi^2(\hbar k_{F})^2}.$$
Using $E_{F}=\frac{\hbar^2k_{F}^2}{2m}$ and $k_{F}^3=3\pi^2n$ where $n$ is the free electron density,
$$g(E_{F})=\frac{m(3\pi^2n)}{\pi^2(2mE_{F})}=\frac{3n}{2E_{F}}.$$
This gives the susceptibility
$$\chi=\frac{3n\mu_{0}\mu_{B}^2}{2E_{F}}.$$
This is temperature independent, unlike in [[Paramagnetism]] where it follows Curie's law.
