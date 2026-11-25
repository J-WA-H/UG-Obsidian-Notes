Looking at some experimental scattering results for $Q\approx 0$, for the proton, the structure functions in the [Rosenbluth formula](Helicity.md) are
$$Q_{E}^{P}(Q^2\approx0)=1\text{ - charge of proton}$$
$$G_{M}^{P}(Q^2\approx 0)=2.79.$$
We'd expect $G_M$ to give the spin, so $\frac{1}{2}$, but this is not what is observed. For the neutron:
$$G_{E}^{N}(Q^2\approx 0)=0\text{ - as expected, charge of neutron}$$
$$G_{M}^{N}(Q^2\approx 0)= -1.991.$$
As the neutron has no charge, it should not produce a magnetic field - but it does so it must contain some charged substructure.

Considering a scattering event using quantum field theory - relativistic quantum mechanics - we have individual packets of [4-Momentum](4-Momentum%20Conservation.md) transferred from the bullet to the target, instead of a continuous field $V(r)$:
![[Pasted image 20250123184720.png]]
The transfer mechanism is a virtual particle.
The virtual particle can borrow energy $\Delta E$ for a time $\Delta t$, given by $\Delta E\Delta t\approx \frac{\hbar}{2}$.
Mathematically, the propagator is
$$\frac{1}{q^2-M^2}$$
where $M$ is the mass of the virtual particle.

We also have vertices and these are the strength of the interaction. If the interaction is electromagnetic then the virtual particle is a photon, with mass $0$ and the strength is proportional to the charge.

We can evaluate the matrix element $\mu$ from this diagram:
$$\mu=\frac{eZ_{1}eZ_{2}}{q^2-\cancelto{0}{M^2}}$$
which gives the [[Cross-Sections]]	
$$\sigma \propto |\mu|^2=\frac{(eZ_{1})^2(eZ_{2})^2}{q^4}.$$
This is the Rutherford formula.
