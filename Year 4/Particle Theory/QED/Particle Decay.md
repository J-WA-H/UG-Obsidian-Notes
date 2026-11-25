Scattering amplitudes can also be used to calculate decays as well as scattering. Consider a scalar field decaying into two fermions.
![[Pasted image 20260131162416.png]]
Using Feynman's rules for a [scalar](Feynman%20Rules.md) and [fermion field](Electron%20Scattering%20off%20Static%20Potential.md)  
$$\mathcal{M}=\bar{u}(p_{1})(-ig)v(p_{2})\tag{11.1} $$
This gives
$$\overline{\sum}|\mathcal{M}|^2=\overline{\sum}|\bar{u}(p_{1})(-ig)v(p_{2})|^2g^2=\mathrm{Tr}[(p\!\!\!/_{1}+m)(p\!\!\!/_{2}-m)]g^2=4g^2(p_{1}p_{2}-m^2)=2g^2(M_{\phi}^2-4m^2).\tag{11.2} $$This comes from
$$(p_{1}+p_{2})^2=2p_{1}p_{2}+2m^2=M_{\phi}^2\implies{4}p_{1}p_{2}=2M_{\phi}^2-4m^2.\tag{11.3} $$
This can be used to calculate the decay width, which gives the inverse lifetime of the particle. It is given by the incoming flux,
$$\Gamma=\frac{1}{2M_{\phi}} \int \frac{d^3p_{1}d^3p_{2}}{(2\pi)^32E_{1}(2\pi)^32E_{2}}\overline{\sum}|\mathcal{M}|^2(2\pi)^4\delta^{(4)}(P-p_{1}-p_{2}).\tag{11.4} $$
Since everything is fixed in terms of mass, this integral evaluates to $2^n\pi^mf\left( \frac{m^2}{M_{\phi}^2} \right)$.