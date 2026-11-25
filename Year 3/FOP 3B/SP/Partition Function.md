Recall [Expansion of Boltzmann entropy](Distributions%20and%20Gibb's%20Entropy.md) from the Stirling approximation:
$$\frac{S}{k_{B}}=N\ln N-\sum_{j}(n_{j}\ln n_{j}).$$
We aim to maximise this subject to the constraints $\sum_{j}n_{j}=N$ and $\sum_{j}n_{j}\epsilon_{j}=U$. To do this we will use the method of [Lagrange multipliers](Stationary%20points%20&%20Lagrange%20Multipliers.md).
$$L(n_{1},n_{2},\dots)=N\ln N-\sum_{j}n_{j}\ln(n_{j})-\alpha\left( \sum_{j}n_{j} \right)-\beta\left( \sum_{j}n_{j}\epsilon_{j} \right)$$
where $\alpha$, $\beta$ are the Lagrange multipliers.
As the derivative for each state, we have
$$\frac{\partial L}{\partial n_{j}}=-\ln(n_{j})-1-\alpha-\beta \epsilon_{j}=0.$$
Rewrite $A=1-\alpha$ and rearrange for $n_{j}$
$$n_{j}=e^Ae^{-\beta \epsilon_{j}}.$$
This follows that the number of particles in an occupied energy level undergoes [exponential decay](Counting%20states.md).

This equation gives the most likely distribution of particles in a system with constant $N$ and $U$.

This gives that the total number of particles in a system is given by
$$N=\sum_{j}n_{j}=e^A\sum_{j}e^{-\beta \epsilon_{j}}.$$
We now define the **partition function**
$$Z=\sum_{j}e^{-\beta \epsilon_{j}}.$$
This definition gives us a value of $A$,
$$e^A=\frac{N}{Z}$$
$$\implies n_{j}=\frac{N}{Z}e^{-\beta \epsilon_{j}}$$
and
$$p_{j}=\frac{1}{Z}e^{-\beta \epsilon_{j}}.$$
This shows $Z$ acts as a normalisation constant for the probability.
We can use this definition to calculate other thermodynamical quantities.

We can rewrite [Gibb's entropy](Distributions%20and%20Gibb's%20Entropy.md) in terms of $Z$:
$$S=-Nk_{B}\sum_{j}p_{j}\ln (p_{j})=-Nk_{B}\sum_{j}p_{j}\left( -\frac{\epsilon_{j}}{k_{B}T}-\ln(Z) \right)$$
We know internal energy is $U=N\sum_{j}p_{j}\epsilon_{j}$,
$$S=\frac{U}{T}+Nk_{B}\ln(Z).$$
We can find the Free energy of the system, $F=U-TS$.
Hence:
$$F=-Nk_{B}T\ln(Z).$$
