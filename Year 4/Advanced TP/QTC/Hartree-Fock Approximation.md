Consider the full Hamiltonian for a 2-particle atom in atomic units
$$\hat{H}=\underbrace{-\frac{\nabla^2}{2}-\frac{\nabla'^2}{2}}_{\text{Kinetic Energy}}+\underbrace{V(\vec{r})+V(\vec{r}')}_{\text{P.E. from Nuclei}}+\underbrace{\frac{1}{|\vec{r}-\vec{r}'|}}_{\text{P.E from }e^-e^-}.\tag{4.1} $$
We want to calculate the expectation value of this Hamiltonian with respect to $\Psi_{a}$ [(3.1)](Reduced%20Density%20Matrices.md),
$$\bra{\Psi_{a}}\hat{H}\ket{\Psi_{a}} =\bra{\Psi_{a}}T\ket{\Psi_{a}}+ \bra{\Psi_{a}}V_{ext}\ket{\Psi_{a}} + \bra {\Psi_{a}}V_{ee}\ket{\Psi_{a}} \tag{4.2}.$$
Consider the first term,
$$\bra{\Psi_{a}}T\ket{\Psi_{a}}=\frac{1}{2}\iint d^3rd^3r'[\phi_{1}^{*}(\vec{r})\phi_{2}^{*}(\vec{r}')-\phi_{1}^{*}(\vec{r}')\phi_{2}^{*}(\vec{r})]\left[ -\frac{\nabla^2}{2}-\frac{\nabla'^2}{2} \right][\phi_{1}(\vec{r})\phi_{2}(\vec{r}')-\phi_{1}(\vec{r}')\phi_{2}(\vec{r})]\tag{4.3}. $$
From orthogonality all cross terms vanish so
$$=\frac{1}{2}\left[ \int d^3r\,\phi_{1}^{*}(\vec{r})\left( -\frac{\nabla^2}{2} \right)\phi_{1}(\vec{r})+\int d^3r\,\phi_{2}^{*}(\vec{r})\left( -\frac{\nabla^2}{2} \right)\phi_{2}(\vec{r})+\int d^3r'\,\phi_{1}^{*}(\vec{r}')\left( -\frac{\nabla'^2}{2} \right)\phi_{1}(\vec{r}')+\int d^3r'\,\phi_{2}^{*}(\vec{r}')\left( -\frac{\nabla'^2}{2} \right)\phi_{2}(\vec{r}') \right]\tag{4.4}. $$
This simplifies to, since integration variables are dummy variables,
$$\bra{\Psi_{a}}T\ket{\Psi_{a}}=\int d^3r\,\phi_{1}^{*}(\vec{r})\left( -\frac{\nabla^2}{2} \right)\phi_{1}(\vec{r})+\int d^3r\,\phi_{2}^{*}(\vec{r})\left( -\frac{\nabla^2}{2} \right)\phi_{2}(\vec{r}).\tag{4.5}   $$
For the second term,
$$\bra{\Psi_{a}}V_{ext}\ket{\Psi_{a}} = \frac{1}{2}\iint d^3r d^3r'[\phi_{1}^{*}(\vec{r})\phi_{2}^{*}(\vec{r}')-\phi_{1}^{*}(\vec{r}')\phi_{2}^{*}(\vec{r})][V(\vec{r})+V(\vec{r}')][\phi_{1}(\vec{r})\phi_{2}(\vec{r}')-\phi_{1}(\vec{r}')\phi_{2}(\vec{r})]\tag{4.6} $$$$=\int dr\,V(r)[|\phi_{1}(\vec{r})|^2+|\phi_{2}(\vec{r})|^2]=\int dr\,V(\vec{r})\rho(\vec{r})\tag{4.7}. $$

For the third term,
$$\bra{\Psi_{a}}V_{ee}\ket{\Psi_{a}}=\iint \frac{|\Psi_{a}(\vec{r},\vec{r}')|}{|\vec{r}-\vec{r}'|^2}=\underbrace{\frac{1}{2}\iint dr dr' \frac{\rho(\vec{r})\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}}_{U[\rho]}-\underbrace{\frac{1}{2}\iint dr dr'  \frac{\rho(\vec{r},\vec{r}')\rho(\vec{r}',\vec{r})}{|\vec{r}-\vec{r}'|}}_{E_{X}[\rho]}.\tag{4.8} $$
For general $N$,
$$\bra{\Psi_{a}}\hat{H}\ket{\Psi_{a}} = \sum_{\sigma}\sum_{i=1}^{N^\sigma}\bra{\phi_{i}^\alpha}\left(-\frac{\nabla^2}{2}\right)\ket{\phi_{i}^\sigma} + \int d^3r\,\rho(\vec{r})V(\vec{r})+\frac{1}{2}\iint drdr'\, \frac{\rho(\vec{r})\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}-\frac{1}{2}\sum_{\sigma}\iint dr dr' \frac{\rho^\sigma(\vec{r},\vec{r}')\rho(\vec{r}',\vec{r})}{|\vec{r}-\vec{r}'|}\tag{4.9}. $$
We aim to find the single particle wavefunctions $\phi_{i}^\sigma,\phi_{i}^\bar{\sigma}$ such that $\bra{\psi}\hat{H}\ket{\psi}$ is minimised under the constraint $\braket{ \psi | \psi }=1$.
Minimise
$$E[\psi]=\bra{\psi} H\ket{\psi} -\lambda \braket{ \psi | \psi } \tag{4.10}. $$$$E[\{ \phi_{i}^\uparrow \},\{ \psi_{j}^\downarrow \}]=T[\phi]+V_{ext}[\rho_{\phi}]+U[\rho_{\phi}]+E_{X}[\rho^\sigma_{\phi}]\tag{4.11}. $$The Hartree / Coulomb energy is $U[\rho]$ and the exchange energy of $\rho^\sigma(\vec{r},\vec{r}')$ is $E_X[\{ \rho^\sigma \}]$. Vary one orbit (single particle wavefunction) $\phi_{k}^\sigma(\vec{r})$:
$$\begin{matrix}
\phi^\sigma_{k}(\vec{r})\to \phi^\sigma_{k}(\vec{r})+\varepsilon U(\vec{r}) \\
\phi^\sigma_{i,j}(\vec{r})\to \phi^\sigma_{i,j}(\vec{r}) & i,j\neq k \\
\phi_{k}^{\sigma*}(\vec{r})\to \phi_{k}^{\sigma*}(\vec{r})+\varepsilon U^{*}(\vec{r})
\end{matrix}\tag{4.12}. $$This gives
$$\phi_{k}^\sigma(\vec{r})\phi_{k}^{\sigma*}(\vec{r}')\to[\phi _{k}^\sigma(\vec{r})+\varepsilon U(\vec{r})][\phi_{k}^{\sigma*}(\vec{r}')+\varepsilon U^{*}(\vec{r}')]=\phi^\sigma_{k}(\vec{r})\phi_{k}^{\sigma*}(\vec{r}')+\varepsilon [\phi_{k}^{\sigma}(\vec{r})U^{*}(\vec{r}')+U(\vec{r})\phi_{k}^{\sigma*}(\vec{r}')]+\mathcal{O}(\varepsilon^2).\tag{4.13}. $$
$$\implies \rho(\vec{r})\to \rho(\vec{r})+\varepsilon[U^{*}(\vec{r})\phi_{k}^\sigma(\vec{r})+\phi_{k}^{\sigma*}(\vec{r})U(\vec{r})]+\mathcal{O}(\varepsilon^2),\;\rho^\sigma(\vec{r},\vec{r}')\to\rho^\sigma(\vec{r},\vec{r}')+\varepsilon[\phi_{k}^
\sigma(\vec{r})U^{*}(\vec{r}')+U(\vec{r})\phi_{k}^{\sigma*}(\vec{r}')]+\mathcal{O}(\varepsilon^2)\tag{4.14} $$
and $\rho^\bar{\sigma}(\vec{r},\vec{r})=\rho^\bar{\sigma}(\vec{r},\vec{r}')$.
We want to minimise $T+V_{ext}+U+E_{X}-\sum_{\tau}\lambda_{\tau}\sum_{i=1}^{N^\tau}\braket{ \phi_{i}^\tau | \phi_{i}^\tau }=E[\{ \phi_{i}^\sigma \},\{ \phi_{j}^\bar{\sigma} \}]$.
$$T\to T+\varepsilon\left[ -\frac{1}{2}\int dr\,U^{*}(\vec{r})\nabla^2\phi_{k}^{\sigma*}(\vec{r})-\frac{1}{2}\int dr\,\phi^\sigma_{k}\nabla^2U(\vec{r}) \right]\tag{4.15} $$
$$V_{ext}\to V_{ext} +\varepsilon\left[ \int dr\,U^{*}(\vec{r})V(r)\phi_{k}^{\sigma *}(\vec{r})+\int dr\,\phi_{k}^\sigma(\vec{r})V(\vec{r})U(\vec{r}) \right]\tag{4.16} $$
$$U\to U+\varepsilon \int d^3r\,U^{*}(\vec{r})\int \frac{dr'\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}\phi_{k}^\sigma(\vec{r})+\varepsilon \int d^3r\,\phi_{k}^{\sigma*}(\vec{r})\int dr' \frac{\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}U(\vec{r})\tag{4.17} $$
$$E_{X}\to E_{X}-\varepsilon \int dr\,U^{*}(\vec{r})\int dr' \frac{\rho^\sigma(\vec{r},\vec{r}')}{|\vec{r}-\vec{r}'|}\phi_{k}^\sigma(\vec{r}')-\varepsilon \int dr\,\phi_{k}^{\sigma*}(\vec{r})\int dr' \frac{\rho^\sigma(\vec{r},\vec{r}')}{|\vec{r}-\vec{r}'|}U(\vec{r}')\tag{4.18}. $$
$$-\sum_{\tau}\lambda_{\tau}\sum_{i}\int dr|\phi_{i}^\tau(\vec{r})|^2\to-\sum_{\tau}\lambda_{\tau}\sum_{i}\int dr |\phi_{i}^\tau(\vec{r})|^2-\varepsilon\lambda_{k}^\sigma\left[ \int dr\,U^{*}(\vec{r})\phi_{k}^\sigma(\vec{r})+\int dr\,\phi_{k}^{\sigma*}U(r) \right].\tag{4.19} $$
To minimise this we evaluate
$$\lim_{ \varepsilon \to 0 } \frac{{E[\{ \phi^\sigma_{i\neq k} \}, \phi_{k}^\sigma+\varepsilon u_{j}\{ \phi_{j}^\bar{\sigma} \}]-E[\{ \phi_{i}^\sigma \},\{ \phi_{j}^\bar{\sigma} \}]}}{\varepsilon}\tag{4.20} $$
$$=\int d^{3}r\,U^{*}(\vec{r})\left( \left[ -\frac{\nabla^2}{2}+V(\vec{r})+\int dr' \frac{\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}-\lambda_{k}^\sigma \right]\phi_{k}^\sigma(\vec{r})-\int dr' \frac{\rho^\sigma(\vec{r},\vec{r}')}{|\vec{r}-\vec{r}'|}\phi_{k}^\sigma(\vec{r}') \right)$$$$+\int d^{3}r\,\phi_{k}^{\sigma*}\left( \left[ -\frac{\nabla^2}{2}+V(\vec{r})+\int dr' \frac{\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}-\lambda_{k}^\sigma \right]U(\vec{r})-\int dr' \frac{\rho^\sigma(\vec{r},\vec{r}')}{|\vec{r}-\vec{r}'|}U(\vec{r}') \right)\tag{4.21}. $$
Each term in the sum is zero so
$$\int d^{3}r\,U^{*}(\vec{r})\left( \left[ -\frac{\nabla^2}{2}+V(\vec{r})+\int dr' \frac{\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}-\lambda_{k}^\sigma \right]\phi_{k}^\sigma(\vec{r})-\int dr' \frac{\rho^\sigma(\vec{r},\vec{r}')}{|\vec{r}-\vec{r}'|}\phi_{k}^\sigma(\vec{r}') \right)=0\tag{4.22}.$$
This gives $\braket{ U | f }=0$ $\forall$ $U(\vec{r})$ so the backet equals zero. This can be written as $(\dots)=\sum_{n}C_{n}\chi_{n}(\vec{r})$ with $C_{n}=\int dr\,\chi_{n}(\vec{r})(\dots)=0$, this gives
$$\left( -\frac{\nabla^2}{2}+V(\vec{r})+\int d^{3}r' \frac{\rho(\vec{r}')}{|\vec{r}-\vec{r}'|} \right)\phi_{k}^\sigma(\vec{r})-\int d^3r' \frac{\rho^\sigma(\vec{r},\vec{r}')}{|\vec{r}-\vec{r}'|}\phi_{k}^\sigma(\vec{r}')=\lambda_{k}^\sigma \phi_{k}^\sigma(\vec{r})\tag{4.23}. $$
These are the Hartree-Fock equations. If we define the Hartree term
$$V_{H}[\rho](\vec{r})=\int d^{3}r' \frac{\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}\tag{4.24} $$and the Fock term
$$\hat{V}_{X}^\sigma \phi^{\sigma'}(\vec{r})=\begin{cases}
0 & \sigma'\neq {0} \\
-\int d^{3}r' \frac{\rho^{\sigma}(\vec{r},\vec{r}')}{|\vec{r}-\vec{r}'|}\phi^\sigma(\vec{r}') & \sigma'=\sigma
\end{cases}\tag{4.25} $$
modifies the equation to an eigenvalue equation
$$\left( -\frac{\nabla^2}{2}+V(\vec{r})+V_{H}[\rho](\vec{r})+\hat{V}_{X}^\sigma[\rho^\sigma](\vec{r},\vec{r}') \right)\phi_{k}^\sigma(\vec{r})=\lambda_{k}^\sigma \phi_{k}^\sigma.\tag{4.26} $$
