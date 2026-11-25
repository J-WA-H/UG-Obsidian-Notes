For orbital angular momentum, 
$$\underline{\hat{L}}=\underline{\hat{r}}\times(-i\hbar \underline{\nabla}).$$
$$[\hat{L}_{x},\hat{L}_{y}]=i\hbar \hat{L}_{z}$$
$$[\hat{L}^2,\hat{L}_{z}]=0.$$
$$|\underline{l}|=\sqrt{ \ell(\ell+1) }\hbar$$
$$L_{z}=m_{\ell}\hbar.$$
The [magnetic moment](Magnetic%20Dipoles.md): $\underline{\mu}_{\ell}=-\gamma \underline{l}$.
$$(\mu_{\ell})_{z}=-\gamma l_{z}=-(\gamma \hbar)m_{\ell}=-\mu_{B}m_{\ell}.$$
Energy: $E_\ell=-\underline{\mu}_{\ell}\cdot \underline{B}=-(\mu_{\ell})_{z}B=\mu_{B}Bm_{\ell}\implies E_{\ell}$ is quantised.

Spin:
$$[\hat{S}^2,\hat{S}_{z}]=0$$
$$|\underline{s}|=\sqrt{ s(s+1) }\hbar.$$
$$s_{z}=m_{s}\hbar.$$
$$\underline{\mu}_{s}=-g_{s}\gamma \underline{S}$$
$$(\mu_{s})_{z}=-g_{s}\mu_{B}m_{s}$$
$$\therefore E_{s}=-\underline{\mu}_{s}\cdot \underline{B}=g_{s}\mu_{B}Bm_{s}.$$
Spin-Orbit Coupling:

![[Pasted image 20250123155238.png]]
Consider an electron orbiting a positive charge. The angular momentum points into the page. Moving to the electrons frame of reference, the positive charge is orbiting which represents a current, so using the right hand rule $\underline{\mu}$ points into the page
$$\therefore \underline{\mu}\;||\;\underline{L}.$$
The spin-orbit energy is given by
$$E=-\underline{\mu}_{s}\cdot \underline{B}\propto\left( \frac{dV}{dr} \right)\underline{S}\cdot \underline{L}.$$
Total angular momentum, $\underline{J}=\underline{L}+\underline{S}$:
$$[\hat{J}^2,J_{z}]=0$$
$$|\underline{j}|=\sqrt{ j(j+1) }\hbar$$
$$|l-s|\leq j\leq l+s.$$
$$J_{z}=m_{j}\hbar.$$
$\underline{\mu}_{j}=-g_{j}\gamma \underline{J}$, where
$$g_{j}=\frac{3}{2}+\frac{{s(s+1)-\ell(\ell+1)}}{2j(j+1)}.$$
Energy: $E_{j}=-\underline{\mu}_{j}\cdot \underline{B}=-(\mu_{j})_{z}B=g_{j}\mu_{B}Bm_{j}$.

For multi-electron atoms, there are two contributions - Coulomb and spin orbit.

For light atoms, coulomb contribution $\gg$ spin orbit contribution.

This gives the LS/Russel-Saunders coupling
![[Pasted image 20250123161007.png]]
Hund's rules:
- Maximise $S$
- Maximise $L$
- select $J$
	- $j=|l-s|$ if shell < half filled
	- $j=l+s$ if shell > half filled.

Example: consider a material with 9 electrons
![[Pasted image 20250123161247.png]]
$$\sum m_{s}=7\cdot \frac{1}{2}-2\cdot \frac{1}{2}=\frac{5}{2}$$
$$\sum m_{l}=3+2=5.$$
As the shell is more than half full, $J=L+S=5+\frac{5}{2}=\frac{15}{2}$.

For a single electron atom we have the [Hamiltonian](Diamagnetism.md):
$$\hat{H}_{mag}=\gamma(\underline{l}+g_{s}\underline{s})\cdot \underline{B}+\frac{e^2}{8m}(\underline{B}\times \underline{r})^2.$$
For a multi electron atom:
$$\sum \underline{l}_{i}=\underline{L};\;\sum \underline{s}_{i}=\underline{S}.$$
$$\therefore \hat{H}_{mag}=g_{J}\gamma \underline{B}\cdot \underline{J}+\frac{e^2}{8m}\sum_{i}(\underline{B}\times \underline{r}_{i})^2.$$
For a full shell, $\underline{L}=\underline{S}=\underline{J}=\underline{0}$, hence the paramagnetic term is zero so the solid is diamagnetic.