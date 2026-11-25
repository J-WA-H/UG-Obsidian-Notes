 We can find expressions for the [fields](Vector%20and%20Scalar%20Potentials.md) from the expressions for the [potentials](Fields%20from%20Continuous%20Distributions.md).
For $\underline{E}$:
$$\underline{E}=-\underline{\nabla}\phi-\frac{\partial \underline{A}}{\partial t}.$$
$$\frac{\partial \underline{A}}{\partial t}=\frac{\mu_{0}}{4\pi}\int_{V'} \frac{\partial \underline{j}}{\partial t} \frac{1}{R}dV'=\frac{1}{4\pi\varepsilon_{0}} \frac{1}{c_{2}}\int_{V'} \frac{\partial \underline{j}}{\partial t} \frac{1}{R} dV'$$
$$-\underline{\nabla}\phi=-\frac{1}{4\pi\varepsilon_{0}} \int_{V'}\left[ -\frac{\dot{\rho}}{c} \frac{\underline{\hat{R}}}{R}-\frac{\rho \underline{\hat{R}}}{R^2} \right]dV'$$
This gives 
$$\underline{E}=\frac{1}{4\pi\varepsilon_{0}}\int_{V'}\left[ \rho  \frac{\underline{\hat{R}}}{R^2}+\frac{1}{c} \frac{\partial\rho}{\partial t} \frac{\underline{\hat{R}}}{R}-\frac{\partial\underline{j}}{\partial t} \frac{1}{c^2R} \right]dV'.$$
This is the first Jefimemko equation.

For $\underline{B}$:
$$\underline{\nabla}\times\left( \frac{\underline{j}}{R} \right)=\frac{1}{R}(\underline{\nabla}\times \underline{j})-\underline{j}\times \underline{\nabla}\left( \frac{1}{R} \right)$$
$$\implies \underline{\nabla}\times \underline{A}=\frac{\mu_{0}}{4\pi}\int_{V'}\left[ \frac{1}{R}(\underline{\nabla}\times \underline{j})-\underline{j}\times \underline{\nabla}\left( \frac{1}{R} \right) \right]dV'.$$
$$\underline{\nabla}\times \underline{j}=\frac{1}{c}\left[ \frac{\partial}{\partial}\underline{j}(\underline{r}',t_{r})\times \underline{\nabla}R \right]=\frac{1}{c}\left( \frac{\partial\underline{j}}{\partial t} \times \underline{\hat{R}}\right).$$
This gives
$$\underline{B}=\frac{\mu_{0}}{4\pi}\int_{V}\left[ \frac{\underline{j}(\underline{r}',t_{r})}{R^2}+\frac{\partial\underline{j}}{\partial t} \frac{1}{cR} \right]\times \underline{\hat{R}}dV'.$$
This is the second Jefimemko equation.
Note that these equations are not just the static case with the retarded time inserted, like the potentials. If we did this for the fields we would not get the correct solutions. A valid solution to Maxwell's equation for potential would also have been obtained by using advanced time $t_{a}=t+\frac{R}{c}$ - however since this violates causality. Disregarding physics, both solutions arise because $\square$ involves a second time derivative term so is invariant under time reversal.