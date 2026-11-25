Mesons consist of a quark and an antiquark. The mass of mesons are dependent on the binding energy between them as well as the quark masses.
This binding energy is dependent on [quantum numbers](Notation%20for%20Bound%20States.md) $n$, $L$, and $S$.
![[Pasted image 20250220183725.png]]
Consider the EM production of charmonium from positronium ($e^{-}e^{+}$),
![[Pasted image 20250220183948.png]]
As the photon has a spin of 1, conservation of angular momentum means that the resulting charmonium state must have a spin of 1 and orbital angular momentum 0 as 1 configuration, which is the $1^{3}S_{1}$ particle, known as the $J/\psi$ particle.
This interaction cannot produce the $1^{1}S_{0}$, $\eta_{c}$ particle as it breaks [conservation of angular momentum](Conserved%20Quantities.md).

The [magnetic moment](Magnetic%20Dipoles.md) is $\underline{\mu}=\frac{e}{2m}\underline{S}$, which when put into the Dirac equation and expand the potential to first order we get positronium ($e^{-}e^{+}$),
$$V^{QED}=\frac{8\pi}{3} \frac{\alpha}{m_{e}m_{e^{+}}}\underline{S}_{1}\cdot \underline{S}_{2}\delta(\underline{r}).$$
The $\delta$-function makes sure the particles are close together. This holds for electromagnetic binding, like positronium.

Mesons are bound by the strong force, hence this is adjusted for gluons and the strong coupling constant $\alpha_{s}$.
The magnetic dipole is the same so multiplying the terms give
$$V^{QCD}=\frac{32\pi}{9} \frac{\alpha_{s}}{m_{q}m_{\bar{q}}}\underline{S}_{1}\cdot \underline{S}_{2}\delta(\underline{r}).$$
The denominator has increased by a factor of 3 to take into account colour, and the numerator has been multiplied by $2^{2}$ which comes from gluons colour/anti-colour and how they can't be separated.

The energy associated with this spin-spin interaction is $\bra{\psi}V\ket{\psi}$ so we get $\bra{\psi}V\delta(\underline{r})\ket{\psi}=V|\psi(0)|^{2}$.
To evaluate the spin product, it is not as simple as a simple dot product.
Consider the total spin operator $\hat{S}=\hat{S}_{1}+\hat{S}_{2}$.
$$\hat{S}^2=(\hat{S}_{1}+\hat{S}_{2})^2=\hat{S}_{1}^{2}+\hat{S}_{2}^2+2\hat{S}_{1}\hat{S}_{2}.$$
Let $\hat{S}^2$ act on the meson:
$$S(S+1)=s_{1}(s_{1}+1)+s_{2}(s_{2}+1)+2s_{1}s_{2}.$$
For quarks, $s_{1}=s_{2}=\frac{1}{2}$.
$$S(S+1)=\frac{1}{2}\left( \frac{1}{2}+1 \right)+\frac{1}{2}\left( \frac{1}{2}+1 \right)+2s_{1}s_{2}=\frac{3}{4}+\frac{3}{4}+2s_{1}s_{2}.$$
$$\implies s_{1}s_{2}=\frac{1}{2}S(S+1)-\frac{3}{4}.$$
$$\therefore E=\frac{32\pi}{9} \frac{\alpha_{s}}{m_{q}m_{\bar{q}}}|\psi(0)|^2{\left[ \frac{1}{2}S(S+1)-\frac{3}{4} \right]}.$$
Now $\Delta E$ is known, the difference between the energy for $S=0$ and $S=1$, this can be applied to any $q\bar{q}$ pair.
![[Pasted image 20250220190139.png]]
Because of $|\psi(0)|^2$ term, the difference in energy is approximately 0 for the $P$ state.

The dissociation level is the maximum energy level a meson can exist. As the state is excited, the [[Gluons]] strength increases so at some point it will be more efficient to form other particles with lower energy.
![[Pasted image 20250220190638.png]]
![[Pasted image 20250220190554.png]]

