A system has energy levels $\epsilon_{1}$, $\epsilon_{2}$, $\dots$. If they are double degenerate then each energy contains two states.
If $\epsilon_{j}$ has degeneracy $g_{j}$ then
$$U=\sum_{j}g_{j}\epsilon_{j}.$$
We shall start [[Counting states]] for degenerate levels:
Recall:
$$\Omega(\{n_{j}\})=\frac{N!}{\prod_{j}n_{j}!}.$$
Let state $\epsilon_{1}$ be $g_{1}$ fold degenerate. The number of configurations are $g_{1}^{n_{1}}$ so 
$$\Omega(\{n_{j}\})=N! \frac{g_{1}^{n_{1}}}{\prod_{j}n_{j}!}.$$
Have another $g_{2}$ fold degenerate state $\epsilon_{2}$
$$\Omega(\{n_{j}\})=N! \frac{g_{1}^{n_{1}}g_{2}^{n_{2}}}{\prod_{j}n_{j}!}.$$
We can generalise this to
$$\Omega(\{n_{j}\})=N!\prod_{j} \frac{g_{j}^{n_{j}}}{n_{j}!}.$$
Now we have $\Omega$, we can now find the [entropy](Boltzmann%20Entropy.md),
$$\frac{S}{k_{B}}=\sum_{j}[n_{j}\ln g_{j}-(n_{j}\ln n_{j}-n_{j})].$$
