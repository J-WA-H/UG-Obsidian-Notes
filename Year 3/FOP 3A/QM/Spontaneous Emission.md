Spontaneous emission puts electrons in thermal equilibrium in a photon gas, so the number of particles in each state must be constant.![[Pasted image 20241108182920.png]]
Because the system is in thermal equilibrium, the number of atoms leaving state b must be the same as the number of atoms entering state b.
$$N_{a}R_{b\to a}=N_{b}(A+R_{b\to a}).$$
Using the rate for [[Stimulated Emissions]]:
$$N_{a}B\rho(\omega_{0})=N_{b}(A+B\rho(\omega_{0}))\implies A=\left( \frac{N_{a}}{N_{b}} -1\right)B\rho(\omega_{0}).$$
$$\implies \rho(\omega_{0})=\frac{A}{B} \frac{1}{\left( \frac{N_{a}}{N_{b}} \right)-1}.$$
Using results from [statistical mechanics](Partition%20Function.md), $N_a\propto\exp\left( -\frac{E_{a}}{k_{B}T} \right)$ so
$$\frac{N_{a}}{N_{b}}=e^{-(E_{a}-E_{b})/k_{B}T}=e^{\hbar \omega_{0}/k_{B}T}.$$
Since we know
$$\rho(\omega_{0})=\frac{{\hbar \omega_{0}^3}}{\pi^2 c^3} \frac{1}{\exp(\hbar \omega_{0}/k_{B}T)-1}\implies \frac{A}{B}=\frac{{\hbar \omega_{0}^3}}{\pi^2c^3}.$$
Since $B=\frac{{\pi \lvert p \rvert^2}}{3\varepsilon_{0}\hbar^2}$, this gives the rate of spontaneous emission
$$A=\frac{{\lvert p \rvert^2\omega_{0} }}{3\pi c^3\hbar\varepsilon_{0}}.$$
At $T=0K$, $\rho(\omega_{0})=0$ so spontaneous emission is the only process that occurs.

Only considering spontaneous emission:
$$dN_{b}=-N_{b}Adt\implies N_{b}(t)=N_{b}(0)e^{-At}.$$
The lifetime of this excited state is defined to be the time, $\tau$, for the population in $b$ to reach $\frac{1}{e}$ of its initial value:
$$\tau=\frac{1}{e}.$$
