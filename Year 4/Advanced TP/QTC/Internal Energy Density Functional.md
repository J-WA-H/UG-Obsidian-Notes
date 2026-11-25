The [functional](Density%20Functional%20Theorem.md) $F[\rho]$ is the internal energy density functional, also known as the universal density functional or the Hohenberg-Kohn density functional. From the Schrodinger equation,
$$H_{V}\psi=E\psi \implies(T+V_{ee}+V)\psi[\rho]=E_{0}\psi[\rho];\;V\leftrightarrow \rho\tag{9.1} $$
$$F[\rho ]=\bra{\psi[\rho]} T+V_{ee}\ket{\psi[\rho]}\underbrace{ =\bra{\psi[\rho]} T\ket{\psi[\rho]} }_{ T[\rho] } +\underbrace{ \bra{\psi[\rho]}V_{ee}\ket{\psi[\rho]} }_{ V_{ee}[\rho] } \tag{9.2}.  $$
This shows the internal energy density functional is the sum of the kinetic energy density functional $T[\rho]$ and the electron-electron repulsion energy density functional $V_{ee}[\rho]$, $F[\rho]=T[\rho]+V_{ee}[\rho]$.

To approximate $F$, we need to approximate $T[\rho]$ and $V_{ee}[\rho]$. The main assumption is that $\rho$ is obtained from $\delta E$, i.e. $\rho$ is the ground state density of a local $V(\vec{r})$. This is not always true. A more general definition for all $\rho$ is $F[\rho]=\mathrm{min}[\bra{\psi}T+V_{ee}\ket{\psi}]$ $\forall$ $\psi \leftrightarrow \rho$.

Minimising the state $\psi[\rho]$ also satisfies $(T+V_{ee}+V_{ex})\psi[\rho]=E\psi[\rho]$ for an excited state potential.

We can approximate $F[\rho]$ using the uniform electron gas [[Jellium]],
$$E_{kin}=\frac{3V}{10}\rho k_{F}^2=\frac{3V}{10}(3\pi^2)^{2/3}\rho^{5/3}.\tag{9.3} $$To go from a uniform to a weakly varying density,
$$V\to \int d^3r,\;\rho\to \rho(\vec{r}),\;N=\rho V\to \int d^3r\rho(\vec{r})\tag{9.4}. $$
This gives
$$E_{kin}=\frac{3}{10}\int d^3r(3\pi)^{2/3}\rho^{5/3}(\vec{r})\implies T^{TF}[\rho]=\frac{3}{10}(3\pi^2)^{2/3}\int d^3r\rho^{5/3}(\vec{r})\tag{9.5}. $$
This is the Thomas-Fermi kinetic energy.
$$V_{ee}\to \frac{1}{2}\int \frac{d^3rd^3r'}{|\vec{r}-\vec{r}'|}\rho(\vec{r})\rho(\vec{r}')=U\tag{9.6} $$is the Hartree-Coulomb energy. The exchange energy is
$$E_{X}=-\frac{3Nk_{F}}{4\pi}\to E_{X}[\rho]=-\frac{3}{4\pi}\int d^{3}r\rho(\vec{r})(3\pi^2)^{1/3}\rho^{1/3}(\vec{r})\tag{9.7} =-\frac{3}{4}\left( \frac{3}{\pi} \right)^{1/3}\int d^{3}r\rho^{4/3}(\vec{r}).$$
The inclusion of the exchange energy is the Thomas-Fermi-Dirac model.
$$F^{TFD}[\rho]=\frac{3}{10}(3\pi)^{2/3}\int d^3r \rho^{5/3}(\vec{r})+\frac{1}{2}\iint \frac{d^3rd^3r'}{|\vec{r}-\vec{r}'|}\rho(\vec{r})\rho(\vec{r}')-\frac{3}{4}\left( \frac{3}{\pi} \right)^{1/3}\int d^3r\rho^{4/3}(\vec{r}).\tag{9.8} $$
This is a self-consistent solution of the TFD equations.
$$E_{V_{ext}}[\rho]=F^{TFD}[\rho]+\int d^3rV_{ext}(\vec{r})\rho(\vec{r})-\mu \int d^3r\rho(\vec{r})\tag{9.9}. $$
Minimising this gives
$$\frac{1}{2}(3\pi^2)^{2/3}\rho_{0}^{2/3}(\vec{r})+V_{H}[\rho_{0}](\vec{r})+V_{X}^{LDA}[\rho_{0}](\vec{r})+V_{ext}(\vec{r})-\mu=0\tag{9.10} $$
where
$$V_{H}[\rho_{0}](\vec{r})=\left.\frac{\delta U}{\delta \rho(\vec{r})}\right|_{\rho_{0}}=\int \frac{d^3r'\rho(\vec{r}')}{|\vec{r}-\vec{r}'|};\;V_{X}^{LDA}[\rho_{0}](\vec{r})=\left. \frac{\delta E_{X}}{\delta \rho(\vec{r})} \right|_{\rho_{0}}=-\left( \frac{3}{\pi} \right)\rho^{1/3}(\vec{r}).\tag{9.11} $$Solving this gives
$$\rho_{0}(\vec{r})=-\frac{2}{(3\pi^2)^{2/3}}[V_{H}[\rho_{0}](\vec{r})+V_{X}^{LDA}[\rho_{0}](\vec{r})+V_{ext}(\vec{r})-\mu]^{3/2}.\tag{9.12}$$
We find that this is not accurate due to to $\frac{\delta T^{TF}}{\delta \rho}$ as it does not take into account Pauli exclusion, so the solutions are bosonic.