Like the [[Canonical Ensemble]], consider a system in a large reservoir,
![[Pasted image 20250211192106.png]]
In this case the exchange of particles is allowed between the reservoir and the system but the total number of particles, $N=N_{R}+N_{S}$ is constant.

Derivation: Proceeds as before for the canonical ensemble but $S_{R}=S_{R}(E_{R},N_{R})$.
$$S_{R}(E_{R},N_{R})\approx S_{R}(E,N)-\frac{\partial S_{R}(E,N)}{\partial E}E_{N}(N_{S})-\frac{\partial S_{R}(E,N)}{\partial N}N_{S}.$$
Call
$$\frac{\partial S_{R}}{\partial N}=-\frac{\mu}{T}$$
where $\mu$ is the chemical potential.
$$S_{R}(E_{R},N_{R})\approx S_{R}(E,N)-\frac{E_{n}(N_{S})}{T}+\frac{\mu}{T}N_{S}.$$
This gives the [[Density Operator]]
$$\rho_{nm}=B\exp[-\beta E_{n}+\beta \mu N_{S}]\delta_{nm}=B\exp[-\beta E_{n}(N_{S})-\alpha N_{S}]\delta_{nm}$$
where
$$\alpha=\frac{1}{k_{B}} \frac{\partial S_{R}}{\partial N}.$$
In operator notation, $\nu_{S}$ is the number operator.
$$\mathrm{Tr}(\rho)=1=\frac{1}{B}=Z(\alpha,T)=\mathrm{Tr}(\exp[-\beta H(\nu_{S})-\alpha \nu_{S}]).$$
This gives the grand partition function,
$$Z=\sum_{N}\sum_{n}\exp[-\beta E_{n}(N)-\alpha N]$$
We can write $e^{-\alpha N}=(e^{-\alpha})^{N}$ and define fugacity, $z=e^{=\alpha}$.
$$Z=\sum_{N}Q_{N}(T)z^{N}$$
where $Q_N(T)$ is the partition function for a system of $N$ particles.
