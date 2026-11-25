A ferromagnet is a material where all spins are aligned.
Including the [[Exchange Interaction]], the [magnetic Hamiltonian](Angular%20Momentum%20in%20QM.md), ignoring the weak diamagnetic term, becomes
$$\hat{H}_{mag}=\sum_{i,j}-J_{ij}\underline{s}_{i}\cdot \underline{s}_{j}+\sum_{i}\gamma g_{J}\underline{B}\cdot \underline{J}_{i}.$$
The exchange energy term is not easy to calculate.

For the Weiss model, define the molecular B field as
$$\underline{B}_{mf}=\frac{1}{\gamma g_{J}}\sum_{j}-J_{ij}\underline{s}_{j}.$$
This is not strictly a B-field, it comes from the exchange interpretation between atoms.
$$\therefore\hat{H}_{mag}=\sum_{i}\gamma g_{J}\underline{B}_{mf}\cdot \underline{s}_{i}+\sum_{i}\gamma g_{J}\underline{B}\cdot \underline{J}_{i}.$$
Assume $\underline{L}_{i}=0$ then $\underline{J}_{i}=\underline{s}_{i}$
$$\therefore \hat{H}_{mag}=\sum_{i}\gamma g_{J}(\underline{B}+\underline{B}_{mf})\cdot \underline{J}_{i}.$$
Say $\underline{B}_{mf}=\lambda \underline{M}$, where $\lambda$ is a constant that depends on the exchange interaction.
$$\hat{H}_{mag}=\sum_{i}\gamma g_{J}(\underline{B}+\lambda \underline{M})\cdot \underline{J}_{i}.$$
This is similar to the [paramagnetic](Paramagnetism.md) term.
Using the paramagnetic results,
$$\frac{M}{M_{s}}=B_{J}(y);\;y=\frac{g_{J}\mu_{B}JB}{k_{B}T}.$$
For ferromagnets,
$$y=\frac{g_{J}\mu_{B}J}{k_{B}T}(B+\lambda M).$$
For zero B-field:
$$\frac{M}{M_{s}}=B_{J}(y)$$
$$y=\left( \frac{g_{J}\mu_{B}J}{k_{B}T} \right)\lambda M\implies M=\left( \frac{k_{B}T}{\lambda g_{J}\mu_{B}J} \right)y.$$
The valid values of $M$ are the intercept of these two equations for $M$.
![[Pasted image 20250130143116.png]]
It can be seen that the gradient of the linear graph depends on temperature.
At a critical temperature, the Curie temperature $T_c$, there is only one interception at $M=0$ so this transitions to a paramagnet.
![[Pasted image 20250130143430.png]]
Applying a B field to a paramagnetic material causes a net magnetisation which aligns all the spins and creates a ferromagnet.
For a $J=\frac{1}{2}$ solid:
$$\frac{M}{M_{s}}=\frac{\mu_{B}}{k_{B}T}(B+\lambda M)$$
$$\implies \frac{M}{M_{s}}\left( 1-\frac{\lambda \mu_{B}M_{s}}{k_{B}T} \right)=\frac{\mu_{B}B}{k_{B}T}.$$
For weak magnetic materials
$$\chi=\frac{\mu_{0}M}{B}$$
$$\implies \chi=\frac{\mu_{0}\mu_{B}M_{s}}{k_{B}\left[ T-\frac{\lambda \mu_{B}M_{s}}{k_{B}T} \right]}\propto \frac{1}{T-T_{c}}.$$
![[Pasted image 20250130144454.png]]
