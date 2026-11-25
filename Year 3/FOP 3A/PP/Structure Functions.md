[[Inelastic Scattering]] needs to be described by two independent parameters: $(Q^2,\nu)$, or $(E',\theta)$ where $\theta$ is the angle of scattering.
Note for elastic scattering this reduces to one variable from $2m_{p}\nu-Q^2=1$.

We often use dimensionless quantities so we can define
$$X=\frac{Q^2}{2m_{p}\nu}\implies 0\leq X\leq 1.$$
$X$ measures how inelastic a collision, where $0$ is fully inelastic and $1$ is fully elastic.

This allows us to define structure functions [similar to](Helicity.md) $G_{E}$ and $G_{M}$ for inelastic scattering, 
$$Y=\frac{p_{p}q}{p_{p}p_{e}}$$
where $Y$ gives the fractional loss of energy of the incoming electron.
The inelastic version of Rosenbluth's formula is:
$$\frac{\partial^2\sigma}{\partial Q^2\partial X}=\frac{4\pi \alpha^2}{Q^4}\left[ \left( 1-Y-\frac{m_{p}^2Y^2X^2}{Q^2} \right) \frac{F_{2}(X,Q^2)}{X}+Y^2F_{1}(X,Q^2) \right].$$
This gives structure functions $F_{1},F_{2}$ analogous to $G_{E},G_{M}$.
Plotting these functions for the three types of scattering gives

![[Pasted image 20250124095923.png]]
![[Pasted image 20250124100001.png]]
![[Pasted image 20250124100015.png]]
For a given $X$ we find that $F_{1},F_{2}$ gives information on the structure of the target particle.
Consider the inelastic scattering of an electron off of a proton:
![[Pasted image 20250130185036.png]]
Each internal particle particle carries a fraction of the 4-momentum, $\eta_{i}$
$$\sum \eta_{i}=1.$$
If we fix $Q^{2}\approx 100\text{ GeV}\gg m_{p}$ so we can take the proton mass to be zero.
$$k^2=0=(\eta_{1}p_{p}+p_{e}-p'_{e})^2=(n_{1}p_{p}+q)^2=\eta_{1}^2p_{p}^2+2\eta_{1}p_{p}q+q^2$$
$$=2\eta_{1}p_{p}-Q^2=2\eta_{1}p_{p}q-Q^2\implies \eta_{i}=\frac{Q^2}{2p_{p}q}=\frac{Q^2}{2m_{p}\nu}=X.$$
