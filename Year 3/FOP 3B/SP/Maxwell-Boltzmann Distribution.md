We can use the [Boltzmann entropy](Boltzmann%20Entropy.md) for [degenerate](Degeneracy.md) energy state and maximise it subject to constraints
$$\sum_{j}n_{j}=N;\;\sum_{j}n_{j}\epsilon_{j}=U.$$
Using [Lagrange multiplies](Stationary%20points%20&%20Lagrange%20Multipliers.md) 
$$L=\sum_{j}[n_{j}\ln g_{j}-(n_{j}\ln n_{j}-n_{j})-\alpha n_{j}-\beta n_{j}\epsilon_{j}].$$
Now maximise $L$
$$\frac{\partial L}{\partial n_{j}}=\ln g_{j}-\ln n_{j}+1-1-\alpha-\beta\epsilon_{j}=0$$
$$\implies \ln\left( \frac{g_{j}}{n_{j}} \right)=\alpha+\beta \epsilon_{j}.$$
$$\implies \frac{n_{j}}{g_{j}}=e^{-\alpha}e^{-\beta \epsilon_{j}}=f_{MB}(\epsilon_{j}).$$
This is the Maxwell-Boltzmann distribution which for large $N$ holds for distinguishable/classical particles.
