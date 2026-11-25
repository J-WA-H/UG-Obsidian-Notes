Invoke a fictitious system of electrons, not interacting, with the same density $\rho(\vec{r})$ as the interacting system. In order that the Kohn-Sham system has density $\rho(\vec{r})$ it must be bound by an appropriate local potential $V_{s}[\rho](\vec{r})$.

The single particle equations for the Kohn-Sham system is
$$\left( -\frac{\nabla^2}{2}+V_{s}[\rho](\vec{r}) \right)\phi_{i}(\vec{r})=\varepsilon_{i}\phi_{i}(\vec{r})\tag{10.1},$$
$$\rho(\vec{r})=\sum_{\sigma}\sum_{i=1}^{N^\sigma}|\phi_{i}^\sigma(\vec{r})|^2\tag{10.2} ,$$
$$T_{s}[\rho]=-\frac{1}{2}\sum_{\sigma}\sum_{i=1}^{N}\int d^3r\phi ^{\sigma*}_{i}(\vec{r})\nabla^2\phi^\sigma_{i}(\vec{r})\tag{10.3}.$$
Using the slater determinant for a Kohn-Sham electron $\Phi_{s}[\rho]$, $$F[\rho]\to\bra{\Phi_{s}[\rho]} T\ket{\Phi_{s}[\phi]} =T_{s}[\rho]=\mathrm{min}\bra{\phi } T\ket{\phi} \;\forall\;\phi \leftrightarrow \rho=\sum_{\sigma}\sum_{i=1}^{N^\sigma}\bra{\phi_{i}^\sigma}-\frac{\nabla^2}{2}\ket{\psi_{i}^\sigma}  .\tag{10.4} $$
This kinetic energy functional an approximate the [[Internal Energy Density Functional]] since electron-electron interactions are ignored.

This gives the basic equation of Kohn-Sham DFT,
$$\frac{\delta T_{s}[\rho]}{\delta \rho(\vec{r})}+V_{s}[\rho](\vec{r})-\text{const}=0.\tag{10.5} $$
A correction is needed to obtain an accurate equation
$$F[\rho]=T_{s}[\rho]+\frac{1}{2}\iint d^3rd^3r' \frac{\rho(\vec{r})\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}+E_{XC}[\rho]\tag{10.6} .$$
Now $F[\rho]=T_{s}[\rho]+U[\rho]+E_{XC}[\rho]$ and $\frac{\delta E_{XC}[\rho]}{\delta \rho(\vec{r})}=V_{XC}[\rho](\vec{r})$. The basic equation of [[Density Functional Theorem]] gives
$$\frac{\delta T_{s}[\rho]}{\delta \rho(\vec{r})}+V_{H}[\rho](\vec{r})+V_{XC}[\rho](\vec{r})+V_{ext}(\vec{r})-\mu=0.\tag{10.7} $$
Using $(10.5)$,
$$V_{s}[\rho](\vec{r})=V_{ext}(\vec{r})+V_{H}[\rho](\vec{r})+V_{XC}[\rho](\vec{r})+\text{const.}\tag{10.8} $$Using this with $(10.1-10.2)$ can obtain the density of the system. Use a trial density to solve for $V_{s}[\rho]$, then use this to find $\phi_{i}^\sigma$, then update $\rho(\vec{r})$ and repeat until it converges.

An alternative method to solve for the system uses the variational principle,
$$E_{V_{ext}}[\rho]=F[\rho]+\int d^3rV_{ext}(\vec{r})\rho(\vec{r})\geq E_{0}\tag{10.9} $$becomes a functional of KS orbitals
$$E_{V_{ext}}[\{ \phi_{i}^\sigma(\vec{r}) \}]=-\frac{1}{2}\sum_{\sigma}\sum_{i=1}^{N^\sigma}\int d^3r\phi_{i}^{\sigma*}(\vec{r})\nabla^2\phi_{i}^{\sigma}(\vec{r})+\int d^3rV_{ext}(\vec{r})\rho(\vec{r})+\iint d^3rd^3r' \frac{\rho(\vec{r})\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}+E_{XC}[\rho](\vec{r}).\tag{10.10} $$

The simplest approximation is the local density approximation (LDA). Like the TF and TFD theory, this treats the density of an electronic system as locally homogeneous and then employ the XC energy as it is calculated numerically accurately with Quantum Monte Carlo methods from [[Jellium]].

The total XC energy, using the approximation that $\rho=\frac{N}{V}$ is
$$E_{XC}[\rho]=N\varepsilon_{XC}[\rho]\tag{10.11} .$$This then gives
$$E_{XC}^{LDA}[\rho]=\int d^3r\rho(\vec{r})\varepsilon_{XC}(\rho(\vec{r})).\tag{10.12} $$
