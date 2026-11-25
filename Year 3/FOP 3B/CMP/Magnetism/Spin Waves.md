When experimentally determining the magnetisation of a [ferromagnetic](Ferromagnetism.md) solid, it drops off faster than the theory determined by the Brillouin function,
![[Pasted image 20250205141452.png]]
Here it is shown that disorder in the solid is introduced faster than theory - spins misalign faster.

Consider a $J=\frac{1}{2}$ solid, with spin configurations either $\uparrow$ or $\downarrow$:
At $T=0\text{ K}$, $\uparrow\uparrow\uparrow\uparrow$.
At $T>0\text{ K}$, $\uparrow\downarrow\uparrow\uparrow$.
This spin flip introduces disorder. In reality this is not how a system achieves disorder.

In reality, the spins shift by a slight angle as this requires a lower energy than a full spin flip and process about the axis parallel to the original spin, which causes this difference in $M$.

![[Pasted image 20250205142759.png]]

Consider a 1D chain of atoms separated with a distance $a$,
![[Pasted image 20250205143045.png]]
Each atom has been assigned an index that increases in integer intervals.
The [exchange energy](Exchange%20Interaction.md) at the $j^{th}$ atom is
$$E=\sum_{i\neq j}-J_{ij}\underline{S}_{i}\cdot \underline{S}_{j}.$$
Assuming only the nearest neighbours are important, this gives
$$E=-2J_{ex}\underline{S}_{j}\cdot(\underline{S}_{j-1}+\underline{S}_{j+1}).$$
We know that the [magnetic dipole](Angular%20Momentum%20in%20QM.md) is given by $\underline{\mu}=-\gamma g_{s}\underline{S}_{j}$. This gives the energy as
$$E=-\underline{\mu}\cdot\left[ -\frac{2J_{ex}}{\gamma g_{s}}(\underline{S}_{j-1}-\underline{S}_{j+1}) \right].$$
As the energy of a magnetic dipole is given by $E=-\underline{\mu}\cdot \underline{B}$, this exchange energy gives an effective $B$ field,
$$\underline{B}_{eff}=-\frac{2J_{ex}}{\gamma g_{s}}(\underline{S}_{j-1}+\underline{S}_{j+1}).$$
Consider the [torque](Magnetic%20Dipoles.md), 
$$\tau=\frac{d\underline{S}_{j}}{dt}=\underline{\mu}\times \underline{B}_{eff}=-\gamma g_{s}\underline{S}_{j}\times\left[ -\frac{2J_{ex}}{\gamma g_{s}}(\underline{S}_{j-1}+\underline{S}_{j+1}) \right].$$
This gives the equation of motion for the spin wave,
$$\frac{d\underline{S}_{j}}{dt}=\frac{2J_{ex}}{\hbar}\underline{S}_{j}\times(\underline{S}_{j-1}+\underline{S}_{j+1}).$$
The $\hbar$ comes from quantum mechanics.
To solve this, assume the spins are nearly vertical, $S_{j}^{z}\approx S$ and call $\underline{S}_{j-1}+\underline{S}_{j+1}=\underline{S}_{k}$,
$$\underline{S}_{j}\times \underline{S}_{k}=\begin{bmatrix}
S_{j}^{x} \\
S_{j}^{y} \\
S
\end{bmatrix}\times \begin{bmatrix}
S_{k}^x \\
S_{k}^y \\
2S
\end{bmatrix}=\begin{bmatrix}
2SS_{j}^y-SS_{k}^{y} \\
-2SS_{k}^x+SS_{k}^{x} \\
S_{j}^xS_{k}^y-S_{j}^yS_{k}^x
\end{bmatrix}.$$
Since $S_{j}^{z}\approx S$, $S_{j}^x,S_{j}^y$ are small so $S_{j}^{x}S_{k}^{y}-S_{j}^{y}S_{k}^{x}\approx 0$
$$\therefore \underline{S}_{j}\times \underline{S}_{k}=\begin{bmatrix}
2SS _{j}^{y}-SS_{k}^{y} \\
-2SS_{j}^{x}+SS_{k}^{x} \\
0
\end{bmatrix}.$$
Now solve for $\frac{d\underline{S}_{j}}{dt}$ for each component,
$$\frac{dS_{j}^{x}}{dt}=\frac{2J_{ex}S}{\hbar}[2S_{j}^{y}-(S_{j-1}^{y}+S_{j+1}^{y})]$$
$$\frac{dS_{j}^{y}}{dt}=-\frac{2J_{ex}S}{\hbar}[2S_{j}^{x}-(S_{j-1}^{x}+S_{j+1}^{x})]$$
$$\frac{dS_{j}^{z}}{dt}=0.$$
Take trial solutions: $S_{j}^{x}=Ae^{i(qja-\omega t)}$; $S_{j}^{y}=Be^{i(qja-\omega t)}$ where $q$ is the wavenumber.
$$\frac{dS_{j}^{x}}{dt}=-i\omega Ae^{i(qja-\omega t)}=\frac{2J_{ex}S}{\hbar}[2Be^{i(qja-\omega t)}-Be^{i(q(j-1)a-\omega t)}-Be^{i(q(j+1)a-\omega t)}]$$
$$=\frac{2J_{ex}S}{\hbar}[2-(e^{-iqa}+e^{iqa})]Be^{i(qja-\omega t)}$$
$$\therefore \frac{2J_{ex}S}{\hbar}[2-2\cos(qa)]B\cancel{e^{i(qja-\omega t)}}=-i\omega A\cancel{e^{i(qja-\omega t)}}$$
$$-i\omega A=\frac{4J_{ex}S}{\hbar}[1-\cos(qa)]B.$$
For the $y$ component, we can use the above method and get
$$-i\omega B=-\frac{4J_{ex}S}{\hbar}[1-\cos(qa)]A.$$
Dividing these equations gives
$$\frac{A}{B}=-\frac{B}{A}\implies A^2=-B^2\implies A=iB=e^{i\pi/2}.$$
This gives
$$-i\omega(iB)=\frac{4J_{ex}S}{\hbar}[1-\cos(qa)]B$$
$$\implies \hbar \omega=4J_{ex}S[1-\cos(qa)].$$
This the energy of a spin wave.