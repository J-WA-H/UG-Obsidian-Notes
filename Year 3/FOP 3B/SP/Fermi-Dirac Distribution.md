This [process](Maxwell-Boltzmann%20Distribution.md) can be repeated for fermions to obtain the Fermi-Dirac distribution. We have states $\epsilon_{j}$ that has $g_j$ degeneracy and we want to scatter $n_j$ particles into this state.

For state $\epsilon_{j}$ we only require 0 or 1 particles in each $g_j$ degeneracy, hence $n_{j}\leq g_{j}$ (Pauli exclusion).

To count states, we can label each of the $g_j$ as empty or full hence we are dividing them into two piles.
Number of microstates for $\epsilon_{j}$ is
$$\Omega_{j}(\epsilon_{j})=\frac{g_{j}!}{n_{j}!(g_{j}-n_{j})!}.$$
So for the total system we multiply the number of microstates in each $g_{j}$ states.
$$\Omega_{FD}=\prod_{j} \frac{g_{j}!}{n_{j}!(g_{j}-n_{j})!}.$$
We again aim to maximise entropy subject to the usual constraints on $N$ and $U$.
$$\frac{S}{k_{B}}=\ln\left[ \prod_{j} \frac{g_{j}!}{n_{j}!(g_{j}-n_{j})!} \right]=\sum_{j}(\ln g_{j}!-\ln n_{j}!-\ln(g_{j}!-n_{j}!)).$$
From [Stirling's approximation](Logs%20of%20Factorials.md) we get
$$\frac{S}{k_{B}}=\sum_{j}[g_{j}\ln g_{j}-\cancel{g_{j}}-(n_{j}\ln n_{j}-\cancel{n_{j}})-((g_{j}-n_{j})\ln(g_{j}-n_{j})-(g_{j}-\cancel{n_{j}}))]$$
so using [Lagrange multipliers](Stationary%20points%20&%20Lagrange%20Multipliers.md) 
$$L=\sum_{j}[g_{j}\ln g_{j}-n_{j}\ln n_{j}-(g_{j}-n_{j})\ln(g_{j}-n_{j})-\alpha n_{j}-\beta n_{j}\epsilon_{j}].$$
$$\frac{\partial L}{\partial n_{j}}=-\ln n_{j}-1+\ln(g_{j}-n_{j})+1-\alpha-\beta \epsilon_{j}=0$$
$$\implies \ln\left( \frac{g_{j}}{n_{j}}-1 \right)=\alpha+\beta \epsilon_{j}$$
$$\implies \frac{n_{j}}{g_{j}}=f_{FD}(\epsilon_{j})=\frac{1}{e^\alpha e^{\beta \epsilon_{j}}+1}.$$
This is the Fermi-Dirac distribution.