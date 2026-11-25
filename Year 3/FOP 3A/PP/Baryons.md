Baryons are systems that consist of 3 quarks.

e.g. the proton $(uud)$ with [isospin](Isospin%20and%20Strangeness.md) $\frac{1}{2}$ and spin $\frac{1}{2}$, $1^2S_{\frac{1}{2}}$
$\Delta^{++}(uuu)$ with isospin $\frac{3}{2}$ and spin $\frac{3}{2}$, $1^4S_{\frac{3}{2}}$.

Considering the possible $u,d,s$ quarks in the $1^2S_{\frac{1}{2}}$ state, plotting them on a graph of isospin and strangeness gives.
![[Pasted image 20250307145644.png]]
We can do the same for the $1^4S_{\frac{3}{2}}$ baryons, which include $uuu,ddd,sss$.

As baryons are fermions, they must have an [antisymmetric wavefunction](Two%20Particle%20Systems.md).
$$\psi_{total}=\psi_{spatial}\psi_{flavour}(u,d,s)\psi_{spin}(\uparrow,\downarrow)\psi_{colour}(r,g,b).$$
In the ground state, $\psi_{spatial}$ is symmetric, and by definition $\psi_{colour}$ is [antisymmetric](Colour%20Charge.md) so the product $\psi_{flavour}\psi_{spin}$ must be symmetric.

Individually, $\psi_{flavour}$ and $\psi_{spin}$ can either be symmetric of antisymmetric, but for the product to be symmetric, they must be the same
- Either $\psi_{flavour}$ is symmetric so $\psi_{spin}$ is symmetric
- Or $\psi_{flavour}$ is antisymmetric so $\psi_{spin}$ is antisymmetric
For example, $\Delta^{++}(uuu)$, $\psi_{flavour}=\ket{uuu}$. Consider if $\psi_{flavour}$ is antisymmetric, $\ket{uuu}=-\ket{uuu}$. The only was this can be true is if $\ket{uuu}=0$ as, when two quarks swap flavours, there is no way to tell which ones have swapped flavour so the only way for this to be antisymmetric is if $\ket{uuu}=0$.
As $\psi_{flavour}$ must be symmetric, $\psi_{spi n}$ must be symmetric, so all spins must be aligned, $\psi_{spin}=\ket{\uparrow\uparrow\uparrow}$, $S=\frac{3}{2}$.

For other combinations, like the proton, both combinations for $\psi_{flavour}$ and $\psi_{spin}$ are possible.

Recall the spin-spin interaction in [[Mesons]],
$$V_{SS}\propto \alpha_{s} \frac{{\hat{S}_{q_{1}}\cdot \hat{S}_{q_{2}}}}{m_{q_{1}}m_{q_{2}}}\delta(x).$$
For baryons, they can be considered as three mesons
![[Pasted image 20250307152530.png]]
$$\hat{S}^2=(\hat{S}_{q_{1}}+\hat{S}_{q_{2}}+\hat{S}_{q_{3}})^2=\sum_{i}\hat{S}_{q_{i}}+2\sum_{i>j}\hat{S}_{q_{i}}\cdot \hat{S}_{q_{j}}.$$
We knows the eigenvalues of spin are
$$\hat{S}^2\psi=S(S+1)\psi.$$
If we have a baryon with spin $S=\frac{1}{2}, \frac{3}{2}$, and quarks have spin $s=\frac{1}{2}$.
If $J=\frac{1}{2}$: $\frac{1}{2}\left( \frac{1}{2}+1 \right)=\frac{3}{4}$
If $J=\frac{3}{2}$: $\frac{3}{2}\left( \frac{3}{2}+1 \right)=\frac{15}{4}$.
$$\therefore \sum_{i>j}\hat{S}_{q_{i}}\cdot \hat{S}_{q_{j}}=\begin{cases}
-\frac{3}{4} & J=\frac{1}{2} \\
+\frac{3}{4} & J=\frac{3}{4}
\end{cases}.$$
Adding this difference to the spin-spin interaction for mesons gives the spin-spin interaction for baryons.
$$V_{SS}\propto \sum_{i>j} \frac{{\hat{S}_{q_{i}}\cdot \hat{S}_{q_{j}}}}{m_{q_{i}}m_{q_{j}}}.$$
The masses inside the sum causes issues as we know $\sum_{i>j} \hat{S}_{q_{i}}\cdot \hat{S}_{q_{j}}$ but we need $\sum_{i>j} \frac{{\hat{S}_{q_{i}}S_{\hat{q}_{j}}}}{m_{q_{i}}m_{q_{j}}}$.
The quark masses a lot

| Quark | Mass (MeV) |
| ----- | ---------- |
| u     | 2          |
| d     | 4          |
| c     | 1280       |
| s     | 95         |
| t     | 173,000    |
| b     | 4180       |
It is difficult to account for quark mass as there are many gluons that add to the effective mass. For light $(ud)$ baryons, we usually use $m_{u}\approx m_{d}\leq m_{s}$.

The sum uses educated guesses on the effective quark light.
