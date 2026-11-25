For spontaneous emission, we assume a continuum of modes,
$$\hat{\vec{E}}=i\sum_{s}\int d^3k \sqrt{ \frac{\hbar ck}{16\varepsilon_{0}\pi^3} }[\vec{e}_{s}(\vec{k})\hat{a}_{s}(\vec{k})e^{ i\vec{k}\cdot \vec{r} }+\text{H.c.}]\tag{19.1} .$$
The complex $\vec{e}_{s}(\vec{k})$ vector generalises the polarisation basis to, for example, left and right circular.
Here the commutation relation between the [[Creation and Annihilation Operators]] are
$$[\hat{a}_{s}(\vec{k}),\hat{a}^{\dagger}_{s}(\vec{k}')]=\delta^{(3)}(\vec{k}-\vec{k}')\delta_{ss'}.\tag{19.2} $$
Consider a two-level atom (the system),
$$\hat{H}_{A}=\frac{\hbar\omega_{eg}}{2}\hat{\sigma}_{z}.\tag{19.3} $$
the quantised electric field (bath),
$$\hat{H}_{F}=\sum_{s}\int d^3k \;\hbar ck\hat{a}^{\dagger}_{s}(\vec{k})\hat{a}_{s}(\vec{k}).\tag{19.4} $$
The total Hamiltonian is then $\hat{H}=\hat{H}_{A}+\hat{H}_{F}+\hat{H}_{C}$ where
$$\hat{H}_{C}=\sum_{s}\int d^3k\;\hbar[\kappa_{s}(\vec{k})\hat{a}_{s}(\vec{k})\hat{\sigma}^{+}+\text{H.c}]\tag{19.5}. $$
This assumes the [rotating wave](Atom-Field%20Interactions.md) and dipole approximations.
The dipole coupling is given by
$$\kappa_{s}(\vec{k})=-ie^{ i\vec{k}\cdot \vec{r}_{A} }\sqrt{ \frac{ck}{16\hbar \varepsilon_{0}\pi^3} }\vec{e}_{s}(\vec{k})\cdot \bra{e} \hat{\vec{d}}\ket{e}.\tag{19.6}  $$
Here $\vec{r}_{A}$ is the atomic centre of mass location.

Transform to the interaction picture:
$$\hat{H}_{I}(t)=e^{ i(\hat{H}_{A}+\hat{H}_{F})t/\hbar }\hat{H}_{C}e^{ -i(\hat{H}_{A}+\hat{H}_{F})t/\hbar }\tag{19.7} .$$
$$\hat{H}_{I}(t)=\hbar\hat{\Gamma}^{\dagger}(t)\hat{\sigma}^{-}e^{ -i\omega_{eg}t }+\text{H.c.}\tag{19.8} $$
where
$$\hat{\Gamma}(t)=\sum_{s}\int d^3k\;\kappa_{s}(\vec{k})\hat{a}_{s}(\vec{k})e^{ -ickt }.\tag{19.9} $$
In the interaction picture, the density operator is
$$\tilde{\rho}(t)=e^{ i(\hat{H}_{A}+\hat{H}_{F})t/\hbar }\rho(t)e^{ -i(\hat{H}_{A}+\hat{H}_{F})t/\hbar }.\tag{19.10} $$
From the Von-Neumann equations,
$$\frac{d\tilde{\rho}}{dt}=-\frac{i}{\hbar}[\hat{H}_{I}(t),\tilde{\rho}(t)].\tag{19.11} $$
Integrating this gives
$$\tilde{\rho}(t)=\tilde{\rho}(0)-\frac{i}{\hbar}\int_{0}^{t}dt'[\hat{H}_{I}(t),\tilde{\rho}(t)]\tag{19.12} $$
Substituting this back into the Von-Neumann equation gives
$$\frac{d\tilde{\rho}}{dt}=-\frac{i}{\hbar}[\hat{H}_{I}(t),\tilde{\rho}(0)]-\frac{1}{\hbar^2}\int_{0}^{t}dt'\left[\hat{H}_{I}(t),[\hat{H}_{I}(t'),\tilde{\rho}(t')]\right].\tag{19.13} $$
Assume that at $t=0$, the density operator factorises into atom and field density operators. Assume the field is initially in a temperature $T$ thermal state,
$$\rho(0)=\rho_{A}(0)\rho_{F}(T).\tag{19.14} $$
The thermal field state is diagonal in the number basis so $\mathrm{Tr}_{F}(\hat{a}_{S}(\vec{k})\rho_{F}(T))=0$. Hence, $\mathrm{Tr}_{F}(\hat{H}_{I}(t)\tilde{\rho}(0))=0$ and defining the interaction picture reduced density operator $\tilde{\rho}_{R}(t)=\mathrm{Tr}(\tilde{\rho}(t))$, we get
$$\frac{d\tilde{\rho}}{dt}=-\frac{1}{\hbar^2}\int_{0}^{t}dt'\mathrm{Tr}_{F}([\hat{H}_{I}(t),[\hat{H}_{I}(t'),\tilde{\rho}(t')]]).\tag{19.15} $$
For the Born approximation, we approximate the field driving the atom by the field as it would be in the absence of the atom. Replace $\tilde{\rho}(t')$ within the integral over $t$ by $\tilde{\rho}_{R}(t')\rho_{F}(T)$. The field's effect on the atom is important, but the atom's effect on the field is negligible. 

For the Markov approximation, replace $\tilde{\rho}_{R}(t')$ within $\tilde{\rho}(t')\approx \tilde{\rho}_{R}(t')\rho_{F}(T)$ by $\tilde{\rho}_{R}(t)$,
$$\frac{d\tilde{\rho}_{R}}{dt}=-\frac{1}{\hbar^2}\int_{0}^{t}dt'\mathrm{Tr}([\hat{H}_{I}(t),[\hat{H}_{I}(t'),\tilde{\rho}_{R}(t)\rho_{F}(T)]]).\tag{19.16} $$
The differential equation depends on the state of the atom at the current time $t$ only. Earlier atom states in principle affect the field which then later affects the atom back. The Markov approximation assumes no memory in the reservoir/field beyond a very short time.

To get the thermal field expectation values, first note that $\mathrm{Tr}_{F}(\hat{a}_{s}^{\dagger}(\vec{k})\hat{a}_{s'}(\vec{k})\rho_{F}(T))=\delta^{(3)}(\vec{k}-\vec{k}')\delta_{ss'}g(k)N(k,T)$. Here $g(k)$ is the density of states and
$$N(k,T)=\frac{e^{ -\hbar ck/k_{B}T }}{1-e^{ -\hbar ck/k_{B}T }}\tag{19.17} .$$
Setting $\tau=t'-t$, $$\mathrm{Tr}_{F}(\hat{\Gamma}^{\dagger}(t)\hat{\Gamma}(t-\tau)\rho_{F}(T))=\sum_{s}\int d^{3}k\;g(k)|\kappa_{s}(\vec{k})|^2N(k,T)e^{ ick\tau }.\tag{19.18} $$$$\mathrm{Tr}(\hat{\Gamma}(t)\hat{\Gamma}^{\dagger}(t-\tau)\rho_{F}(T))=\sum_{s}\int d^{3}k\;g(k)|\kappa_{s}(\vec{k})|^2[N(k,T)+1]e^{ -ick\tau }.\tag{19.19} $$
The master equation for $\tilde{\rho}_{R}$ is
$$\frac{d\tilde{\rho}_{R}}{dt}=[\hat{\sigma}^{+}\tilde{\rho}_{R}\hat{\sigma}^{-}-\tilde{\rho}_{R}\hat{\sigma}^{-}\hat{\sigma}^{+}]\xi+\text{H.c.}+[\hat{\sigma}^{-}\tilde{\rho}_{R}\hat{\sigma}^{+}-\hat{\sigma}^{+}\hat{\sigma}^{-}\tilde{\rho}_{R}][\xi+\zeta]+\text{H.c.}\tag{19.20} $$where
$$\xi=\sum_{s}\int d^{3}k\;g(k)|\kappa_{s}(\vec{k})|^2N(k,T)\int_{0}^{t}d\tau \;e^{ -i(ck-\omega_{eg})\tau }\tag{19.21} $$$$\zeta=\sum_{s}\int d^{3}k\;g(k)|\kappa_{s}(\vec{k})|^2\int_{0}^{t}d\tau\;e^{ -i(ck-\omega_{eg})\tau }.\tag{19.22} $$
The timescale is given by the time integral in $(19.21-22)$. Markov assumes a timescale of changes to the atom state much longer than those of the bath/field. Shorter timescales dominate the integral over $\tau$.
Hence, the extended integral to infinity is
$$\lim_{ t \to \infty } \int_{0}^{t}d\tau\;e^{ -i(ck-\omega_{eg})\tau }=\pi\delta(ck-\omega_{eg})+i\mathcal{P} \frac{1}{\omega_{eg}-ck}.\tag{19.23} $$The $\mathcal{P}$ indicates the Cauchy principle value.

The principle value terms cause atomic frequency shifts, due to thermal or quantum fluctuations (Lamb shift). While measurable, shifts are very small and are commonly neglected. We will also neglect these terms.

Identify the reduced density operator $\tilde{\rho}_{R}$ with atomic density operator $\tilde{\rho}_{A}$. Define
$$\Gamma=2\pi \sum_{s}\int d^{3}k\;g(k)|\kappa_{s}(\vec{k})|^2\delta(ck-\omega_{eg}).\tag{19.24} $$
The radiatively damped two-level atom master equation is
$$\frac{d\tilde{\rho}_{A}}{dt}=\frac{\Gamma}{2}\left[ N\left( \frac{\omega_{eg}}{c},T \right)+1 \right](2\hat{\sigma}^{-}\tilde{\rho}_{A}\hat{\sigma}^{+}-\tilde{\rho}_{A}\hat{\sigma}^{+}\hat{\sigma}^{-}-\hat{\sigma}^{+}\hat{\sigma}^{-}\tilde{\rho}_{A})+\frac{\Gamma}{2}N\left( \frac{\omega_{eg}}{c},T \right)(2\hat{\sigma}^{+}\tilde{\rho}_{A}\hat{\sigma}^{-}-\tilde{\rho}_{A}\hat{\sigma}^{-}\hat{\sigma}^{+}-\hat{\sigma}^{-}\hat{\sigma}^{+}\tilde{\rho}_{A})\tag{19.25}. $$
If we can consider the radiation field to be in the vacuum state, i.e. $N\left( \frac{\omega_{eg}}{c} \right)=0$,
$$\frac{d\tilde{\rho}_{A}}{dt}=\frac{\Gamma}{2}(2\hat{\sigma}^{-}\tilde{\rho}_{A}\hat{\sigma}^{+}-\tilde{\rho}_{A}\hat{\sigma}^{+}\hat{\sigma}^{-}-\hat{\sigma}^{+}\hat{\sigma}^{-}\tilde{\rho}_{A}).\tag{19.26} $$
This describes spontaneous emission.