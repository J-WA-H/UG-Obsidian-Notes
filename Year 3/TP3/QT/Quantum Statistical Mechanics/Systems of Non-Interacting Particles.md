Consider systems with large number of non-interacting particles. Assume that they are equivalent and have the same energy levels. The total energy is given by
$$E=\sum_{j}n_{j}E_{j}$$
where $n_j$ is the number of particles in eigenstate $j$.

To total number of particles is
$$N_{s}=N=\sum_{j}n_{j}.$$
There are 3 different classes of $n_j$,
$$n_{j}=\begin{cases}
0,1,2,3,\dots & \text{distinguishable} & \text{Maxwell-Boltzmann} \\
0,1,2,3,\dots & \text{indistinguishable} & \text{Bose-Einstein} \\
0,1 & \text{indistinguishable} & \text{Fermi-Dirac}
\end{cases}.$$
We need the number of distinguishable states $g_{E}$ of the system corresponding to each energy level.

For MB, the wavefunction is the product of $N$ single particle wavefunctions $\psi=\phi_{E_{j}}(1)\phi_{E_{d}}(2)$.

Consider if all particles have different energies, there is an $n!$ degeneracy but if $n_j$ are in the same level, there is an $n_j!$ degeneracy
$$\therefore g_{E}^{MB}=\frac{N!}{\prod n_{j}!}.$$
There is only 1 totally symmetric wavefunction and 1 totally antisymmetric wavefunction.
If there are $N$ indistinguishable particles, $g_{E}^{BE}=1$ and
$$g_{E}^{FD}=\begin{cases}
1 & n_{j}=0,1 \\
0 & \text{Otherwise}
\end{cases}.$$
In every case the partition function $Q$ will be
$$Q_{N}(T)=\sum_{\{ n_{j} \}}g_{E}\exp\left[ -\beta \sum_{j}n_{j}E_{j} \right].$$
This is a sum over all possible set of $n_j$.

The average energy is
$$\langle E \rangle =\sum_{i}\langle n_{i} \rangle E_{i}.$$
$$\langle n_{i} \rangle =\frac{1}{Q_{N}(T)}\sum_{\{ n_{j} \}}g_{E}\exp\left[ -\beta \sum_{j}n_{j}E_{j} \right]n_{i}.$$
Consider
$$-\frac{d}{d(\beta E_{i})}\ln(Q_{N}(t))=-\frac{1}{Q_{N}} \frac{d}{d(\beta E_{i})}Q_{N}(T)=\frac{-1}{Q_{N}(T)} \frac{d}{d(\beta E_{i})}\sum_{\{ n_{j} \}} g_{E}\exp\left[ -\beta \sum_{j}n_{j}E_{j} \right]$$
$$=\frac{1}{Q_{N}(T)}\sum_{\{ n_{j} \}}g_{E}\exp\left[ -\beta \sum_{j}n_{j}E_{j} \right]n_{i}=\langle n_{i} \rangle.$$
$$\therefore \langle n_{i} \rangle =-\frac{d\ln Q_{N}(T)}{d(\beta E_{i})}.$$
For Maxwell-Boltzmann, 
$$Q_{N}(T)=\left[ \sum_{j}\exp[-\beta E_{j}] \right]^{N}.$$
$$\therefore \langle n_{j} \rangle =-\frac{d}{d(\beta E_{j})}\left( N\ln\left( \sum_{j}\exp[-\beta E_{j}] \right) \right)=-\frac{N}{\sum_{j}\exp[-\beta E_{j}]}e^{-\beta E_{i}}$$
$$=e^{-\beta E_{i}}\exp\left[ \ln\left( \frac{N}{\sum_{j}\exp[-\beta E_{j}]} \right) \right]=\exp\left[ -\beta E_{i}-\ln\left( \frac{\sum_{j}\exp[-\beta E_{j}]}{N} \right) \right]$$
The logarithm is a temperature dependent constant $\alpha$,
$$\therefore \langle n_{i} \rangle =\exp[-(\beta E_{j}+\alpha)].$$
This is the Maxwell-Boltzmann distribution.

It is more difficult to evaluate the Bose-Einstein or Fermi-Dirac distributions.

We need to move to the [[Grand Canonical Ensemble]] so the grand canonical partition function is
$$Z=\sum_{n_{1}=0}^{\infty}\sum_{n_{2}=0}^{\infty}\dots g_{E}\exp\left[ -\beta \sum_{j}n_{j}E_{j}-\alpha_{j}\sum_{j}n_{j} \right]$$
$$=\prod_{j}\sum_{j=0}^{\infty}g_{E}\exp[-n_{j}(\beta E_{j}+\alpha)].$$
For the Bose-Einstein, $g_{E}=1$ and $n_{j}, 0\to \infty$.
$$\therefore Z^{BE}=\prod_{j}\sum_{n_{j}=0}^{\infty}[\exp [-\beta E_{j}-\alpha]]^{n_{j}}=\prod_{j}\sum_{n_{j}=0}^{\infty}x^{n_{j}}=\prod_{j} \frac{1}{1-x}$$
$$=\prod_{j} \frac{1}{1-\exp[-\beta E_{j}-\alpha]}.$$
For FD, $g_{E}=0,1$, $n_{j}=0,1$.
$$Z^{FD}=\prod_{j}(1+\exp[-(\beta E_{j}+\alpha)])$$
$$\therefore \langle n_{i} \rangle =-\frac{d\ln Z}{d(\beta E_{i})}.$$
There are 2 cases,
BE:
	$$\langle n_{i} \rangle =-\frac{d}{d(\beta E_{i})}\ln\left[ \prod_{j} \frac{1}{1-\exp[-(\beta E_{j}+\alpha)]} \right]=\frac{d}{d(\beta E_{i})}\sum_{j}\ln(1-\exp[-(\beta E_{j}+\alpha)])$$
	$$=\frac{d}{d(\beta E_{i})}\ln(1-\exp[-(\beta E_{i}+\alpha)])=\frac{1}{1-\exp[-(\beta E_{i}+\alpha)]}\exp[-(\beta E_{i}+\alpha)]$$
	$$=\frac{1}{\exp[\beta E_{i}+\alpha]-1}.$$
	This is the Bose-Einstein distribution.

For Fermi-Dirac:
$$\langle n_{i} \rangle ^{FD}=-\frac{d}{d(\beta E_i)}\ln\left( \prod_{j}(1+\exp[-(\beta E_{j}+\alpha)]) \right)--\frac{d}{d(\beta E_{i})}\ln(1+\exp[-(\beta E_{i}+\alpha)])$$$$=\frac{e^{-(\beta E_{i}+\alpha)}}{1-\exp[-(\beta E_{i}+\alpha)]}=\frac{1}{\exp[\beta E_{i}+\alpha]+1}.$$
This is the Fermi-Dirac distribution.
This gives
$$\langle n_{i} \rangle =\frac{1}{\exp[\beta E_{i}+\alpha]+\gamma}$$
where
$$\gamma=\begin{cases}
0 & \text{MB} \\
-1 & \text{BE} \\
1 & \text{FD}
\end{cases}.$$
There are 2 interesting limits:
1. $\beta E_{i}+\alpha$ is large, $\gamma$ becomes insignificant so $n\approx e^{-(\beta E_{i}+\alpha)}$, a falling exponential
2. $\beta E_{i}+\alpha$ is small, where there is a difference between the distribution functions.

Bosons: $\gamma=-1$,
$$\exp[\beta E_{i}+\alpha]-1\approx\beta E_{i}+\alpha+\dots$$
There is a large distribution function so a large occupancy. 
This is a Bose-Einstein condensate - the macroscopic number of particles are a in the lowest energy level.

Fermions: $\gamma=1$:
$$\alpha=-\beta \mu\therefore n=\frac{1}{\exp[\beta(E-\mu)]+1}.$$
For large $\beta$, $T\to{0}$ so we get a step function.
$$E>\mu \implies n=0$$
$$E<\mu \implies n=1.$$
