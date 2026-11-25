The evolution of density perturbations depend critically on the sound speed $c_{s}$, which is very different before and after recombination.

At early times, baryonic matter is completely ionised. Recombination to neutral atoms happens at $z_{rec}\approx 1000$ with $T\approx 3000\text{ K}$, $a_{rec}=10^{-3}$.

Before recombination:
![[Pasted image 20251101160335.png]]
For $a<a_{rec}$, baryons are fully ionised. The Thomson scattering of photons or the free electrons result in a very short mean free path for photons. Baryons and photons are locked together and behave as a single baryon-fluid with the same temperature $T$.

After recombination:
![[Pasted image 20251101160612.png]]
For $a>a_{rec}$, baryons are in neutral atoms (H and He). Photons have decoupled from baryons so we have two separate fluids, baryons - normal [collisional fluid](Fluid%20Equations.md), and photons - a collisionless free-streaming fluid.

Consider a blackbody radiation of temperature $T$ contained in a fixed volume $V$ with energy density $u=\alpha_{r}T^4$ with $\alpha_{r}=\frac{4\sigma}{c}$. The interna; energy is
$$U=uV=\alpha_{r}T^4V\tag{14.1} .$$The second law of thermodynamics gives
$$dU=TdS-pdV.\tag{14.2} $$
Consider raising temperature at a fixed volume, $dV=0$,
$$dS=\frac{dU}{T}=4\alpha_{r}T^4dTV\tag{14.3} .$$
Integrating from $S=0$ at $T=0$ gives a total entropy in volume $V$,
$$S=\frac{4}{3}\alpha_{r}T^3V.\tag{14.4} $$which gives an entropy of density of photons as
$$s_{\gamma}=\frac{4}{3}\alpha_{r}T^3.\tag{14.5} $$
Baryons and photons behave as a single coupled fluid with
$$\begin{matrix}
\rho=\rho_{\gamma}+\rho_{b}, & \rho_{b}=n_{b}m_{p}, & \rho_{\gamma}=\frac{\alpha_{r}T^4}{c^2}
\end{matrix}\tag{14.6} $$
and $\rho_{b}\ll \rho_{\gamma}$ as $n_{\gamma}\gg n_{b}$ which gives the total pressure
$$p\approx p_{\gamma}=\frac{1}{3}\rho_{\gamma}c^2\tag{14.7} .$$
As $s_{b}\ll s_{\gamma}$, entropy per unit volume is
$$s=s_{b}+s_{\gamma}\approx s_{\gamma}=\frac{4}{3}\alpha_{r}T^4\tag{14.8} $$
so the entropy per baryon is
$$\tilde{S}=\frac{s}{n_{p}}\propto \frac{T^3}{n_{b}}\propto \frac{\rho_{\gamma}^{3/4}}{\rho_{b}}.\tag{14.9} $$Considering adiabatic perturbations have $\tilde{S}=\text{const}$ so $\delta \tilde{S}=0$ with
$$\frac{\delta \tilde{S}}{\tilde{S}}=\frac{3}{4} \frac{\delta \rho_{\gamma}}{\rho_{\gamma}}-\frac{\delta \rho_{b}}{\rho_{b}}\tag{14.10} $$
we get
$$\frac{\delta \rho_{b}}{\rho_{b}}=\frac{3}{4} \frac{\delta \rho_{\gamma}}{\rho_{\gamma}}=3 \frac{\delta T}{T}.\tag{14.11} $$
These density and pressure perturbations become
$$\delta p=\frac{1}{3}c^2\delta \rho_{\gamma},\;\delta \rho=\delta \rho_{\gamma}+\delta \rho_{b}=\delta \rho_{\gamma}+\frac{3}{4}\left( \frac{\rho_{b}}{\rho_{\gamma}} \right)\delta \rho_{\gamma}.\tag{14.12} $$
This gives a sound wave speed of
$$c_{s}=\frac{c}{\sqrt{ 3 }} \frac{1}{\left( 1+\frac{3}{4} \frac{\rho_{b}}{\rho_{\gamma}} \right)^{1/2}}.\tag{14.13} $$
$c_{s}\approx \frac{c}{\sqrt{ 3 }}$ if $\rho_{b}\ll \rho_{\gamma}$ which is valid until recombination since $\frac{\rho_{b}}{\rho_{\gamma}}\propto a$ and $\rho_{b}=\rho_{\gamma}$.

After recombination, baryons behave as a normal gas, $\rho=n_{b}m_{p}$, $p=n_{b}k_{B}T_{b}$. For adiabatic perturbations in a monatomic ideal gas, $p\propto \rho^{5/3}$, the sound speed is
$$c_{s}=\left( \frac{\partial p}{\partial \rho} \right)^{1/2}_{ad}=\left( \frac{5}{3} \frac{p}{\rho} \right)^{1/2}=\left( \frac{5}{3} \frac{k_{B}T_{b}}{m_{p}} \right)^{1/2}.\tag{14.14} $$
For $150 \lesssim z <1000$, weak thermal coupling between the baryons and photons due to a small residual ionised fraction keeps
$$T_{b}\approx T_{\gamma}=T_{\gamma_{0}}a^{-1}.\tag{14.15} $$
This gives a sound speed that decreases with time
$$c_{s}=\left( \frac{5}{3} \frac{k_{B}T_{\gamma_{0}}}{m_{p}} \right)^{1/2}a^{-1/2}.\tag{14.16} $$
Sound waves in the universe at recombination produce temperature fluctuations in the CMB. The [[Jean's Length]] at recombination is around $1^{\circ}$. $\delta T$ on smaller scales gives evidence for sound waves at early times.

