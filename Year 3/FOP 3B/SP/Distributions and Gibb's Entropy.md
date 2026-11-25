Recall a [simple permutation problem](Basic%20Ideas,%20Probability%20and%20Distributions.md) where we are organising a large number of particles into two groups and counting the possible number of compositions of the groups.

Plot choose function with radius:
N=10 (small)
![[Pasted image 20241017144451.png]]
N=100 (Larger):
![[Pasted image 20241017144520.png]]
N=very big:
![[Pasted image 20241017144550.png]]
We want to find the most likely distribution subject to constraints that the total number of particles are constant and the total internal energy is constant.
$$N=\sum_{j}n_{j};\; U=\sum_{j}n_{j}\epsilon_{j}$$
The number of microstates for a given distribution ${n_j}$ is given by
$$\Omega(\{n_{j}\})=\frac{N!}{\prod_{j}n_{j}!}.$$
Using [Boltzmann entropy](Boltzmann%20Entropy.md), we get
$$S(\{n_{j}\})=k_{B}\ln\left( \frac{N!}{\prod_{j}n_{j}!} \right)$$
$$\frac{S}{k_{B}}=\ln (N!)-\ln\left( \prod_{j}n_{j}! \right)=\ln(N!)-\sum_{j}\ln(n_{j}!)$$
Using [Stirling's approximation](Logs%20of%20Factorials.md), we get
$$\frac{S}{k_{B}}=N\ln N-\cancel N-\sum_{j}(\ln n_{j}-\cancel{n_{j}})$$
$$=\sum_{j}n_{j}\ln (N)-\sum_{j}n_{j}\ln(n_{j})=-\sum_{j}n_{j}(\ln(n_{j})-\ln(N))$$
$$=-\sum_{j}n_{j}\ln\left( \frac{n_{j}}{N} \right)\; \div N$$
$$\frac{S}{k_{B}N}=-\sum_{j} \frac{n_{j}}{N}\ln\left( \frac{n_{j}}{N} \right)$$
The probability of finding a particle in state $j$ is given by $p_{j}=\frac{n_{j}}{N}$ which gives
$$S=-Nk_{B}\sum_{j}p_{j}\ln(p_{j})$$
This is known as the **Gibb's entropy**