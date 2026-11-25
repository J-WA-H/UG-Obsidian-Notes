Consider a system, $S$, in thermal contact with a large reservoir, $R$.
![[Pasted image 20250211183217.png]]
$S+R$ is closed and properties are defined by the [[Microcanonical Ensemble]].

$S$ has a fixed number of particles, $N_S$, volume $V_S$, and energy eigenstate $E_S$. Similarly $R$ has a fixed number of particles $N_{R}$, volume $V_R$, and energy eigenstate $E_R$.

$S$ and $R$ are in thermal contact so can exchange energy, but the interaction is weaker.

At any time $S,R$ are in definite energy eigenstates $E_{R},E_{S}$.
They have common temperature $T$ in equilibrium.
From conservation of energy, $E=E_{S}+E_{R}$ so the whole system is described by the microcanonical ensemble, $E_{0}\leq E\leq E_{0}+\Delta$, assuming $\Delta\ll E_{0}$.

The probability that the system $S$ is in the state with energy $E_{n}$ for a given temperature $T$.
$d\Gamma(E)$ is the number of states of the combined system between $E$ and $E+dE$.
The probability of the whole system being in this state is
$$d\mathbb{P}=\begin{cases}
cd\Gamma(E) & E_{0}\leq E\leq E_{0}+\Delta \\
0 & \text{Otherwise}
\end{cases}$$
where $c$ is a constant probability of finding one state.
$$d\Gamma=d\Gamma_{S}d\Gamma_{R}.$$
$$d\mathbb{P}=cd\Gamma_{S}(E_{S})d\Gamma_{R}(E_{R})\delta(E-E_{S}-E_{R}).$$
The [[Delta Function]] ensures conservation of energy.

We want the probability $S$ gas energy $E_n$ regardless of the state of the reservoir.
$$d\mathbb{P}=cd\Gamma_{S}(E_{n})\int d\Gamma_{R}(E_{R})\delta(E-E_{n}-E_{R})dE_{R}$$
$$=cd\Gamma_{S}(E_{n})\Delta\Gamma_{R}(E-E_{n}).$$
$\Delta\Gamma$ is the total number of states in the reservoir subject to energy conservation.

The energy of the reservoir is $S_{R}=k_{B}\ln\Delta\Gamma_{R}\implies\Delta\Gamma_{R}=\exp\left[ \frac{S_{R}}{k_{B}T} \right]$.
If the system is very small compared to the reservoir, $E_{n}\ll E_{R},E$.
$$S_{R}(E_{R})=S_{R}(E-E_{n})\approx S_{R}(E)-\frac{dS_{R}}{dE}E_{n}+\dots=S_{R}(E)-\frac{E_{n}}{T}.$$
$$\therefore d\mathbb{P}=cd\Gamma_{S}(E_{n})\exp\left[ \frac{S_{R}}{k_{B}}-\frac{E_{n}}{k_{B}T} \right].$$
$\frac{S_{R}}{k_{B}}$ is a constant so absorb it into $c$,
$$d\mathbb{P}=Ae^{-E_{n}/k_{B}T}d\Gamma_{S}(E_{n}).$$
$\therefore$  the probability of the system being in state $E_n$ is $Ae^{-E_{n}/k_{B}T}$
$$\implies \rho_{nm}=Ae^{-E_{n}/k_{B}T}\delta_{nm}.$$

Using the properties of the [[Density Operator]],
$$\mathrm{Tr}(\rho)=1\implies \sum_{n}Ae^{-\beta E_{n}}=1\implies A=\frac{1}{\sum_{n}e^{-\beta E_{n}}}.$$
This gives the partition function,
$$Q_{NS}(T)=\frac{1}{\sum_{n}e^{-\beta E_{n}}}=\mathrm{Tr}(e^{-\beta H}).$$
The sum is over distinct states, not necessarily energy eigenstates.
$$\rho=\frac{1}{Q_{NS}(T)}e^{-\beta H}.$$
The ensemble average of this operator is
$$\langle A \rangle =\mathrm{Tr}(\rho A)=\frac{1}{Q_{NS}}\mathrm{Tr}(e^{-\beta H}A)=\frac{\mathrm{Tr}(e^{-\beta H}A)}{\mathrm{Tr}(e^{-\beta H})}.$$
Example: $\langle H \rangle$.
Consider
$$\frac{dQ_{NS}}{d\beta}=\frac{d}{d\beta}(\mathrm{Tr}(e^{-\beta H}))=-\mathrm{Tr}(e^{-\beta H}H).$$
$$\therefore \langle H \rangle =\frac{\mathrm{Tr}(e^{-\beta H})}{Q_{NS}}=-\frac{1}{Q_{NS}} \frac{dQ_{NS}}{d\beta}=-\frac{d}{d\beta}(\ln Q_{NS}).$$
