Consider a [semiconductor](Band%20Gaps%20in%20Semiconductors.md) at $T>0\text{ K}$, the electron concentration in the conduction band is $n$ and the hole concentration is $p$.
![[Pasted image 20250213145259.png]]
An intrinsic semiconductor has $n=p=n_{i}$, where $n_i$ is the intrinsic carrier concentration. Assuming a semiconductor is in equilibrium, so it in the lowest energy state.

The concentrations are given by the electron density of states, $g_e(E)$ and the [[Fermi-Dirac Distribution]], as electrons are fermions.
$$n=\int_{CB}f_{FD}(E)g_{e}(E)dE$$
$$p=\int_{VB}(1-f_{FD}(E))g_{h}(E)dE.$$
The hole concentration has $1-f_{FD}(E)$ as this is the probability of an unoccupied state.

From [[Free-Electron Theory]], the density of states is
$$g_{E}(E)=\frac{1}{2\pi^2}\left( \frac{2m_{e}}{\hbar^2} \right)^{3/2}\sqrt{ E }.$$
Adjusting this for the valence and conduction band gives
$$g_{e}(E)=\frac{1}{2\pi^2}\left( \frac{2m_{e}^{*}}{\hbar^2} \right)^{3/2}\sqrt{ E-E_{c} }$$
$$g_{h}(E)=\frac{1}{2\pi^2}\left( \frac{2m_{h}^{*}}{\hbar^2} \right)^{3/2}\sqrt{ E_{V}-E }.$$
For $n$, take the limits between $E_{C}$ and $E_V$,
![[Pasted image 20250213150844.png]]
$$\therefore n=\int_{E_{C}}^{E_{T}} \frac{1}{1+\exp\left[ \frac{{E-\mu}}{k_{B}T} \right]}\left[ \frac{1}{2\pi^2}\left( \frac{2m_{e}^{*}}{\hbar^2} \right)^{3/2}\sqrt{ E-E_{C} } \right]dE.$$
To evaluate this, some assumptions have to be made:
1. $E_{T}\to \infty$ so FD vanishes fast
2. $E_{C}-\mu\gg k_{B}T$ so $\exp\left[ \frac{{E-\mu}}{k_{B}T} \right]\gg 1$ so the 1 in the denominator can be ignored.

Bringing all the constants to the front give
$$n=A\int_{E_{C}}^{\infty}\exp\left[ -\frac{{E-\mu}}{k_{B}T} \right]\sqrt{ E-E_{C} }dE$$
Evaluating this gives
$$n=N_{C}\exp\left[ -\frac{E_{C}-\mu}{k_{B}T} \right].$$
$$N_{C}=2\left( \frac{m^{*}_{e}k_{B}T}{2\pi \hbar^2} \right)^{3/2},$$
this is the conduction band effective density of states.

For the hole concentration is can be shown that
$$p=N_{V}\exp\left[ -\frac{{\mu-E_{V}}}{k_{B}T} \right]$$
where
$$N_{V}=2\left(\frac{m_{h}^{*}k_{B}T}{2\pi \hbar^2}\right)^{3/2}$$
is the valance band effective density of states.

Considering when $n=p$,
$$N_{C}\exp\left[ -\frac{E_{C}-\mu}{k_{B}T} \right]=N_{V}\exp\left[ -\frac{\mu-E_{V}}{k_{B}T} \right]$$
$$\implies \mu=\frac{E_{C}+E_{V}}{2}+\frac{1}{2}k_{B}T\ln\left( \frac{N_{V}}{N_{C}} \right).$$
We know that $N_{V}\propto(m_{h}^{*})^{3/2}$ and $N_{C}\propto(m_{e}^{*})^{3/2}$.
If $m^{*}_{e}\approx m_{h}^{*}$ then $\ln\left[ \frac{N_{V}}{N_{C}} \right]\approx 0$ so
$$\mu=\frac{E_{C}+E_{V}}{2}.$$
The chemical potential is in the middle of the band gap.

The law of mass action defines the product between $n$ and $p$.
$$np=N_{C}\exp\left[ -\frac{E_{C}-\mu}{k_{B}T} \right]N_{V}\exp\left[ -\frac{{\mu-E_{V}}}{k_{B}T} \right]$$
$$\implies np=N_{C}N_{V}\exp\left[ -\frac{E_{C}-E_{V}}{k_{B}T} \right]$$
using the band gap $E_{g}=E_{C}-E_{V}$,
$$np=N_{C}N_{V}\exp\left[ -\frac{E_{g}}{k_{B}T} \right].$$
For an intrinsic semiconductor, $n=p=n_{i}$,
$$n_{i}=\sqrt{ N_{C}N_{V} }\exp\left[ -\frac{E_{g}}{k_{B}T} \right].$$
We also know $\sqrt{ N_{V}N_{C} }\propto T^{3/2}$ but the exponential dependence dominates, so as $T$ increases, $n_{i}$ increases rapidly.

All this can be used to define electrical conductivity. Using [drift velocity](Holes%20in%20Semiconductors.md),
$$J=-ne(\underline{v}_{d})_{e}+pe(\underline{v}_{d})_{h}.$$
For an intrinsic semiconductor, $n=p=n_{i}$ and
$$(\underline{v}_{d})_{e}=-\mu_{e}\underline{E}$$
$$(\underline{v}_{d})_{h}=\mu_{h}\underline{E}$$
where $\mu_{e},\mu_{h}$ are the electron and hole mobilities respectively. 
$$\therefore\underline{J}=[n_{i}e(\mu_{e}+\mu_{h})]\underline{E}.$$
Conductivity is defined as 
$$\sigma=n_{i}e(\mu_{e}+\mu_{j})$$
so
$$\underline{J}=\sigma \underline{E}.$$
This is Ohm's law.

For a semiconductor, as $T$ increases, $n_{i}$ rapidly increases so $\mu$ decreases so $\sigma$ increases with $T$.
For a metal, as T increases, $n$ remains approximately constant so $\mu$ decreases so $\sigma$ decreases with $T$.