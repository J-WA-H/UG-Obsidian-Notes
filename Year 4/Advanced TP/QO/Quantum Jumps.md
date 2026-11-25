The Lindbald [[Master Equation]] can, in general, be rephrased as
$$\frac{d\rho}{dt}=-\frac{i}{\hbar}[\hat{H}_{eff}\rho-\rho \hat{H}^{\dagger}_{eff}]+\sum_{k}\chi_{k}\hat{C}_{k}\rho \hat{C}_{k}^{\dagger}\tag{21.1}. $$
The effective Hamiltonian incorporates damping dynamics and is in general
$$\hat{H}_{eff}=\hat{H}-i\sum_{k} \frac{\chi_{k}}{2}\hat{C}^{\dagger}_{k}\hat{C}_{k}.\tag{21.2} $$
The $\sum_{k} \chi_{k}\hat{C}_{k}\rho \hat{C}_{k}^{\dagger}$ is a recycling term. If discarded, the solution for $\rho$ would be $\rho(t+\delta t)=e^{ -i\hat{H}_{eff}\delta t/\hbar }\rho(t)e^{ i\hat{H}_{eff}^{\dagger}\delta t/\hbar }$. The recycling term compensates for the decay in the trace of $\rho(t+\delta t)$. For small time increments $\delta t$ we can say that
$$\frac{d\rho}{dt}\approx \frac{{\rho(t+\delta t)-\rho(t)}}{\delta t}\tag{21.3} $$and therefore
$$\rho(t+\delta t)=\rho(t)-\frac{i}{\hbar}[\hat{H}_{eff}\rho(t)-\rho(t)\hat{H}_{eff}^{\dagger}]\delta t+\sum_{k}\chi_{k}\hat{C}_{k}\rho(t)\hat{C}_{k}^{\dagger}\delta t\tag{21.4} .$$
Note that to first order in $\delta t$,
$$\rho(t)-i[\hat{H}_{eff}\rho(t)-\rho(t)\hat{H}_{eff}^{\dagger}]\approx \left( 1-i\hat{H}_{eff} \frac{\delta t}{\hbar} \right)\rho(t)\left( 1+\hat{H}_{eff}^{\dagger} \frac{\delta t}{\hbar} \right)=e^{ -i\hat{H}_{eff} \delta t/\hbar }\rho(t)e^{ i\hat{H}_{eff}^{\dagger}\delta t/\hbar }.\tag{21.5} $$
This gives
$$\rho(t+\delta t)\approx e^{ -i\hat{H}_{eff}\delta t/\hbar}\rho(t)e^{ i\hat{H}_{eff}^{\dagger}\delta t/\hbar }+\sum_{k}\chi_{k}\hat{C}_{k}\rho(t)\hat{C}_{k}^{\dagger}\delta t.\tag{21.6} $$
Consider an initial pure state $\ket{\psi}$. The likelihood for a jump event to occur before the time $\delta t$ has elapsed in general is
$$\Delta P=\sum_{k}\chi_{k}\bra{\psi} \hat{C}_{k}^{\dagger}\hat{C}_{k}\ket{\psi}\delta t\tag{21.7}.  $$For [[Github/Year 4/Advanced TP/QO/Spontaneous Emission|Spontaneous Emission]], $$\Delta P=\Gamma \bra{\psi} \hat{\sigma}^{+}\hat{\sigma}^{-}\ket{\psi}\delta t=\Gamma \braket{ \psi | e } \braket{ e | \psi } \delta t=\Gamma |\braket{ e | \psi } |^2\tag{21.8}.  $$
For cavity decay,
$$\Delta P=\kappa \bra{\psi} \hat{a}^{\dagger}\hat{a}\ket{\psi} \delta t=\kappa \sum_{n=1}^{\infty}n|\braket{ n | \psi } |^2\tag{21.9}. $$
Consider an initial pure state $\ket{\psi(t)}$. If there is a jump $\hat{C}_{k}$ within $\delta t$, the resulting state $\propto \hat{C}_{k}\ket{\psi(t)}$, or as a density operator $\propto \hat{C}_{k}\ket{\psi}\bra{\psi}\hat{C}_{k}^{\dagger}$. The exact jump is, in general, unspecified.

In general, $$\ket{\psi_{J}(t+\delta t)}\bra{\psi_{J}(t+\delta t)} = \frac{\sum_{k}\chi_{k}\hat{C}_{k}\ket{\psi(t)}\bra{\psi(t)}\hat{C}_{k}^{\dagger}}{\sum_{k}\chi_{k}\bra{\psi(t)}\hat{C}_{k}^{\dagger}\hat{C}_{k}\ket{\psi(t)}  }=\frac{\sum_{k}\chi_{k}\bra{\psi(t)}\hat{C}_{k}^{\dagger}\hat{C}_{k}\ket{\psi(t)} }{\Delta P}\tag{21.10}.   $$
We can reformulate the recycling term to
$$\sum_{k}\chi_{k}\hat{C}_{k}\rho(t)\hat{C}_{k}^{\dagger}=\Delta P\rho_{J}(t+\delta t)\tag{21.11} .$$For no jumps to occur, we need an evolution that is described by $\hat{H}_{eff}$, but the state must be normalised. To linear order in $\delta t$,
$$\ket{\psi'(t+\delta t)} =\left( 1-i \frac{\hat{H}_{eff}\delta t}{\hbar} \right)\ket{\psi(t)} \braket{ \psi'(t+\delta t) | \psi(t+\delta t) }=1-\sum_{k}\chi_{k}\bra{\psi} \hat{C}_{k}^{\dagger}\hat{C}_{k}\ket{\psi(t)} \delta t=1-\Delta P.\tag{21.12}  $$
To linear order in $\delta t$,
$$\ket{\psi_{N}(t+\delta t)} \bra{\psi_{N}(t+\delta t)} = \frac{{\left( 1-i \frac{\hat{H}_{eff}\delta t}{\hbar} \right)\ket{\psi(t)} \bra{\psi(t)} \left( 1+i \frac{\hat{H}_{eff}^{\dagger}\delta t}{\hbar} \right)}}{1-\Delta P}.\tag{21.13} $$We can reformulate the non-recycling terms,
$$e^{ -i\hat{H}_{eff}\delta t/\hbar }\rho(t)e^{ i\hat{H}_{eff}^{\dagger}\delta t/\hbar }=(1-\Delta P)\rho_{N}(t+\delta t).\tag{21.14} $$
Adding the jump and non jump results gives
$$\rho(t+\delta t)=(1-\Delta P)\rho_{N}(t+\delta t)+\Delta P\rho_{J}(t+\delta t)\tag{21.15}. $$This is a probabilistic sum of no jump and jump possibilities. We can statistically approximate the density operator evolution through averaging over multiple quantum trajectories.

The evolution can be determined through quantum Monte-Carlo methods:
- Take initial wavefunction $\ket{\psi(t)}$
- Propagate via $\ket{\psi'(t+\delta t)}=e^{ -i\hat{H}_{eff}\delta t/\hbar }\ket{\psi(t)}$
- Time interval $\delta t$ is so small so no more than one jump event should occur, hence typically
$$\ket{\psi'(t+\delta t)} =\left( 1-i \frac{\hat{H}_{eff}\delta t}{\hbar} \right)\ket{\psi(t)} .\tag{21.16} $$
- Choose a random number $r$ between 0 and 1
- If $r>\braket{ \psi'(t+\delta t) | \psi'(t+\delta t) }=1-\Delta P$ a jump occurs, and
$$\ket{\psi(t+\delta t)}=\frac{\hat{C}\ket{\psi(t)}}{\sqrt{ \bra{\psi(t)} \hat{C}^{\dagger}\hat{C}\ket{\psi(t)}  } } \tag{21.17}. $$
- If $r< 1-\Delta P$ then no jump occurs, and
$$\ket{\psi(t+\delta t)} =\frac{\ket{\psi'(t+\delta t)}}{\sqrt{ \braket{ \psi'(t+\delta t) | \psi'(t+\delta t) }  }}\tag{21.18} .$$
This process is then repeated to generate $\ket{\psi(t+2\delta t)}, \ket{\psi(t+3\delta t)}, \ket{\psi(t+4\delta t)},\dots$, producing a quantum trajectory. Average over a number $N$ of quantum trajectories $j$ is
$$\rho(n\delta t)=\frac{1}{N}\sum_{j=1}^{N}\ket{\psi_{j}(n\delta t)}\bra{\psi_{j}(n\delta t)} .\tag{21.19}  $$
The statistical approximation of the density operator is propagated by the master equation.