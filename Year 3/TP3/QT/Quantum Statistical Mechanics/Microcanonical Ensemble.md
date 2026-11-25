Consider a closed system where for each system there is a fixed number of particles, $N$, fixed volume $V$ and energy $E$ that lives in a small range $E_{0}\leq E\leq E_{0}+\Delta$ where $\Delta$ is small.

Definition: $\Gamma$ is the total number of distinct [pure states](Pure%20and%20Mixed%20States.md) in which a member of the ensemble can be found.
$$\Gamma=\Gamma(N,V,E_{0},\Delta).$$
Fundamental Postulates:
1. There is an equal probability of finding the system in any state of these states
	$$\rho_{nn}=\begin{cases}
\frac{1}{\Gamma} & E_{0}\leq E\leq E_{0}+\Delta \\
0 & \text{Otherwise}
\end{cases}.$$

2. Assume members of the ensemble don't interact $\implies$ wavefunctions don't interfere - it can be achieved if the phases $c_{n}^{\alpha}$ are randomly distributed.

Entropy is given by
$$S=k_{B}\ln\Gamma.$$
This is the same as [thermodynamic entropy](Boltzmann%20Entropy.md) but $\Gamma$ is calculated using quantum mechanics.

If each subsystem is in the same state, $\Gamma=1\implies S=0$ - system is perfectly ordered.
For $\Gamma>1$, the system becomes disordered.

Properties of Entropy:
- Entropy of a closed system is maximal when the system is in equilibrium
- Additive - splitting the system into two, the total energy is the sum of the entropies of the subsystems, $S=S_{1}+S_{2}$.
- Temperature
	$$\frac{1}{T}=\frac{dS}{dE}.$$
The microcanonical ensemble is difficult to use so other ensembles need to be defined.
