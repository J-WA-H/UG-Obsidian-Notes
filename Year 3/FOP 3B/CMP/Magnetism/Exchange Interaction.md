Consider two particles in a box with single particle wavefunctions $\phi_{\alpha},\phi_{\beta}$, where $\alpha,\beta$ are two quantum states.
![[Pasted image 20250130112355.png]]
Trial the wave $\psi(\underline{r}_{1},\underline{r}_{2})=\phi_{\alpha}(\underline{r}_{1})\phi_{\beta}(\underline{r}_{2})$.
Two particles are [indistinguishable](Basic%20Ideas,%20Probability%20and%20Distributions.md) if $|\psi (\underline{r}_{1},\underline{r}_{2})|^2=|\psi(\underline{r}_{2},\underline{r}_{1})|^2$, symmetric under exchange.
As $|\phi_{\alpha}(\underline{r}_{1})\phi_{\beta}(\underline{r}_{2})|^2 \neq|\phi_{\alpha}(\underline{r}_{2})\phi_{\beta}(\underline{r}_{1})|^2$, this is the wavefunction for distinguishable particles, so to model indistinguishable particles, a new wavefunction is needed.

Consider alternate solutions:
$$\psi_{s}(\underline{r}_{1},\underline{r}_{2})=\frac{1}{\sqrt{ 2 }}[\phi_{\alpha}(\underline{r}_{1})\phi_{\beta}(\underline{r}_{2})+\phi_{\alpha}(\underline{r}_{2})\phi_{\beta}(\underline{r}_{1})]$$
$\psi_{s}(\underline{r}_{1},\underline{r}_{2})=\psi_{s}(\underline{r}_{2},\underline{r}_{1})$ so this is a symmetric solution and $|\psi_{s}(\underline{r}_{1},\underline{r}_{2})|^2=|\psi_{s}(\underline{r}_{2},\underline{r}_{1})|^2$ so this wavefunction is for indistinguishable particles.
$$\psi_{a}(\underline{r}_{1},\underline{r}_{2})=\frac{1}{\sqrt{ 2 }}[\phi_{\alpha}(\underline{r}_{1})\phi_{\beta}(\underline{r}_{2})-\phi_{\alpha}(\underline{r}_{2})\phi_{\beta}(\underline{r}_{1})]$$
$\psi_{a}(\underline{r}_{1},\underline{r}_{2})=-\psi_{a}(\underline{r}_{2},\underline{r}_{1})$ so this is an antisymmetric solution and $|\psi_{a}(\underline{r}_{1},\underline{r}_{2})|^2=|\psi_{a}(\underline{r}_{2},\underline{r}_{1})|^2$ so this is a wavefunction for indistinguishable particles.

These wavefunctions define the Pauli-exclusion principle.
In its strong form - the total electron wavefunction must be antisymmetric.
In its weak form - no two electrons have the same quantum state, $\psi_{s}=0$ if $\alpha=\beta$.

If we include spin, the total wavefunction becomes $\psi_{T}=\psi(\underline{r}_{1},\underline{r}_{2})\chi$, which needs to be antisymmetric.

Let $\chi$ be symmetric: $\uparrow\uparrow$, $S=s_{1}+s_{2}=\frac{1}{2}+\frac{1}{2}=1\implies m_{s}=-1,0,1$. As there are three $m_{s}$ values this is the triplet.
In this case $\psi=\psi_{a}$ but $\psi_{a}(\underline{r}_{1},\underline{r}_{2})=-\psi_{a}(\underline{r}_{2},\underline{r}_{1})$ so if $\underline{r}_{1}=\underline{r}_{2}, \psi_{a}=0\implies$ electrons cannot be close together.

Now consider when $\chi$ is antisymmetric: $\uparrow\downarrow$, $S=s_{1}+s_{2}=\frac{1}{2}-\frac{1}{2}=0\implies m_{s}=0$. As there is only a single $m_{s}$ value, this is the singlet state.
In this case $\psi=\psi_{s}$ but $\psi_{s}(\underline{r}_{1},\underline{r}_{2})=\psi_{s}(\underline{r}_{2},\underline{r}_{1})$ so if $\underline{r}_{1}=\underline{r}_{2}$, $\psi_{s}\neq 0$ so the electrons can be close.

The exchange energy is given by
$$E=-J\underline{s}_{1}\cdot \underline{s}_{2}$$
where $J$ is the exchange constant.
If $J>0$, parallel spins minimise energy so the triplet is favoured, so exchange energy tries to align spins.
If $J<0$, antiparallel spins minimise energy so the singlet is favoured so the exchange energy tries to anti align spins.

Examples:
For $J>0$, from [Hund's rules](Angular%20Momentum%20in%20QM.md) an atom maximises $S$ so the triplet is favoured.
For $J<0$, a diatomic molecule bound by a covalent bond and has opposite spins
![[Pasted image 20250130123556.png]]
