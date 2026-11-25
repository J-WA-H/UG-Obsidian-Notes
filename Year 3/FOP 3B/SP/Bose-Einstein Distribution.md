The Bose-Einstein distribution gives the most likely distribution for bosons.

The number of microstates is given by
$$\Omega(\epsilon_{j})=\frac{(n_{j}+g_{j}-1)!}{n_{j}!(g_{j}-1)!}$$
Hence the total microstates is
$$\Omega_{BE}=\prod_{j} \frac{(n_{j}+g_{j}-1)!}{n_{j}!(g_{j}-1)!}=\prod_{j} \frac{(n_{j}+g_{j})!}{n_{j}!g_{j}!}.$$
the 1 doesn't matter since $n_{j}$ and $g_{j}$ are large.
$$\frac{S}{k_{B}}=\sum_{j}[(n_{j}+g_{j})\ln(n_{j}+g_{j})-n_{j}\ln n_{j}-g_{j}\ln g_{j}].$$
[Maximising](Stationary%20points%20&%20Lagrange%20Multipliers.md) this with the normal constraints gives the Bose-Einstein distribution
$$f_{BE}(\epsilon_{j})=\frac{1}{e^\alpha e^{\beta \epsilon_{j}}-1}.$$
If we fix a particle number $N$ it appears as the term $e^{\alpha}$. $\alpha$ is some constant so take
$$\alpha=-\frac{\mu}{k_{B}T}.$$
$\mu$ is known as the Fermi-energy.
![[Pasted image 20241107163128.png]]
